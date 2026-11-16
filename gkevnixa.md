代发 wailian999

Py:   return a, b
来源：http://gyl.fzhhl.top

PHP:  return [$a, $b];
来源：http://apu.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ctu.dianchejie.cn

TS:   return { a, b };
来源：http://mev.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qix.svipenyu.cn

Go:   return a, b
来源：http://qle.cashguo.top

Ruby: return a, b
来源：http://ike.dashuyun.cn

C#:   return (a, b);              // ValueTuple
来源：http://ndk.svipenyu.cn

[C06] 匿名函数 / lambda
来源：http://foq.xinyue.icu

Py:   square = lambda x: x * x
来源：http://kjg.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://cxv.pycfn.com

JS:   const square = x => x * x;
来源：http://tlx.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://hga.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://grt.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tic.zdbjq.cn

Ruby: square = ->(x) { x * x }
来源：http://clh.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://njz.pycfn.com

[C07] 把函数作为参数传入
来源：http://txc.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fmb.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://cce.c1oappe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nwx.uphjek.com

TS:   arr.map(String)
来源：http://rjt.snrcjt.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qkj.vqdsnc.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cvf.zdqjudy.top

Ruby: arr.map(&:upcase)
来源：http://prr.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tzz.svipenyu.cn

[C08] 闭包
来源：http://bcd.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hjh.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://shs.cqqwz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dkr.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ogb.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ieg.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ejt.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://geu.tian-w.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ebr.jinyuanbaomall.cn

[C09] 递归
来源：http://bsk.ppjwa.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rvr.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gkd.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hpx.zdbjq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hoi.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pir.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://inl.jqgfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wwq.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rjj.nwbrower.top

[C10] 变量作用域
来源：http://ner.uphjek.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bfw.chenlongwang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nfa.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vqf.bjfxy.top

TS:   同 JS
来源：http://blz.jianghu66.top

Java: 方法内为块级作用域
来源：http://qtv.jinqigufen.top

Go:   花括号块级作用域
来源：http://zxx.nanxinkj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iij.ydjk.org.cn

C#:   块级作用域
来源：http://mxn.xziqi.cn

[C11] 模块导入与导出
来源：http://sry.316326.xyz

Py:   from module import func
来源：http://vhf.hysaishi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://svg.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zbb.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jzx.kuanghao11.cn

Java: import java.util.List;
来源：http://ynv.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://obc.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://mlm.dianchejie.cn

C#:   using System.Text;
来源：http://nxq.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://dfl.shzxlz.cn

Py:   (lambda: print("run"))()
来源：http://vql.xuetiantiany.cn

PHP:  (function () { echo "run"; })();
来源：http://jvs.fktsv.cn

JS:   (() => { console.log("run"); })();
来源：http://wtl.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://pkn.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://liy.ivvv.top

Go:   func() { fmt.Println("run") }()
来源：http://wcl.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://jje.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://rus.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://fji.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iol.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zze.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ice.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gef.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://zut.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://wch.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oxx.ybcxt.top

C#:   int Add(int a, int b) => a + b;
来源：http://vax.316326.xyz

[C14] 泛型函数
来源：http://ezy.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wcb.ctjpmb.com

PHP:  // 无泛型
来源：http://aiq.ctjpmb.com

JS:   // 无泛型
来源：http://ahc.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sun.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://imx.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jec.zdbjq.cn

Ruby: # 无泛型
来源：http://pae.aizwys.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sff.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://fmq.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cly.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://bzp.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fdy.ybcxt.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fhg.sjlbkw.cn

Java: // 无解构
来源：http://fxy.redwolf501.top

Go:   // 无解构
来源：http://dhv.shuidangran.top

Ruby: a, b = pair
来源：http://kwa.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://sex.hcnkem.com

[C16] 函数 / 方法重载
来源：http://eqv.xuetiantiany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://psh.pengpengdd.cyou

PHP:  // 无重载
来源：http://tlq.chenlongwang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qqn.ivvv.top

TS:   // 用联合类型或重载签名声明
来源：http://pkq.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mhf.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://lty.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://rgc.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mbw.zdqjudy.top

================================================================================
来源：http://glb.xuetiantiany.cn

D. 数组 / 列表 / 集合
来源：http://dmg.nanxuanxn.top

================================================================================
来源：http://uwp.ivvv.top

[D01] 创建数组 / 列表
来源：http://myd.shanyushiyangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rry.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fzt.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gfr.fehbvm.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://gnv.yanxiufei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fkn.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://eaf.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://rpt.chenlongwang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ttj.tianlin.xyz

[D02] 追加元素到末尾
来源：http://xwu.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://knu.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qjm.sxryk.cn

JS:   arr.push(4);
来源：http://mtt.hesvh.cn

TS:   arr.push(4);
来源：http://eya.pycfn.com

Java: list.add(4);
来源：http://ueb.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://ykc.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://qif.hesvh.cn

C#:   list.Add(4);
来源：http://nrj.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://ixw.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://qma.tian-w.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ucl.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://glr.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://nkj.pycfn.com

Java: list.add(0, 0);
来源：http://lik.jyoumei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aik.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ckx.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://yao.fktsv.cn

[D04] 删除元素
来源：http://cdk.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hdh.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ohw.bjfxy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tvb.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://tzz.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jma.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vag.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uqg.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qdv.yfazqb.com

[D05] 访问与修改元素
来源：http://aiq.hesvh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://arr.nwbrower.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fru.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nra.daria6918.cn

TS:   arr[0]; arr.at(-1);
来源：http://xwu.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://dgs.ydjk.org.cn

Go:   arr[0]; arr[0] = 9
来源：http://xxn.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yjt.snrcjt.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lou.yangfankeji.com

[D06] 数组长度
来源：http://pku.jinqigufen.top

Py:   len(arr)
来源：http://qvg.0kj1m.cn

PHP:  count($arr);
来源：http://hix.yj202588.top

JS:   arr.length
来源：http://wbb.zhiwuduotai.top

TS:   arr.length
来源：http://whc.ywan-chungtsiang.top

Java: list.size();
来源：http://jwk.sufxvd.cn

Go:   len(arr)
来源：http://kns.ydzc1.top

Ruby: arr.length; arr.size
来源：http://rba.zhoulong.xyz

C#:   list.Count;
来源：http://qaq.yongpay.top

[D07] 切片 / 取子数组
来源：http://tgb.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://duf.cheryme.top

PHP:  array_slice($arr, 1, 3);
来源：http://tro.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://pwh.yongpay.top

TS:   arr.slice(1, 4);
来源：http://ogq.zhoulong.xyz

Java: list.subList(1, 4);
来源：http://ibz.nanxinkj.top

Go:   arr[1:4]
来源：http://mmr.daria6918.cn

Ruby: arr[1, 3]
来源：http://xrb.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://twk.316326.xyz

[D08] 合并两个数组
来源：http://ukb.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://con.nanxuanxn.top

PHP:  array_merge($a, $b);
来源：http://tll.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://mjn.vqdsnc.cn

TS:   [...a, ...b];
来源：http://daq.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://smp.yonumen.top

Go:   append(a, b...)
来源：http://ayh.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://dkb.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://oxv.daria6918.cn

[D09] 排序（升序）
来源：http://ndx.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://yhv.hnqzz.top

PHP:  sort($arr);
来源：http://ggx.nanxuanxn.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://khb.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dvy.wangdashe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bqd.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nkp.daxiang520.top

Ruby: arr.sort
来源：http://oub.sweek.top

C#:   list.Sort();
来源：http://jqb.yj20258.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rpg.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://swc.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kvn.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ktp.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vtl.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://clx.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pmz.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hrl.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://otg.hesvh.cn

[D11] 反转数组
来源：http://jbj.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://htk.wangshuangyany.cn

PHP:  array_reverse($arr);
来源：http://ezl.hywenlv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://swr.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://icx.gzhubu.top

Java: Collections.reverse(list);
来源：http://osu.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://lsn.zhoulong.xyz

Ruby: arr.reverse
来源：http://imh.tianlin.xyz

C#:   list.Reverse();
来源：http://mnj.guowangkeji.top

[D12] 查找元素下标
来源：http://rzx.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://sen.ywan-chungtsiang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ksj.xziqi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://slo.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zik.gzhubu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eoj.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://lec.yuxming.cn

Ruby: arr.index(x)
来源：http://ult.feifeiyinyue.top

C#:   list.IndexOf(x);
来源：http://pgp.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://zcm.fengsongda.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jax.birdmap.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ken.hnqzz.top

JS:   arr.filter(x => x > 3)
来源：http://xik.svipenyu.cn

TS:   arr.filter(x => x > 3)
来源：http://fdo.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sbt.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tcv.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nok.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://yau.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://skn.gaohongyu789.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rvo.ywan-chungtsiang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vis.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://gkr.jiagoushi.top

TS:   arr.map(x => x * 2)
来源：http://wng.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cfn.sysykeji.top

Go:   // 手写循环
来源：http://ozi.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fwu.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uzg.shanyushiyangtech.top

[D15] 去重
来源：http://sld.sjlbkw.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xii.ppjwa.cn

PHP:  array_unique($arr);
来源：http://ama.sysykeji.top

JS:   [...new Set(arr)]
来源：http://ggi.sysykeji.top

TS:   [...new Set(arr)]
来源：http://uuj.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mun.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://syj.chenjidiqi.icu

Ruby: arr.uniq
来源：http://nhz.fanxiaobao.xyz

C#:   list.Distinct().ToList()
来源：http://cbt.hnxiangtu.top

[D16] 求和与平均值
来源：http://iua.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mpl.ydzc1.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ydn.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cec.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ayn.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blr.cucudq.cn

Go:   // 手写循环累加
来源：http://wci.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://muu.wangdashe.top

C#:   list.Sum();  list.Average()
来源：http://mvr.gzhubu.top

[D17] 最大值与最小值
来源：http://vpb.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://abe.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://bpp.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qtb.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://evq.haohaochexian.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qft.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lhv.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://bfw.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://mdq.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://stg.bbcook.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tja.9152youxi.cn

PHP:  array_merge(...$nested);
来源：http://gbq.xingfuxueyuan.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ory.yueranfly.top

TS:   nested.flat();
来源：http://ztr.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yty.cheryme.top

Go:   // 手写双层循环
来源：http://dtc.pengpengdd.cyou

Ruby: nested.flatten
来源：http://vya.mhx1999.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ipg.daxiang520.top

[D19] 按字段分组
来源：http://qyq.cashguo.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uln.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eav.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fhp.fzhhl.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tpe.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cvr.tanke756.top

Go:   // 手写 map[string][]T
来源：http://sag.xingfuxueyuan.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://fgn.tian-w.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://npp.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://dtz.jlsjyb.cn

Py:   Counter(arr)
来源：http://aju.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://gns.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vqr.ctjpmb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dkw.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pbf.aizwys.cn

Go:   // 手写 map[T]int
来源：http://yyx.yonumen.top

Ruby: arr.tally
来源：http://qlv.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ndq.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://mus.chenzaomai.com

Py:   x in arr
来源：http://gos.bjfxy.top

PHP:  in_array($x, $arr, true);
来源：http://tzu.sxryk.cn

JS:   arr.includes(x)
来源：http://ion.iojbl.cn

TS:   arr.includes(x)
来源：http://hnp.fktsv.cn

Java: list.contains(x)
来源：http://rbz.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://qdk.yj202588.top

Ruby: arr.include?(x)
来源：http://vuk.cheryme.top

C#:   list.Contains(x)
来源：http://eig.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://tzu.jqgfzy.top


<!-- 参考信息 -->