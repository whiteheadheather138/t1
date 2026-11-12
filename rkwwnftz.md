代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://fxz.smart0.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://qgh.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://vyo.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qwd.fzhhl.top

[C02] 默认参数
来源：http://kti.daxiang520.top

Py:   def greet(name="World"): return name
来源：http://ldg.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lbp.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://fox.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zvv.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://age.hongshengwenyu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jqe.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://lit.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://caj.shanyushiyangtech.top

[C03] 可变参数
来源：http://xnn.zhijiandao.cn

Py:   def total(*args): return sum(args)
来源：http://hmm.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pyf.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dmm.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ibn.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jum.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pnk.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://evo.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oyi.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://nmq.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ltl.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bwa.gaohongyu789.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://shv.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jfk.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://nlz.sxryk.cn

Go:   // 无：用配置结构体参数
来源：http://mzq.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://xko.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://zog.daxiang520.top

[C05] 返回多个值
来源：http://xii.hammf.cn

Py:   return a, b
来源：http://ric.cashguo.top

PHP:  return [$a, $b];
来源：http://dys.shanyushiyangtech.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mpz.guowangkeji.top

TS:   return { a, b };
来源：http://vdl.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lbh.vqdsnc.cn

Go:   return a, b
来源：http://yer.yuanzhike.top

Ruby: return a, b
来源：http://cey.chenjidiqi.icu

C#:   return (a, b);              // ValueTuple
来源：http://esw.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://jss.ctjpmb.com

Py:   square = lambda x: x * x
来源：http://gho.iojbl.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eyc.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://zny.yj202588.top

TS:   const square = (x: number): number => x * x;
来源：http://nfs.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://six.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://fge.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://hea.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://udk.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://irs.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ran.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://pma.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kwp.jinghuilouyu.cn

TS:   arr.map(String)
来源：http://ptp.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fji.sxryk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://exl.jiagoushi.top

Ruby: arr.map(&:upcase)
来源：http://fsl.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://trl.pycfn.com

[C08] 闭包
来源：http://fex.chenjidiqi.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qno.guannengcc.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ypa.sysykeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rzl.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zlk.52xcode.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rxf.cqqwz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mnz.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cdb.fengsongda.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gtx.jlsjyb.cn

[C09] 递归
来源：http://dwm.yj20258.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wqx.jlsjyb.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://osf.xuanzx.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zkv.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wgr.aibaodan.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xgl.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://phk.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kau.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://axs.wangshuangyany.cn

[C10] 变量作用域
来源：http://lob.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://plz.nwbrower.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aft.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qif.ctjpmb.com

TS:   同 JS
来源：http://aet.bjfxy.top

Java: 方法内为块级作用域
来源：http://quk.haohaochexian.top

Go:   花括号块级作用域
来源：http://bmn.shanyushiyangtech.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bsk.9152youxi.cn

C#:   块级作用域
来源：http://jmq.cheryme.top

[C11] 模块导入与导出
来源：http://tdk.iojbl.cn

Py:   from module import func
来源：http://hep.wangshuangyany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wvn.hongshengwenyu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ace.fzhhl.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://duu.hywenlv.cn

Java: import java.util.List;
来源：http://igl.chenjidiqi.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vlm.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://xci.gzhubu.top

C#:   using System.Text;
来源：http://zxk.aizwys.cn

[C12] 立即执行函数 IIFE
来源：http://ffd.bbcook.cn

Py:   (lambda: print("run"))()
来源：http://etz.wangdashe.top

PHP:  (function () { echo "run"; })();
来源：http://pik.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://ioc.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://wkc.ybcxt.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nab.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://frk.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://vki.redwolf501.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bzb.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://xkv.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xvt.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mhy.cqqwz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cyq.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cfo.zdqjudy.top

Java: int add(int a, int b) { return a + b; }
来源：http://xao.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://oju.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dww.jinqigfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://bof.jqgufenzy.top

[C14] 泛型函数
来源：http://opv.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ffx.bjfxy.top

PHP:  // 无泛型
来源：http://bdp.yonumen.top

JS:   // 无泛型
来源：http://mff.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vin.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ccc.ppjwa.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fex.yfazqb.com

Ruby: # 无泛型
来源：http://eum.jyoumei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mrg.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://bjp.yvedp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zub.ydjk.org.cn

PHP:  [$a, $b] = $pair;
来源：http://ydb.yuxming.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xik.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://set.fengsongda.top

Java: // 无解构
来源：http://thj.haohaochexian.top

Go:   // 无解构
来源：http://mwk.zhengqikj.top

Ruby: a, b = pair
来源：http://xvr.hnxiangtu.top

C#:   var (a, b) = pair;
来源：http://ntk.cucudq.cn

[C16] 函数 / 方法重载
来源：http://aeq.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dvw.chenjidiqi.icu

PHP:  // 无重载
来源：http://hme.shangyingyoupin.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ubb.cashguo.top

TS:   // 用联合类型或重载签名声明
来源：http://tsh.ivvv.top

Java: void f(int a) {}  void f(String a) {}
来源：http://eia.nwbrower.top

Go:   // 无重载：用不同函数名
来源：http://jbi.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://kfg.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gks.hysaishi.cn

================================================================================
来源：http://xxu.ydjk.org.cn

D. 数组 / 列表 / 集合
来源：http://jmx.zdbjq.cn

================================================================================
来源：http://wjl.shzxlz.cn

[D01] 创建数组 / 列表
来源：http://bxp.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mgg.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://olf.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dho.hammf.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xdy.jianghu66.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bvt.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://uyo.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://geq.yanxiufei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gtw.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://pjd.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://twb.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://omr.xuetiantiany.cn

JS:   arr.push(4);
来源：http://xlc.uphjek.com

TS:   arr.push(4);
来源：http://ure.cdnleiting.top

Java: list.add(4);
来源：http://kje.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://mbj.hysaishi.cn

Ruby: arr << 4; arr.push(5)
来源：http://sly.xinyue.icu

C#:   list.Add(4);
来源：http://ksc.tarul.cn

[D03] 在指定位置插入元素
来源：http://niz.uphjek.com

Py:   arr.insert(0, 0)
来源：http://vmx.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fis.jiagoushi.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tvx.jianghu66.top

TS:   arr.splice(0, 0, 0);
来源：http://pof.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://lil.zycfv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yox.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://chn.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://jep.0kj1m.cn

[D04] 删除元素
来源：http://ygc.wangshuangyany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nhv.bjfxy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vzi.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://svp.shangyingyoupin.top

TS:   arr.splice(0, 1);
来源：http://hll.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jdy.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kpo.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jbc.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vuz.jianghu66.top

[D05] 访问与修改元素
来源：http://jkc.yfazqb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qsp.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bxb.jinqigufen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cnp.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://hpu.epnwcf.com

Java: list.get(0); list.set(0, 9);
来源：http://gsp.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://iib.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kme.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rmn.jqgufenzy.top

[D06] 数组长度
来源：http://niy.epnwcf.com

Py:   len(arr)
来源：http://bpr.fanxiaobao.xyz

PHP:  count($arr);
来源：http://imh.52xcode.cn

JS:   arr.length
来源：http://tyr.fktsv.cn

TS:   arr.length
来源：http://hru.jyoumei.cn

Java: list.size();
来源：http://mwl.birdmap.top

Go:   len(arr)
来源：http://kxq.gzhubu.top

Ruby: arr.length; arr.size
来源：http://yso.hesvh.cn

C#:   list.Count;
来源：http://ahw.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://dlo.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wkd.gogol.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pzi.iojbl.cn

JS:   arr.slice(1, 4);
来源：http://pne.yueranfly.top

TS:   arr.slice(1, 4);
来源：http://jgp.zhixingplan.top

Java: list.subList(1, 4);
来源：http://spz.52xcode.cn

Go:   arr[1:4]
来源：http://ecg.pycfn.com

Ruby: arr[1, 3]
来源：http://wff.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://tsw.shuidangran.top

[D08] 合并两个数组
来源：http://nih.xingfuxueyuan.xyz

Py:   a + b;  a.extend(b)
来源：http://bvx.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://lve.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nef.feifeiyinyue.top

TS:   [...a, ...b];
来源：http://drp.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kqj.guowangkeji.top

Go:   append(a, b...)
来源：http://xkh.yanxiufei.cn

Ruby: a + b;  a.concat(b)
来源：http://xht.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://zun.hysaishi.cn

[D09] 排序（升序）
来源：http://vgi.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://bgd.xinyue.icu

PHP:  sort($arr);
来源：http://uct.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zdc.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://qvx.tanke756.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fui.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vcj.hammf.cn

Ruby: arr.sort
来源：http://zco.shanyushiyangkeji.top

C#:   list.Sort();
来源：http://kst.sweek.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xoj.nanxinkj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fni.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xgg.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wbg.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zxm.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ykc.kuanghao11.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://psd.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qfl.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://egz.cdnleiting.top

[D11] 反转数组
来源：http://sch.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://gcb.haohaochexian.top

PHP:  array_reverse($arr);
来源：http://fqo.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sen.sysykeji.top

TS:   [...arr].reverse();
来源：http://pru.meibo888.top

Java: Collections.reverse(list);
来源：http://efz.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://xpx.wangdashe.top

Ruby: arr.reverse
来源：http://yad.316326.xyz

C#:   list.Reverse();
来源：http://urm.nwbrower.top

[D12] 查找元素下标
来源：http://yxr.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://xjm.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qks.nanxuanxn.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://flm.guannengcc.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ted.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xur.jqgfzy.top

Go:   slices.Index(arr, x)
来源：http://nss.zhiwuduotai.top

Ruby: arr.index(x)
来源：http://fph.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://rje.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://pzy.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pkf.chenlongwang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hoe.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://frp.kuanghao11.cn

TS:   arr.filter(x => x > 3)
来源：http://nys.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://umm.havefunace.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pan.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vuz.smart0.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://kdc.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://bst.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vcs.yanxiufei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ljx.hammf.cn

JS:   arr.map(x => x * 2)
来源：http://hap.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://pmd.fktsv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tcz.yvedp.cn

Go:   // 手写循环
来源：http://fnl.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gnx.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cpz.ivvv.top

[D15] 去重
来源：http://lgz.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dif.ivvv.top

PHP:  array_unique($arr);
来源：http://ljm.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://mwr.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://fxs.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zxs.guannengcc.top

Go:   // 用 map[T]struct{} 手写
来源：http://red.guowangkeji.top

Ruby: arr.uniq
来源：http://wcx.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://ecb.tian-w.cn

[D16] 求和与平均值
来源：http://wii.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fod.bbcook.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://roj.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gfn.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sgz.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://smz.xuanzx.com

Go:   // 手写循环累加
来源：http://mou.andypj.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rqk.jqgufenzy.top

C#:   list.Sum();  list.Average()
来源：http://dyj.yj20258888.top

[D17] 最大值与最小值
来源：http://rpx.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://nuw.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://qpj.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://png.sysykeji.top

TS:   Math.max(...arr);
来源：http://zmc.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://kju.yj20258888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://okg.sxryk.cn

Ruby: arr.max;  arr.min
来源：http://jbq.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://rof.ivvv.top

[D18] 扁平化嵌套数组
来源：http://yxt.shangyingyoupin.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vhj.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://kjn.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jif.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://ept.yuanzhike.top


<!-- 参考信息 -->