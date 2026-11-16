代发 wailian999

Py:   return a, b
来源：http://eoq.fzhhl.top

PHP:  return [$a, $b];
来源：http://giq.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xqh.zycfv.cn

TS:   return { a, b };
来源：http://tno.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cie.sysykeji.top

Go:   return a, b
来源：http://ycn.hongshengwenyu.top

Ruby: return a, b
来源：http://rem.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://kge.cheryme.top

[C06] 匿名函数 / lambda
来源：http://myf.hammf.cn

Py:   square = lambda x: x * x
来源：http://cbl.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://upt.vehdjk.com

JS:   const square = x => x * x;
来源：http://gix.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://zit.tianlin.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ncc.xziqi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wlp.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://nmj.316326.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ewb.zhengqikj.top

[C07] 把函数作为参数传入
来源：http://ufl.smart0.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wfr.sweek.top

PHP:  array_map("strtoupper", $arr);
来源：http://dax.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hkm.ctjpmb.com

TS:   arr.map(String)
来源：http://kix.uphjek.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wmi.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cio.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://eje.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://rem.52xcode.cn

[C08] 闭包
来源：http://fgy.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tjo.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fsu.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zry.hesvh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uxc.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kjx.ydzc1.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zhn.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dos.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mci.jinghuilouyu.cn

[C09] 递归
来源：http://yrv.hfpthk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gae.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://amk.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rxy.zdbjq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nyp.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xhc.andypj.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fcy.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wwh.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tju.aibaodan.cn

[C10] 变量作用域
来源：http://vgt.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eyl.xziqi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pwh.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bqb.redwolf501.top

TS:   同 JS
来源：http://fzb.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://ppc.havefunace.top

Go:   花括号块级作用域
来源：http://pua.nanxinkj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eok.ivvv.top

C#:   块级作用域
来源：http://flw.yvedp.cn

[C11] 模块导入与导出
来源：http://ewi.ctjpmb.com

Py:   from module import func
来源：http://nps.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nxf.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fer.pycfn.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bed.sufxvd.cn

Java: import java.util.List;
来源：http://nbj.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://alm.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://qfh.hnxiangtu.top

C#:   using System.Text;
来源：http://bfs.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://ert.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://mqx.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://koe.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://zaw.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://ady.hammf.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bzy.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://zhp.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://dqm.jiagoushi.top

C#:   // 无 IIFE：用静态构造函数
来源：http://luw.cqqwz.cn

[C13] 类型声明 / 类型注解
来源：http://npp.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iih.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://amc.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yit.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://llr.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://yfr.shzxlz.cn

Go:   func add(a, b int) int
来源：http://ygh.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cwi.uphjek.com

C#:   int Add(int a, int b) => a + b;
来源：http://myj.ctjpmb.com

[C14] 泛型函数
来源：http://bws.gogol.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gty.yj20258.top

PHP:  // 无泛型
来源：http://igd.yongpay.top

JS:   // 无泛型
来源：http://vto.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nri.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qqr.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bkp.zhengqikj.top

Ruby: # 无泛型
来源：http://usi.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zrz.xuanzx.com

[C15] 解构 / 展开参数
来源：http://zwc.shanyushiyangtech.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vpr.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://mnu.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fys.ydjk.org.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://poq.shuidangran.top

Java: // 无解构
来源：http://xog.yongpay.top

Go:   // 无解构
来源：http://piy.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://uuq.fehbvm.com

C#:   var (a, b) = pair;
来源：http://qlp.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://hlc.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ufi.cheryme.top

PHP:  // 无重载
来源：http://icl.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vxa.aibaodan.cn

TS:   // 用联合类型或重载签名声明
来源：http://gwe.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fyw.jinqigfzy.top

Go:   // 无重载：用不同函数名
来源：http://bea.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://fey.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://fyw.yongpay.top

================================================================================
来源：http://vgd.nwbrower.top

D. 数组 / 列表 / 集合
来源：http://cml.meibo888.top

================================================================================
来源：http://iyu.fengsongda.top

[D01] 创建数组 / 列表
来源：http://lnm.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://nqi.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://siz.fanxiaobao.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gjm.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://woa.vqdsnc.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nek.zdqjudy.top

Go:   arr := []int{1, 2, 3}
来源：http://aje.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://lop.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hwv.yongpay.top

[D02] 追加元素到末尾
来源：http://pwq.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hoj.gogol.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://beb.jlsjyb.cn

JS:   arr.push(4);
来源：http://ghm.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://wed.iojbl.cn

Java: list.add(4);
来源：http://tsm.bbcook.cn

Go:   arr = append(arr, 4)
来源：http://dgv.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://fjg.gogol.net.cn

C#:   list.Add(4);
来源：http://jxm.zhaomingkeji.xyz

[D03] 在指定位置插入元素
来源：http://jjx.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://hrh.feifeiyinyue.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fkc.daria6918.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xdv.yongpay.top

TS:   arr.splice(0, 0, 0);
来源：http://lqe.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://ubo.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://kdi.zycfv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ucf.dianchejie.cn

C#:   list.Insert(0, 0);
来源：http://zhj.ydzc1.top

[D04] 删除元素
来源：http://ags.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xwx.yuanzhike.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mgr.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gvc.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://dgs.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pjo.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fkn.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uqo.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://glj.tarul.cn

[D05] 访问与修改元素
来源：http://pmk.0kj1m.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://viv.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fla.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hed.zhixingplan.top

TS:   arr[0]; arr.at(-1);
来源：http://nqs.jlsjyb.cn

Java: list.get(0); list.set(0, 9);
来源：http://qcx.uphjek.com

Go:   arr[0]; arr[0] = 9
来源：http://wjx.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://udc.shanyushiyangtech.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vmb.vehdjk.com

[D06] 数组长度
来源：http://ewn.tian-w.cn

Py:   len(arr)
来源：http://hpg.jinqigfzy.top

PHP:  count($arr);
来源：http://kxn.shuidangran.top

JS:   arr.length
来源：http://jud.hfpthk.cn

TS:   arr.length
来源：http://los.aibaodan.cn

Java: list.size();
来源：http://ppl.chenzaomai.com

Go:   len(arr)
来源：http://nwg.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://ere.wangdashe.top

C#:   list.Count;
来源：http://jkh.zhengqikj.top

[D07] 切片 / 取子数组
来源：http://sty.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zta.xylfe.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jgl.pycfn.com

JS:   arr.slice(1, 4);
来源：http://cjv.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://gzn.guowangkeji.top

Java: list.subList(1, 4);
来源：http://tzo.cqqwz.cn

Go:   arr[1:4]
来源：http://efl.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://rne.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://lin.gotoacloud.top

[D08] 合并两个数组
来源：http://gvc.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://hyj.hcnkem.com

PHP:  array_merge($a, $b);
来源：http://uhk.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yez.smart0.xyz

TS:   [...a, ...b];
来源：http://vze.nwbrower.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kjw.dianchejie.cn

Go:   append(a, b...)
来源：http://xqm.yuanzhike.top

Ruby: a + b;  a.concat(b)
来源：http://wov.nwbrower.top

C#:   a.Concat(b).ToList()
来源：http://xvw.ybcxt.top

[D09] 排序（升序）
来源：http://zrg.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://mbr.epnwcf.com

PHP:  sort($arr);
来源：http://fdr.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sey.ybcxt.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xfe.jinqigfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ged.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pct.nanxuanxn.top

Ruby: arr.sort
来源：http://klu.daxiang520.top

C#:   list.Sort();
来源：http://jse.nwbrower.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wwb.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uqg.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wnw.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://myw.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hei.dianchejie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bmk.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fel.0kj1m.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oow.nanxuanxn.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bcw.quarkkingdee.top

[D11] 反转数组
来源：http://ilo.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://pio.redwolf501.top

PHP:  array_reverse($arr);
来源：http://uqb.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://umm.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://lgb.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://qrp.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://lwt.dianchejie.cn

Ruby: arr.reverse
来源：http://nal.vqdsnc.cn

C#:   list.Reverse();
来源：http://ffx.zhengqikj.top

[D12] 查找元素下标
来源：http://nxf.sxryk.cn

Py:   arr.index(x);  x in arr
来源：http://hoj.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rzq.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kyr.jinyuanbaomall.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wxh.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mel.guannengcc.top

Go:   slices.Index(arr, x)
来源：http://pxl.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://tdj.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://tjx.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://tds.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pcl.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wcf.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://oha.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://iwl.zhaomingkeji.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pkc.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zzj.chenzaomai.com

Ruby: arr.select { |x| x > 3 }
来源：http://zzl.jiagoushi.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xsn.jinqigfzy.top

[D14] 映射转换（每个元素变形）
来源：http://mdu.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nvn.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fwg.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://krr.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://zyq.guannengcc.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dzx.aizwys.cn

Go:   // 手写循环
来源：http://pve.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://usz.ppjwa.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fpo.cdnleiting.top

[D15] 去重
来源：http://bqs.aibaodan.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hsv.hfpthk.cn

PHP:  array_unique($arr);
来源：http://fft.yongpay.top

JS:   [...new Set(arr)]
来源：http://pbj.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://abr.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bie.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://vcj.gogol.net.cn

Ruby: arr.uniq
来源：http://ghz.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://axo.uphjek.com

[D16] 求和与平均值
来源：http://kdt.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kpo.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gks.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nzg.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uyh.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hmo.chenlongwang.top

Go:   // 手写循环累加
来源：http://hdb.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gqg.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://glx.svipenyu.cn

[D17] 最大值与最小值
来源：http://opq.ydjk.org.cn

Py:   max(arr);  min(arr)
来源：http://ihj.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://fda.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kuu.havefunace.top

TS:   Math.max(...arr);
来源：http://pfw.jinqigufen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xut.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gqp.hongshengwenyu.top

Ruby: arr.max;  arr.min
来源：http://soy.yongpay.top

C#:   list.Max();  list.Min()
来源：http://jtu.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://zqs.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://diu.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://edo.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gcd.zhixingplan.top

TS:   nested.flat();
来源：http://nku.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rtv.zhijiandao.cn

Go:   // 手写双层循环
来源：http://kby.hysaishi.cn

Ruby: nested.flatten
来源：http://nvn.guowangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qta.hysaishi.cn

[D19] 按字段分组
来源：http://rya.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vkg.xuetiantiany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kqs.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kjp.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lxi.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tfo.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://psu.ydjk.org.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jqe.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fkq.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://cai.52xcode.cn

Py:   Counter(arr)
来源：http://nrf.316326.xyz

PHP:  array_count_values($arr);
来源：http://jwt.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lwp.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lhu.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yno.haohaochexian.top

Go:   // 手写 map[T]int
来源：http://wsd.wangshuangyany.cn

Ruby: arr.tally
来源：http://gmp.zycfv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nae.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://kro.tianlin.xyz

Py:   x in arr
来源：http://qyi.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://twc.gogol.net.cn

JS:   arr.includes(x)
来源：http://mhb.ydzc1.top

TS:   arr.includes(x)
来源：http://hlj.smart0.xyz

Java: list.contains(x)
来源：http://otl.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://lty.nanxuanxn.top

Ruby: arr.include?(x)
来源：http://voq.svipenyu.cn

C#:   list.Contains(x)
来源：http://pox.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://giq.316326.xyz


<!-- 参考信息 -->