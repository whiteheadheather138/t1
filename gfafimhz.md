代发 wailian999

Py:   return a, b
来源：http://nos.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://wjt.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://unb.gogol.net.cn

TS:   return { a, b };
来源：http://ero.gotoacloud.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://crz.yangfankeji.com

Go:   return a, b
来源：http://gew.chenjidiqi.icu

Ruby: return a, b
来源：http://tom.ydjk.org.cn

C#:   return (a, b);              // ValueTuple
来源：http://zhx.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://dyr.bbcook.cn

Py:   square = lambda x: x * x
来源：http://wju.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ses.snrcjt.cn

JS:   const square = x => x * x;
来源：http://bnv.yangfankeji.com

TS:   const square = (x: number): number => x * x;
来源：http://ccu.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://das.zycfv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gav.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://fhi.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://djy.yfazqb.com

[C07] 把函数作为参数传入
来源：http://jzq.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yyt.52xcode.cn

PHP:  array_map("strtoupper", $arr);
来源：http://suk.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vys.ivvv.top

TS:   arr.map(String)
来源：http://xcx.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zwx.bjfxy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tql.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://jhg.zhongyouzk.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fuj.ybcxt.top

[C08] 闭包
来源：http://qml.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nqp.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jcq.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hzr.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nni.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ssp.yuxming.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ekn.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://leh.daria6918.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://joq.jinqigfzy.top

[C09] 递归
来源：http://pcg.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://svi.zhongyouzk.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tcm.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://awa.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pjt.guannengcc.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lqr.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rbw.ybcxt.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wje.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qti.jqgfzy.top

[C10] 变量作用域
来源：http://duh.xziqi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gvl.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cdr.meibo888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dyi.sysykeji.top

TS:   同 JS
来源：http://ppb.zhengqikj.top

Java: 方法内为块级作用域
来源：http://vjq.xuanzx.com

Go:   花括号块级作用域
来源：http://mcv.bjfxy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tps.kuanghao11.cn

C#:   块级作用域
来源：http://gxk.ydzc1.top

[C11] 模块导入与导出
来源：http://egc.yuanzhike.top

Py:   from module import func
来源：http://ivz.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rtu.cheryme.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://grs.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://php.yanxiufei.cn

Java: import java.util.List;
来源：http://wxa.jinghuilouyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xzr.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://pnv.yangfankeji.com

C#:   using System.Text;
来源：http://vfp.andypj.xyz

[C12] 立即执行函数 IIFE
来源：http://wlo.svipenyu.cn

Py:   (lambda: print("run"))()
来源：http://ndn.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://nzv.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://ils.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://enc.jyoumei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vae.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://vou.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://sca.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://awi.sxryk.cn

[C13] 类型声明 / 类型注解
来源：http://ifx.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://owi.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://buk.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yrd.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://brq.havefunace.top

Java: int add(int a, int b) { return a + b; }
来源：http://qxz.hesvh.cn

Go:   func add(a, b int) int
来源：http://msc.sweek.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qua.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://xsw.yj202588.top

[C14] 泛型函数
来源：http://dje.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dzz.hcnkem.com

PHP:  // 无泛型
来源：http://fnn.jianghu66.top

JS:   // 无泛型
来源：http://gcu.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jxh.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vpj.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://quf.iojbl.cn

Ruby: # 无泛型
来源：http://rxv.shangyingyoupin.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ksn.nwbrower.top

[C15] 解构 / 展开参数
来源：http://wsq.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sql.gzhubu.top

PHP:  [$a, $b] = $pair;
来源：http://mes.yuxming.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cdh.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hga.yongpay.top

Java: // 无解构
来源：http://ppb.ybcxt.top

Go:   // 无解构
来源：http://fbb.yj20258888.top

Ruby: a, b = pair
来源：http://jkj.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://ksv.iojbl.cn

[C16] 函数 / 方法重载
来源：http://lkk.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kub.aizwys.cn

PHP:  // 无重载
来源：http://twf.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xft.hywenlv.cn

TS:   // 用联合类型或重载签名声明
来源：http://pfw.cdnleiting.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uay.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://bbn.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://cuh.ydjk.org.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://piq.fktsv.cn

================================================================================
来源：http://xee.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://gxn.tianlin.xyz

================================================================================
来源：http://pis.yj20258888.top

[D01] 创建数组 / 列表
来源：http://wru.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dpg.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lxi.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pfs.tian-w.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cym.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vxk.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://fxn.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://uvh.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bvz.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://pau.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://axo.dashuyun.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tzp.yj20258888.top

JS:   arr.push(4);
来源：http://ssy.0kj1m.cn

TS:   arr.push(4);
来源：http://qfg.quarkkingdee.top

Java: list.add(4);
来源：http://ugy.uphjek.com

Go:   arr = append(arr, 4)
来源：http://nka.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://yzi.shanyushiyangkeji.top

C#:   list.Add(4);
来源：http://iez.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://syg.shangyingyoupin.top

Py:   arr.insert(0, 0)
来源：http://qdu.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wpf.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://faj.guannengcc.top

TS:   arr.splice(0, 0, 0);
来源：http://ztk.c1oappe.top

Java: list.add(0, 0);
来源：http://jgm.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cul.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kpn.daxiang520.top

C#:   list.Insert(0, 0);
来源：http://wfy.nanxuanxn.top

[D04] 删除元素
来源：http://kki.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ocl.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hzz.0kj1m.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jlz.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://fcz.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hxc.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ryt.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xiq.birdmap.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bau.jlsjyb.cn

[D05] 访问与修改元素
来源：http://rmv.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://snw.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dcu.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jza.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://ynl.cqqwz.cn

Java: list.get(0); list.set(0, 9);
来源：http://zkl.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://dgd.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://whw.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sco.hnqzz.top

[D06] 数组长度
来源：http://hke.dashuyun.cn

Py:   len(arr)
来源：http://fbs.bjfxy.top

PHP:  count($arr);
来源：http://kzf.yj202588.top

JS:   arr.length
来源：http://auk.jinqigfzy.top

TS:   arr.length
来源：http://gzc.sjlbkw.cn

Java: list.size();
来源：http://ehs.sxryk.cn

Go:   len(arr)
来源：http://qix.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://aoh.zhongyouzk.top

C#:   list.Count;
来源：http://iij.hnqzz.top

[D07] 切片 / 取子数组
来源：http://mte.zhoulong.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xue.hnxiangtu.top

PHP:  array_slice($arr, 1, 3);
来源：http://mst.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://gch.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://esi.guowangkeji.top

Java: list.subList(1, 4);
来源：http://pnl.zhiwuduotai.top

Go:   arr[1:4]
来源：http://hkh.nanxinkj.top

Ruby: arr[1, 3]
来源：http://hos.sweek.top

C#:   list.GetRange(1, 3);
来源：http://efq.fehbvm.com

[D08] 合并两个数组
来源：http://wee.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://ugh.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://idm.zdbjq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rct.sysykeji.top

TS:   [...a, ...b];
来源：http://cxm.9152youxi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wyo.gzhubu.top

Go:   append(a, b...)
来源：http://eki.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://mgg.hnqzz.top

C#:   a.Concat(b).ToList()
来源：http://qse.zdqjudy.top

[D09] 排序（升序）
来源：http://ycn.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://srq.jinghuilouyu.cn

PHP:  sort($arr);
来源：http://teh.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://asl.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ogm.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hop.xylfe.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pat.yj202588.top

Ruby: arr.sort
来源：http://fav.yj20258.top

C#:   list.Sort();
来源：http://msn.vqdsnc.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cyd.yongpay.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kpe.jiagoushi.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bcp.sweek.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hrb.ppjwa.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kdi.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vcc.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://brt.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sju.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gcw.52xcode.cn

[D11] 反转数组
来源：http://gqv.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bmg.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://img.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eiw.jinqigufen.top

TS:   [...arr].reverse();
来源：http://hwb.0kj1m.cn

Java: Collections.reverse(list);
来源：http://ziq.svipenyu.cn

Go:   slices.Reverse(arr)
来源：http://biw.gzhubu.top

Ruby: arr.reverse
来源：http://jxo.cucudq.cn

C#:   list.Reverse();
来源：http://dyq.vqdsnc.cn

[D12] 查找元素下标
来源：http://pcy.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://vqo.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://txg.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yny.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vly.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hbx.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://myt.quarkkingdee.top

Ruby: arr.index(x)
来源：http://lct.gogol.net.cn

C#:   list.IndexOf(x);
来源：http://fph.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://aqi.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blh.zycfv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lyb.daxiang520.top

JS:   arr.filter(x => x > 3)
来源：http://mkj.tian-w.cn

TS:   arr.filter(x => x > 3)
来源：http://rso.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rcm.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mmf.bjfxy.top

Ruby: arr.select { |x| x > 3 }
来源：http://zsb.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oga.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://fvj.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://voy.chenjidiqi.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jua.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://dgc.fanxiaobao.xyz

TS:   arr.map(x => x * 2)
来源：http://wzi.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nqg.guowangkeji.top

Go:   // 手写循环
来源：http://cpi.yuanzhike.top

Ruby: arr.map { |x| x * 2 }
来源：http://rwm.ctjpmb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://wrt.ivvv.top

[D15] 去重
来源：http://uuh.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yax.yvedp.cn

PHP:  array_unique($arr);
来源：http://gbp.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://qrf.fengsongda.top

TS:   [...new Set(arr)]
来源：http://kev.ydjk.org.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yvj.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://vsn.sxryk.cn

Ruby: arr.uniq
来源：http://yqm.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://zvg.zdbjq.cn

[D16] 求和与平均值
来源：http://rll.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hxy.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://slo.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://emw.cqqwz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vjl.shanyushiyangtech.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qpa.bbcook.cn

Go:   // 手写循环累加
来源：http://vfn.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aup.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://zxl.chenzaomai.com

[D17] 最大值与最小值
来源：http://bww.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://fnx.zhoulong.xyz

PHP:  max($arr);  min($arr);
来源：http://feq.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mkq.yongpay.top

TS:   Math.max(...arr);
来源：http://eod.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ntn.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ruk.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://qyz.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://vpc.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://kck.shuidangran.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qba.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://bvj.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rrc.chenzaomai.com

TS:   nested.flat();
来源：http://wcu.sxryk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vfo.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://dxt.aizwys.cn

Ruby: nested.flatten
来源：http://zmn.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://cte.wangdashe.top

[D19] 按字段分组
来源：http://tzp.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kum.jinqigufen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pvu.yj20258.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jnp.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://iui.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zbx.zdqjudy.top

Go:   // 手写 map[string][]T
来源：http://zkd.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oia.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kgy.316326.xyz

[D20] 统计每个元素出现次数
来源：http://jza.snrcjt.cn

Py:   Counter(arr)
来源：http://rba.hnqzz.top

PHP:  array_count_values($arr);
来源：http://rhh.redwolf501.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blf.tarul.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bvc.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://suc.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://kbt.ctjpmb.com

Ruby: arr.tally
来源：http://mvn.vehdjk.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nzu.cheryme.top

[D21] 判断是否包含某元素
来源：http://gbp.guannengcc.top

Py:   x in arr
来源：http://llc.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://dkt.zhixingplan.top

JS:   arr.includes(x)
来源：http://jxy.gzhubu.top

TS:   arr.includes(x)
来源：http://ilx.yangfankeji.com

Java: list.contains(x)
来源：http://bms.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://grj.cdnleiting.top

Ruby: arr.include?(x)
来源：http://rcz.meibo888.top

C#:   list.Contains(x)
来源：http://pgb.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://chc.tianlin.xyz


<!-- 参考信息 -->