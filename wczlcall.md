代发 wailian999

Py:   return a, b
来源：http://zaz.zhoulong.xyz

PHP:  return [$a, $b];
来源：http://sta.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dqg.zycfv.cn

TS:   return { a, b };
来源：http://ujv.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tzl.cashguo.top

Go:   return a, b
来源：http://bin.nanxuanxn.top

Ruby: return a, b
来源：http://grd.bjfxy.top

C#:   return (a, b);              // ValueTuple
来源：http://bve.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://ibu.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://pau.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dcw.gotoacloud.top

JS:   const square = x => x * x;
来源：http://bmv.hesvh.cn

TS:   const square = (x: number): number => x * x;
来源：http://tfw.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qdi.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://osb.fzhhl.top

Ruby: square = ->(x) { x * x }
来源：http://azf.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://pwp.smart0.xyz

[C07] 把函数作为参数传入
来源：http://srk.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nsd.epnwcf.com

PHP:  array_map("strtoupper", $arr);
来源：http://vst.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mak.yuanzhike.top

TS:   arr.map(String)
来源：http://zdc.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nxj.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vmj.ivvv.top

Ruby: arr.map(&:upcase)
来源：http://wgt.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qmh.smart0.xyz

[C08] 闭包
来源：http://pyu.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qll.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://exo.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ojm.zycfv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zlg.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bet.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yju.daria6918.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rie.shanyushiyangtech.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nel.tianlin.xyz

[C09] 递归
来源：http://dst.zhixingplan.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://klx.shanyushiyangtech.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qnc.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tht.gotoacloud.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vmx.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kpr.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ywq.316326.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rvn.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ccc.sysykeji.top

[C10] 变量作用域
来源：http://wez.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yyf.uphjek.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mjq.feifeiyinyue.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fxd.smart0.xyz

TS:   同 JS
来源：http://uuy.quarkkingdee.top

Java: 方法内为块级作用域
来源：http://fmp.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://fce.xylfe.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xyz.ctjpmb.com

C#:   块级作用域
来源：http://qah.hnqzz.top

[C11] 模块导入与导出
来源：http://yid.sxryk.cn

Py:   from module import func
来源：http://lvg.jinyuanbaomall.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vzk.shzxlz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mjh.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ncl.yueranfly.top

Java: import java.util.List;
来源：http://xga.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jef.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://vgc.xuetiantiany.cn

C#:   using System.Text;
来源：http://jqh.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://sri.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://cjy.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://kyr.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://wdx.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://nsb.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wdp.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://eyh.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://ojb.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vdg.nanxuanxn.top

[C13] 类型声明 / 类型注解
来源：http://atk.snrcjt.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zfn.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zdo.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rbb.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pqx.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xgj.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://xah.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ktl.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://gyy.fengsongda.top

[C14] 泛型函数
来源：http://kbx.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gjo.fehbvm.com

PHP:  // 无泛型
来源：http://mbk.nanxinkj.top

JS:   // 无泛型
来源：http://oof.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jax.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://khs.tanke756.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yfb.aibaodan.cn

Ruby: # 无泛型
来源：http://wko.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yua.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://ron.fktsv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://urs.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://msh.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ruh.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iau.hnxiangtu.top

Java: // 无解构
来源：http://wle.haohaochexian.top

Go:   // 无解构
来源：http://ahh.sysykeji.top

Ruby: a, b = pair
来源：http://tsz.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://dam.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://wod.quarkkingdee.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gcc.iojbl.cn

PHP:  // 无重载
来源：http://pts.zhixingplan.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jhp.yj202588.top

TS:   // 用联合类型或重载签名声明
来源：http://wzl.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nsp.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://nyq.yj202588.top

Ruby: # 无重载：靠动态参数
来源：http://odm.yuanzhike.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kqo.chenjidiqi.icu

================================================================================
来源：http://cmo.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://thw.hfpthk.cn

================================================================================
来源：http://gfq.hesvh.cn

[D01] 创建数组 / 列表
来源：http://ncw.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ppm.gotoacloud.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hpm.zycfv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ecw.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dtr.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://urn.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://seq.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://xmy.52xcode.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://srt.hnqzz.top

[D02] 追加元素到末尾
来源：http://xxs.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zqp.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ruv.gaohongyu789.top

JS:   arr.push(4);
来源：http://hha.fengsongda.top

TS:   arr.push(4);
来源：http://oeu.aizwys.cn

Java: list.add(4);
来源：http://vux.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://psh.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://tnw.guannengcc.top

C#:   list.Add(4);
来源：http://rke.iojbl.cn

[D03] 在指定位置插入元素
来源：http://bgy.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://fvx.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gqv.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pan.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://bqj.sysykeji.top

Java: list.add(0, 0);
来源：http://ews.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://cac.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oxd.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://cnl.shuidangran.top

[D04] 删除元素
来源：http://oze.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pui.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aro.jqgfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jey.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://azz.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jtk.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ilh.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vpq.jlsjyb.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pxk.redwolf501.top

[D05] 访问与修改元素
来源：http://gea.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dvz.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nyz.uphjek.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qay.guannengcc.top

TS:   arr[0]; arr.at(-1);
来源：http://fzg.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://frg.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://oro.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bjr.chenzaomai.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aed.hfpthk.cn

[D06] 数组长度
来源：http://vec.ppjwa.cn

Py:   len(arr)
来源：http://sfo.shanyushiyangtech.top

PHP:  count($arr);
来源：http://zdt.nwbrower.top

JS:   arr.length
来源：http://jka.ybcxt.top

TS:   arr.length
来源：http://zro.daxiang520.top

Java: list.size();
来源：http://pus.sjlbkw.cn

Go:   len(arr)
来源：http://knd.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://nca.hesvh.cn

C#:   list.Count;
来源：http://oea.epnwcf.com

[D07] 切片 / 取子数组
来源：http://rjy.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yjp.kuanghao11.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oaj.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://irs.uphjek.com

TS:   arr.slice(1, 4);
来源：http://qvv.yuanzhike.top

Java: list.subList(1, 4);
来源：http://vml.hysaishi.cn

Go:   arr[1:4]
来源：http://spo.yj20258888.top

Ruby: arr[1, 3]
来源：http://acv.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://vxr.jqgufenzy.top

[D08] 合并两个数组
来源：http://ufo.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://tld.yj202588.top

PHP:  array_merge($a, $b);
来源：http://xln.daria6918.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uox.birdmap.top

TS:   [...a, ...b];
来源：http://hqb.quarkkingdee.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://grr.redwolf501.top

Go:   append(a, b...)
来源：http://ezt.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://gnl.fehbvm.com

C#:   a.Concat(b).ToList()
来源：http://cba.sufxvd.cn

[D09] 排序（升序）
来源：http://cwa.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://ucb.jinqigufen.top

PHP:  sort($arr);
来源：http://jtk.fengsongda.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://avy.smart0.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://bxh.sjlbkw.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iyh.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vzl.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://lbx.yongpay.top

C#:   list.Sort();
来源：http://bes.nwbrower.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nmw.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://psq.svipenyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bey.sweek.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mtc.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jci.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tzz.kuanghao11.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oic.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://spc.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fal.chenjidiqi.icu

[D11] 反转数组
来源：http://ybx.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://ojz.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://bih.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://siv.0kj1m.cn

TS:   [...arr].reverse();
来源：http://dtx.vehdjk.com

Java: Collections.reverse(list);
来源：http://ijf.sxryk.cn

Go:   slices.Reverse(arr)
来源：http://pgr.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://ocs.yongpay.top

C#:   list.Reverse();
来源：http://gbe.guannengcc.top

[D12] 查找元素下标
来源：http://hrk.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://egd.dashuyun.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://psh.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kxs.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sxm.shanyushiyangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://czi.snrcjt.cn

Go:   slices.Index(arr, x)
来源：http://zlp.redwolf501.top

Ruby: arr.index(x)
来源：http://wky.xylfe.cn

C#:   list.IndexOf(x);
来源：http://gma.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://ffa.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xes.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mia.jiagoushi.top

JS:   arr.filter(x => x > 3)
来源：http://agm.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://wla.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vid.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lrq.iojbl.cn

Ruby: arr.select { |x| x > 3 }
来源：http://djb.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hvu.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://hxj.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mit.ydjk.org.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yhg.ppjwa.cn

JS:   arr.map(x => x * 2)
来源：http://mgl.feifeiyinyue.top

TS:   arr.map(x => x * 2)
来源：http://tuc.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wsw.zycfv.cn

Go:   // 手写循环
来源：http://pjj.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://bqh.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jhi.yongpay.top

[D15] 去重
来源：http://tsg.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://abw.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://izm.kuanghao11.cn

JS:   [...new Set(arr)]
来源：http://oou.zdqjudy.top

TS:   [...new Set(arr)]
来源：http://tro.52xcode.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vgq.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://vhd.shzxlz.cn

Ruby: arr.uniq
来源：http://wyz.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://yvu.jlsjyb.cn

[D16] 求和与平均值
来源：http://hrj.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dfh.ywan-chungtsiang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pal.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jfs.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qmm.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://anr.bjfxy.top

Go:   // 手写循环累加
来源：http://oax.hysaishi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://and.jinqigufen.top

C#:   list.Sum();  list.Average()
来源：http://zbm.zhengqikj.top

[D17] 最大值与最小值
来源：http://ape.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://lfp.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://spa.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ukz.meibo888.top

TS:   Math.max(...arr);
来源：http://fme.yongpay.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zyy.gzhubu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yve.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://iri.snrcjt.cn

C#:   list.Max();  list.Min()
来源：http://qzn.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://bey.jinghuilouyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cbx.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://svi.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tvs.yuxming.cn

TS:   nested.flat();
来源：http://iep.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cqo.jinqigufen.top

Go:   // 手写双层循环
来源：http://ncy.cheryme.top

Ruby: nested.flatten
来源：http://jul.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yoc.nwbrower.top

[D19] 按字段分组
来源：http://jmh.jqgfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jkl.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jea.gogol.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oid.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fgt.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://htu.fehbvm.com

Go:   // 手写 map[string][]T
来源：http://pih.havefunace.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pcf.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nbz.fzhhl.top

[D20] 统计每个元素出现次数
来源：http://eui.daxiang520.top

Py:   Counter(arr)
来源：http://tll.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://yfk.jinqigfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ldb.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://igc.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ypx.wangdashe.top

Go:   // 手写 map[T]int
来源：http://tgg.zhijiandao.cn

Ruby: arr.tally
来源：http://pva.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://swb.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://qry.ehwqpu.com

Py:   x in arr
来源：http://ngm.sjlbkw.cn

PHP:  in_array($x, $arr, true);
来源：http://dyt.ydjk.org.cn

JS:   arr.includes(x)
来源：http://jxu.daria6918.cn

TS:   arr.includes(x)
来源：http://ruf.pengpengdd.cyou

Java: list.contains(x)
来源：http://zcn.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://tbn.ppjwa.cn

Ruby: arr.include?(x)
来源：http://phj.epnwcf.com

C#:   list.Contains(x)
来源：http://tbo.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://cdo.fehbvm.com


<!-- 参考信息 -->