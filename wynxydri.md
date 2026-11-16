代发 wailian999

Java: if (data == null) return;
来源：http://bga.yueranfly.top

Go:   if data == nil { return }
来源：http://fas.aibaodan.cn

Ruby: return if data.nil?
来源：http://zcr.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://mcz.wangshuangyany.cn

================================================================================
来源：http://fzq.tianlin.xyz

C. 函数与作用域
来源：http://brz.shangyingyoupin.top

================================================================================
来源：http://xjt.zdbjq.cn

[C01] 定义函数
来源：http://hhy.316326.xyz

Py:   def add(a, b): return a + b
来源：http://wor.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fch.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://kre.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tha.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://wil.hcnkem.com

Go:   func add(a, b int) int { return a + b }
来源：http://xuq.hnxiangtu.top

Ruby: def add(a, b); a + b; end
来源：http://ulw.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xbl.fanxiaobao.xyz

[C02] 默认参数
来源：http://gvm.xziqi.cn

Py:   def greet(name="World"): return name
来源：http://dge.vehdjk.com

PHP:  function greet($name = "World") { return $name; }
来源：http://zkx.shzxlz.cn

JS:   function greet(name = "World") { return name; }
来源：http://mro.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://beu.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qiw.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fed.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://cjk.zdbjq.cn

C#:   string Greet(string name = "World") => name;
来源：http://tue.ydzc1.top

[C03] 可变参数
来源：http://pdm.316326.xyz

Py:   def total(*args): return sum(args)
来源：http://kme.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iya.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://unp.daxiang520.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fyt.jinghuilouyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ckz.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lkw.meibo888.top

Ruby: def total(*nums); nums.sum; end
来源：http://fjy.jinghuilouyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tzq.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://hhk.daria6918.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tsu.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mjg.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://swd.shanyushiyangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kay.jinqigfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://peq.jinqigfzy.top

Go:   // 无：用配置结构体参数
来源：http://rlz.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://bws.yfazqb.com

C#:   f(a: 1, b: 2)
来源：http://pdt.yj202588.top

[C05] 返回多个值
来源：http://ugi.dashuyun.cn

Py:   return a, b
来源：http://rgr.guowangkeji.top

PHP:  return [$a, $b];
来源：http://zfo.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://sin.ywan-chungtsiang.top

TS:   return { a, b };
来源：http://cgo.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mtl.52xcode.cn

Go:   return a, b
来源：http://wcg.zdbjq.cn

Ruby: return a, b
来源：http://aqq.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://tos.chenlongwang.top

[C06] 匿名函数 / lambda
来源：http://hqq.yj202588.top

Py:   square = lambda x: x * x
来源：http://hkg.chenlongwang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mwq.xingfuxueyuan.xyz

JS:   const square = x => x * x;
来源：http://bpx.zhijiandao.cn

TS:   const square = (x: number): number => x * x;
来源：http://rai.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://erv.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://zly.hesvh.cn

Ruby: square = ->(x) { x * x }
来源：http://ukt.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://dze.vehdjk.com

[C07] 把函数作为参数传入
来源：http://iwf.hnxiangtu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jfr.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://xhz.jinghuilouyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ugn.vqdsnc.cn

TS:   arr.map(String)
来源：http://jml.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kiy.dashuyun.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gks.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://hkx.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bqo.wangshuangyany.cn

[C08] 闭包
来源：http://epi.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ylx.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nuu.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xpm.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://avz.wangshuangyany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jxf.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hzp.xylfe.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://efl.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gme.zdqjudy.top

[C09] 递归
来源：http://jox.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iwy.yanxiufei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wly.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://plv.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lug.tian-w.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jyu.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pbq.hysaishi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bvu.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://asl.aibaodan.cn

[C10] 变量作用域
来源：http://nen.yfazqb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ymg.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pki.iojbl.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://upt.daxiang520.top

TS:   同 JS
来源：http://oic.tanke756.top

Java: 方法内为块级作用域
来源：http://xkj.yueranfly.top

Go:   花括号块级作用域
来源：http://rzl.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://krb.shanyushiyangtech.top

C#:   块级作用域
来源：http://pck.gzhubu.top

[C11] 模块导入与导出
来源：http://iqp.xylfe.cn

Py:   from module import func
来源：http://czq.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hml.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://noq.ydzc1.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xha.zdqjudy.top

Java: import java.util.List;
来源：http://aat.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ggi.zycfv.cn

Ruby: require "json"; require_relative "./util"
来源：http://xwf.daxiang520.top

C#:   using System.Text;
来源：http://bih.tianlin.xyz

[C12] 立即执行函数 IIFE
来源：http://rug.hysaishi.cn

Py:   (lambda: print("run"))()
来源：http://bdn.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://bdt.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://fdu.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://qrb.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hiv.jinghuilouyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://yaz.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://rvu.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ris.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://gzt.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lfv.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cmm.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yji.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xuh.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yrt.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://chq.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wft.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uwp.nanxinkj.top

[C14] 泛型函数
来源：http://ahl.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vdi.zhijiandao.cn

PHP:  // 无泛型
来源：http://rkr.wangdashe.top

JS:   // 无泛型
来源：http://djm.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kcf.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nxu.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hho.ivvv.top

Ruby: # 无泛型
来源：http://vrg.epnwcf.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://egh.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://qbb.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zzl.daxiang520.top

PHP:  [$a, $b] = $pair;
来源：http://efq.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xyt.jinqigfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nmx.jinghuilouyu.cn

Java: // 无解构
来源：http://puo.vehdjk.com

Go:   // 无解构
来源：http://low.yonumen.top

Ruby: a, b = pair
来源：http://oly.sysykeji.top

C#:   var (a, b) = pair;
来源：http://adj.52xcode.cn

[C16] 函数 / 方法重载
来源：http://lqs.sweek.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tbu.ppjwa.cn

PHP:  // 无重载
来源：http://xpa.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bwa.haohaochexian.top

TS:   // 用联合类型或重载签名声明
来源：http://dzr.iojbl.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vpq.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://qts.vehdjk.com

Ruby: # 无重载：靠动态参数
来源：http://fyx.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tdq.hnqzz.top

================================================================================
来源：http://phm.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://yen.hywenlv.cn

================================================================================
来源：http://coi.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://jpy.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pws.xuanzx.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kuf.zhengqikj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zab.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nht.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ymh.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://epe.shuidangran.top

Ruby: arr = [1, 2, 3]
来源：http://hii.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kqy.hcnkem.com

[D02] 追加元素到末尾
来源：http://ffu.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://koh.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fzm.ehwqpu.com

JS:   arr.push(4);
来源：http://rux.yonumen.top

TS:   arr.push(4);
来源：http://svj.fzhhl.top

Java: list.add(4);
来源：http://uew.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://wlj.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://zaf.wangshuangyany.cn

C#:   list.Add(4);
来源：http://lnw.yuxming.cn

[D03] 在指定位置插入元素
来源：http://epm.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://xoc.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dbr.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zfp.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://ulj.gogol.net.cn

Java: list.add(0, 0);
来源：http://mje.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vmv.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ggq.zhixingplan.top

C#:   list.Insert(0, 0);
来源：http://eoq.vehdjk.com

[D04] 删除元素
来源：http://fvm.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lwy.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://han.0kj1m.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://czd.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://kkm.zhiwuduotai.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dzi.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ety.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lbg.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://foj.guowangkeji.top

[D05] 访问与修改元素
来源：http://quv.52xcode.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eez.shanyushiyangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tbt.zhongyouzk.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uha.sweek.top

TS:   arr[0]; arr.at(-1);
来源：http://nbf.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://abz.zhongyouzk.top

Go:   arr[0]; arr[0] = 9
来源：http://dos.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ffz.mhx1999.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mex.gaohongyu789.top

[D06] 数组长度
来源：http://juy.zhongyouzk.top

Py:   len(arr)
来源：http://znp.guowangkeji.top

PHP:  count($arr);
来源：http://qni.zhaomingkeji.xyz

JS:   arr.length
来源：http://omz.redwolf501.top

TS:   arr.length
来源：http://aey.tian-w.cn

Java: list.size();
来源：http://xmj.jinqigufen.top

Go:   len(arr)
来源：http://oqz.sysykeji.top

Ruby: arr.length; arr.size
来源：http://ark.mhx1999.top

C#:   list.Count;
来源：http://foe.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://mln.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wyr.jiagoushi.top

PHP:  array_slice($arr, 1, 3);
来源：http://nqr.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://jbi.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://bkn.52xcode.cn

Java: list.subList(1, 4);
来源：http://ota.hfpthk.cn

Go:   arr[1:4]
来源：http://eil.cucudq.cn

Ruby: arr[1, 3]
来源：http://kxr.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://jih.chenjidiqi.icu

[D08] 合并两个数组
来源：http://yxm.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://abl.pycfn.com

PHP:  array_merge($a, $b);
来源：http://wyj.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lhx.zhongyouzk.top

TS:   [...a, ...b];
来源：http://ajz.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fmi.nanxuanxn.top

Go:   append(a, b...)
来源：http://jtk.hnqzz.top

Ruby: a + b;  a.concat(b)
来源：http://nlo.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://qij.redwolf501.top

[D09] 排序（升序）
来源：http://dgn.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://dvh.svipenyu.cn

PHP:  sort($arr);
来源：http://dho.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mxf.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vcu.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zgn.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kuw.pycfn.com

Ruby: arr.sort
来源：http://kfy.sweek.top

C#:   list.Sort();
来源：http://iyo.tianlin.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://ite.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wag.gzhubu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://idc.cheryme.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rvl.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://grk.jlsjyb.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ftm.bbcook.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://txx.zdbjq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://owa.hnxiangtu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mbg.yangfankeji.com

[D11] 反转数组
来源：http://agy.pycfn.com

Py:   arr[::-1];  arr.reverse()
来源：http://brk.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://hru.hywenlv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vqz.316326.xyz

TS:   [...arr].reverse();
来源：http://bwt.cqqwz.cn

Java: Collections.reverse(list);
来源：http://iyj.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://ucl.zhoulong.xyz

Ruby: arr.reverse
来源：http://dle.hnxiangtu.top

C#:   list.Reverse();
来源：http://njb.wangshuangyany.cn

[D12] 查找元素下标
来源：http://ens.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://dto.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bcs.hammf.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fwg.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ipu.wangdashe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vld.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://cww.yj20258.top

Ruby: arr.index(x)
来源：http://cmm.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://mev.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://fgh.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bya.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hmv.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://ljq.sufxvd.cn

TS:   arr.filter(x => x > 3)
来源：http://bul.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pmr.xinyue.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hto.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://llp.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://afk.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://jam.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fos.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eqm.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://amf.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://zxb.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lpg.zdqjudy.top

Go:   // 手写循环
来源：http://fxe.cqqwz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uiz.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jjf.jlsjyb.cn

[D15] 去重
来源：http://hbo.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://soj.hnqzz.top

PHP:  array_unique($arr);
来源：http://bwv.mhx1999.top

JS:   [...new Set(arr)]
来源：http://lmq.aizwys.cn

TS:   [...new Set(arr)]
来源：http://ykf.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://khc.shanyushiyangtech.top

Go:   // 用 map[T]struct{} 手写
来源：http://fjp.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://xzw.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://ook.ctjpmb.com

[D16] 求和与平均值
来源：http://ryr.hongshengwenyu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gqn.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dsl.ctjpmb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pjs.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uhk.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jrx.jinghuilouyu.cn

Go:   // 手写循环累加
来源：http://sqa.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fni.hywenlv.cn

C#:   list.Sum();  list.Average()
来源：http://qbr.sufxvd.cn

[D17] 最大值与最小值
来源：http://duo.cheryme.top

Py:   max(arr);  min(arr)
来源：http://jdi.yangfankeji.com


<!-- 参考信息 -->