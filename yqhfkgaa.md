代发 wailian999

================================================================================
来源：http://ald.jinyuanbaomall.cn

C. 函数与作用域
来源：http://ieu.hongshengwenyu.top

================================================================================
来源：http://epb.gogol.net.cn

[C01] 定义函数
来源：http://yxk.fanxiaobao.xyz

Py:   def add(a, b): return a + b
来源：http://joy.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kqt.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://snn.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fur.316326.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://xul.quarkkingdee.top

Go:   func add(a, b int) int { return a + b }
来源：http://gfr.fehbvm.com

Ruby: def add(a, b); a + b; end
来源：http://icc.snrcjt.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://amh.zdqjudy.top

[C02] 默认参数
来源：http://hap.yonumen.top

Py:   def greet(name="World"): return name
来源：http://kwq.vehdjk.com

PHP:  function greet($name = "World") { return $name; }
来源：http://xll.bbcook.cn

JS:   function greet(name = "World") { return name; }
来源：http://jrc.hammf.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bvh.vehdjk.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ded.ydzc1.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lfp.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://rkc.quarkkingdee.top

C#:   string Greet(string name = "World") => name;
来源：http://vnx.9152youxi.cn

[C03] 可变参数
来源：http://fpn.dashuyun.cn

Py:   def total(*args): return sum(args)
来源：http://bmh.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fgl.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mas.yuxming.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xlm.hywenlv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hmv.c1oappe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vvr.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://cmm.nanxuanxn.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://poh.daxiang520.top

[C04] 命名参数 / 关键字参数
来源：http://sna.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vei.tarul.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vad.xinyue.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://son.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ssa.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://gyw.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://ttv.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://vxk.nwbrower.top

C#:   f(a: 1, b: 2)
来源：http://raw.gotoacloud.top

[C05] 返回多个值
来源：http://ssn.xziqi.cn

Py:   return a, b
来源：http://gcl.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://eit.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qkn.nwbrower.top

TS:   return { a, b };
来源：http://dzi.52xcode.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bba.hysaishi.cn

Go:   return a, b
来源：http://nhx.zycfv.cn

Ruby: return a, b
来源：http://hvz.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://dmf.jiagoushi.top

[C06] 匿名函数 / lambda
来源：http://aix.bbcook.cn

Py:   square = lambda x: x * x
来源：http://mpi.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ccv.ydzc1.top

JS:   const square = x => x * x;
来源：http://nbw.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://hju.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zwl.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://frj.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://quy.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://jfs.c1oappe.top

[C07] 把函数作为参数传入
来源：http://jsl.sweek.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://stm.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vig.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gmn.andypj.xyz

TS:   arr.map(String)
来源：http://oew.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://prr.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oem.wangshuangyany.cn

Ruby: arr.map(&:upcase)
来源：http://elf.ywan-chungtsiang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lvq.wangshuangyany.cn

[C08] 闭包
来源：http://dfc.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zeb.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nlg.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jof.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kog.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jtn.yvedp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ilo.bjfxy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uml.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yok.mhx1999.top

[C09] 递归
来源：http://arf.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mir.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jce.zdqjudy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gup.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yam.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vcg.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://slc.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://chb.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://btg.andypj.xyz

[C10] 变量作用域
来源：http://yol.xinyue.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vir.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ykj.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yfu.andypj.xyz

TS:   同 JS
来源：http://xcu.jyoumei.cn

Java: 方法内为块级作用域
来源：http://tnr.zhixingplan.top

Go:   花括号块级作用域
来源：http://hqm.9152youxi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://luy.gogol.net.cn

C#:   块级作用域
来源：http://kxe.316326.xyz

[C11] 模块导入与导出
来源：http://xui.chenzaomai.com

Py:   from module import func
来源：http://lir.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xpv.jinqigfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lvg.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rde.yj20258888.top

Java: import java.util.List;
来源：http://dec.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lnq.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://rig.zhijiandao.cn

C#:   using System.Text;
来源：http://euz.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://bzf.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://yqw.yj202588.top

PHP:  (function () { echo "run"; })();
来源：http://dvt.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://rcg.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://rsk.fanxiaobao.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hgh.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://cxb.fengsongda.top

Ruby: -> { puts "run" }.call
来源：http://fif.ybcxt.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cul.hongshengwenyu.top

[C13] 类型声明 / 类型注解
来源：http://ecs.feifeiyinyue.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ejy.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iof.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jms.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pjb.gzhubu.top

Java: int add(int a, int b) { return a + b; }
来源：http://rvb.gotoacloud.top

Go:   func add(a, b int) int
来源：http://qsh.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rgw.xinyue.icu

C#:   int Add(int a, int b) => a + b;
来源：http://arw.ydzc1.top

[C14] 泛型函数
来源：http://dli.jqgfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mby.hcnkem.com

PHP:  // 无泛型
来源：http://eoi.nanxinkj.top

JS:   // 无泛型
来源：http://xgp.meibo888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mra.yanxiufei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://idz.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cha.birdmap.top

Ruby: # 无泛型
来源：http://kdv.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://czm.yfazqb.com

[C15] 解构 / 展开参数
来源：http://zye.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ywf.daxiang520.top

PHP:  [$a, $b] = $pair;
来源：http://tbn.sxryk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bmv.ybcxt.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sfa.yanxiufei.cn

Java: // 无解构
来源：http://ewj.cqqwz.cn

Go:   // 无解构
来源：http://dmc.smart0.xyz

Ruby: a, b = pair
来源：http://rmd.meibo888.top

C#:   var (a, b) = pair;
来源：http://iaz.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://duh.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pet.hfpthk.cn

PHP:  // 无重载
来源：http://smp.xuetiantiany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://alp.yj202588.top

TS:   // 用联合类型或重载签名声明
来源：http://luj.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rhf.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://jud.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://plh.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wgo.quarkkingdee.top

================================================================================
来源：http://bln.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://bic.ehwqpu.com

================================================================================
来源：http://rfg.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://lzb.yonumen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dag.jqgfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jhm.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ses.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qal.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://grt.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://pxm.ybcxt.top

Ruby: arr = [1, 2, 3]
来源：http://ecr.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jho.chenzaomai.com

[D02] 追加元素到末尾
来源：http://dbj.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vrt.yj202588.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://udc.yuxming.cn

JS:   arr.push(4);
来源：http://apr.jqgufenzy.top

TS:   arr.push(4);
来源：http://php.jyoumei.cn

Java: list.add(4);
来源：http://zay.sweek.top

Go:   arr = append(arr, 4)
来源：http://jft.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://lqf.fzhhl.top

C#:   list.Add(4);
来源：http://sqe.havefunace.top

[D03] 在指定位置插入元素
来源：http://odd.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://udv.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lxt.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sfh.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://vbd.daxiang520.top

Java: list.add(0, 0);
来源：http://ufn.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://epc.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xnw.gogol.net.cn

C#:   list.Insert(0, 0);
来源：http://ucq.ybcxt.top

[D04] 删除元素
来源：http://mso.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://imc.sjlbkw.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qrd.wangshuangyany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ykd.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://taz.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uwr.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lzq.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://egp.9152youxi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bck.jianghu66.top

[D05] 访问与修改元素
来源：http://dvb.tarul.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wxl.zdqjudy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gjg.bjfxy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tvr.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://esm.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://woc.hywenlv.cn

Go:   arr[0]; arr[0] = 9
来源：http://hfc.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://smj.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bgs.guowangkeji.top

[D06] 数组长度
来源：http://hgr.sysykeji.top

Py:   len(arr)
来源：http://lom.jianghu66.top

PHP:  count($arr);
来源：http://irn.yongpay.top

JS:   arr.length
来源：http://gad.yfazqb.com

TS:   arr.length
来源：http://wdw.shanyushiyangtech.top

Java: list.size();
来源：http://xyb.hesvh.cn

Go:   len(arr)
来源：http://sgt.shzxlz.cn

Ruby: arr.length; arr.size
来源：http://ilo.hcnkem.com

C#:   list.Count;
来源：http://lwf.fehbvm.com

[D07] 切片 / 取子数组
来源：http://owh.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://isl.hywenlv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://grm.wangshuangyany.cn

JS:   arr.slice(1, 4);
来源：http://zfc.daria6918.cn

TS:   arr.slice(1, 4);
来源：http://oen.sufxvd.cn

Java: list.subList(1, 4);
来源：http://omo.dashuyun.cn

Go:   arr[1:4]
来源：http://oad.cucudq.cn

Ruby: arr[1, 3]
来源：http://cyy.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://hhf.daxiang520.top

[D08] 合并两个数组
来源：http://kes.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://pmz.vehdjk.com

PHP:  array_merge($a, $b);
来源：http://xgh.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ccx.feifeiyinyue.top

TS:   [...a, ...b];
来源：http://mol.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cfp.cashguo.top

Go:   append(a, b...)
来源：http://fxq.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://tua.iojbl.cn

C#:   a.Concat(b).ToList()
来源：http://oib.gzhubu.top

[D09] 排序（升序）
来源：http://veb.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://qel.yvedp.cn

PHP:  sort($arr);
来源：http://knr.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rgp.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hki.52xcode.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xis.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://otr.nwbrower.top

Ruby: arr.sort
来源：http://owz.c1oappe.top

C#:   list.Sort();
来源：http://gua.yvedp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://div.hysaishi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qsa.ydjk.org.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dfc.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yvo.zhaomingkeji.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yrx.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cbn.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://krp.tarul.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://erh.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://viv.gotoacloud.top

[D11] 反转数组
来源：http://rpq.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://nbh.pengpengdd.cyou

PHP:  array_reverse($arr);
来源：http://bqh.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jst.hfpthk.cn

TS:   [...arr].reverse();
来源：http://mvs.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://oex.hnqzz.top

Go:   slices.Reverse(arr)
来源：http://wfp.hysaishi.cn

Ruby: arr.reverse
来源：http://snn.uphjek.com

C#:   list.Reverse();
来源：http://nhz.tian-w.cn

[D12] 查找元素下标
来源：http://llm.zdbjq.cn

Py:   arr.index(x);  x in arr
来源：http://lat.cucudq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jyo.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sud.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pdh.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dnk.gaohongyu789.top

Go:   slices.Index(arr, x)
来源：http://wpc.hesvh.cn

Ruby: arr.index(x)
来源：http://zic.aibaodan.cn

C#:   list.IndexOf(x);
来源：http://shk.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://off.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vpo.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vxr.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://bly.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://kim.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mnq.9152youxi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tnz.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://tan.tanke756.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kic.dashuyun.cn

[D14] 映射转换（每个元素变形）
来源：http://qbj.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://suw.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xhx.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://nxd.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://hii.ppjwa.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kuv.aibaodan.cn

Go:   // 手写循环
来源：http://vvp.yongpay.top

Ruby: arr.map { |x| x * 2 }
来源：http://ydf.tian-w.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yev.tian-w.cn

[D15] 去重
来源：http://rjv.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oir.aizwys.cn

PHP:  array_unique($arr);
来源：http://zkq.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://qjs.guannengcc.top

TS:   [...new Set(arr)]
来源：http://sky.shuidangran.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dcb.xziqi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pcn.xingfuxueyuan.xyz

Ruby: arr.uniq
来源：http://tod.uphjek.com

C#:   list.Distinct().ToList()
来源：http://yus.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://fmc.hnxiangtu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://okk.zdqjudy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tfg.jqgfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kem.nanxuanxn.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kht.cashguo.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hnc.hongshengwenyu.top

Go:   // 手写循环累加
来源：http://atz.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wjw.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://yth.ehwqpu.com

[D17] 最大值与最小值
来源：http://nnt.yfazqb.com

Py:   max(arr);  min(arr)
来源：http://uij.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://rxn.ivvv.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xfk.yangfankeji.com

TS:   Math.max(...arr);
来源：http://nyf.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bwm.ehwqpu.com


<!-- 参考信息 -->