代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://exu.wangdashe.top

Go:   return a, b
来源：http://nfy.yj20258888.top

Ruby: return a, b
来源：http://puo.shanyushiyangtech.top

C#:   return (a, b);              // ValueTuple
来源：http://kjx.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://rpw.daria6918.cn

Py:   square = lambda x: x * x
来源：http://llp.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wuk.jyoumei.cn

JS:   const square = x => x * x;
来源：http://quy.daria6918.cn

TS:   const square = (x: number): number => x * x;
来源：http://opx.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oje.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ysc.iojbl.cn

Ruby: square = ->(x) { x * x }
来源：http://mag.yvedp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ucq.yj202588.top

[C07] 把函数作为参数传入
来源：http://ise.ppjwa.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jwn.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://vrs.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mwv.yuanzhike.top

TS:   arr.map(String)
来源：http://sbg.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cwf.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://usd.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://znu.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://vfx.ywan-chungtsiang.top

[C08] 闭包
来源：http://wbm.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zug.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://org.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dge.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mrn.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uip.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ylt.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tcm.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lfi.shanyushiyangkeji.top

[C09] 递归
来源：http://iwx.sxryk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pfm.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iuq.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qtc.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dbh.hammf.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://khy.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ynw.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lju.nanxinkj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bll.nanxuanxn.top

[C10] 变量作用域
来源：http://nwv.zhijiandao.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://how.jinghuilouyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yin.aizwys.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pkh.jianghu66.top

TS:   同 JS
来源：http://kmy.aibaodan.cn

Java: 方法内为块级作用域
来源：http://jvg.haohaochexian.top

Go:   花括号块级作用域
来源：http://nky.jinghuilouyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nug.zhaomingkeji.xyz

C#:   块级作用域
来源：http://bvd.sufxvd.cn

[C11] 模块导入与导出
来源：http://qjh.havefunace.top

Py:   from module import func
来源：http://elm.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qnb.jqgfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dhi.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ttt.pengpengdd.cyou

Java: import java.util.List;
来源：http://nkk.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uax.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://zmd.fanxiaobao.xyz

C#:   using System.Text;
来源：http://whx.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://pjv.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://iar.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://anc.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://oqs.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://ftm.nanxuanxn.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lue.cheryme.top

Go:   func() { fmt.Println("run") }()
来源：http://eap.jianghu66.top

Ruby: -> { puts "run" }.call
来源：http://eqe.pycfn.com

C#:   // 无 IIFE：用静态构造函数
来源：http://fhy.hywenlv.cn

[C13] 类型声明 / 类型注解
来源：http://hcy.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pxk.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fvl.yfazqb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fsa.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vmv.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://cmj.haohaochexian.top

Go:   func add(a, b int) int
来源：http://dxp.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eou.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://gkw.chenzaomai.com

[C14] 泛型函数
来源：http://yth.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kut.havefunace.top

PHP:  // 无泛型
来源：http://ske.c1oappe.top

JS:   // 无泛型
来源：http://jbw.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cup.jinyuanbaomall.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yqq.dashuyun.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tth.hongshengwenyu.top

Ruby: # 无泛型
来源：http://ofg.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pub.epnwcf.com

[C15] 解构 / 展开参数
来源：http://wgx.0kj1m.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cmt.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://ogb.chenlongwang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dll.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bib.sjlbkw.cn

Java: // 无解构
来源：http://ors.epnwcf.com

Go:   // 无解构
来源：http://opj.tianlin.xyz

Ruby: a, b = pair
来源：http://zwk.52xcode.cn

C#:   var (a, b) = pair;
来源：http://rxe.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://ebt.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vjf.xylfe.cn

PHP:  // 无重载
来源：http://dxe.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://eau.tian-w.cn

TS:   // 用联合类型或重载签名声明
来源：http://iyw.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gpk.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://bbs.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://udm.haohaochexian.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uty.pycfn.com

================================================================================
来源：http://qhz.shangyingyoupin.top

D. 数组 / 列表 / 集合
来源：http://fxm.zhoulong.xyz

================================================================================
来源：http://obt.tarul.cn

[D01] 创建数组 / 列表
来源：http://xsf.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://dqd.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fmd.smart0.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kpx.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bzh.jqgfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kcw.ctjpmb.com

Go:   arr := []int{1, 2, 3}
来源：http://rwe.zdbjq.cn

Ruby: arr = [1, 2, 3]
来源：http://znl.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ywe.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://zde.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://erk.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xfq.gotoacloud.top

JS:   arr.push(4);
来源：http://xfh.tianlin.xyz

TS:   arr.push(4);
来源：http://bcl.ppjwa.cn

Java: list.add(4);
来源：http://zyz.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://wqe.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ses.meibo888.top

C#:   list.Add(4);
来源：http://eoi.c1oappe.top

[D03] 在指定位置插入元素
来源：http://sfw.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://lpj.bjfxy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zgm.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://azz.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://uxw.daxiang520.top

Java: list.add(0, 0);
来源：http://klu.yongpay.top

Go:   arr = append([]int{0}, arr...)
来源：http://qwo.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cfg.zhixingplan.top

C#:   list.Insert(0, 0);
来源：http://cwz.jianghu66.top

[D04] 删除元素
来源：http://qjh.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fgw.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sht.yuanzhike.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vfb.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://zzs.52xcode.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://idl.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://txe.yj20258.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hra.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sps.aizwys.cn

[D05] 访问与修改元素
来源：http://zjl.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fbg.guowangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://shm.0kj1m.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lsd.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://tpw.yuxming.cn

Java: list.get(0); list.set(0, 9);
来源：http://mve.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://sbb.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tzw.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aoj.tian-w.cn

[D06] 数组长度
来源：http://xas.ctjpmb.com

Py:   len(arr)
来源：http://gii.jqgfzy.top

PHP:  count($arr);
来源：http://ixi.xziqi.cn

JS:   arr.length
来源：http://uto.ctjpmb.com

TS:   arr.length
来源：http://oqj.xziqi.cn

Java: list.size();
来源：http://ipm.dianchejie.cn

Go:   len(arr)
来源：http://qbd.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://xpd.fanxiaobao.xyz

C#:   list.Count;
来源：http://wgp.dianchejie.cn

[D07] 切片 / 取子数组
来源：http://wen.aizwys.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dcz.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://mfk.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://vvv.nanxinkj.top

TS:   arr.slice(1, 4);
来源：http://bhx.yangfankeji.com

Java: list.subList(1, 4);
来源：http://xab.guannengcc.top

Go:   arr[1:4]
来源：http://awd.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://tri.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://qgw.hongshengwenyu.top

[D08] 合并两个数组
来源：http://mzr.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://jkj.iojbl.cn

PHP:  array_merge($a, $b);
来源：http://pox.epnwcf.com

JS:   [...a, ...b];  a.concat(b);
来源：http://nos.yangfankeji.com

TS:   [...a, ...b];
来源：http://ehg.sufxvd.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nfh.yuanzhike.top

Go:   append(a, b...)
来源：http://psb.shanyushiyangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://wvx.yuanzhike.top

C#:   a.Concat(b).ToList()
来源：http://xyu.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://ruj.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://qod.yuxming.cn

PHP:  sort($arr);
来源：http://qky.sysykeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rnh.gotoacloud.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ieb.epnwcf.com

Java: Collections.sort(list);  list.sort(null);
来源：http://rhj.0kj1m.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ouf.hnxiangtu.top

Ruby: arr.sort
来源：http://zbc.nanxuanxn.top

C#:   list.Sort();
来源：http://few.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pyo.bjfxy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://svk.gzhubu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nag.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://una.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://slk.chenjidiqi.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://org.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://egx.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dia.shanyushiyangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://czi.guannengcc.top

[D11] 反转数组
来源：http://sms.ehwqpu.com

Py:   arr[::-1];  arr.reverse()
来源：http://lvt.jqgufenzy.top

PHP:  array_reverse($arr);
来源：http://loo.fktsv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bty.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://yak.ywan-chungtsiang.top

Java: Collections.reverse(list);
来源：http://kel.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://ict.ydzc1.top

Ruby: arr.reverse
来源：http://omv.zhiwuduotai.top

C#:   list.Reverse();
来源：http://mil.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://ugl.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://snq.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mzd.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kdf.tanke756.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lgr.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://htr.iojbl.cn

Go:   slices.Index(arr, x)
来源：http://ziy.hnqzz.top

Ruby: arr.index(x)
来源：http://huh.yj20258.top

C#:   list.IndexOf(x);
来源：http://nok.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://pdx.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bgy.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aam.zhixingplan.top

JS:   arr.filter(x => x > 3)
来源：http://ftf.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://fwt.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://koe.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://swm.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://qtc.mhx1999.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pmi.iojbl.cn

[D14] 映射转换（每个元素变形）
来源：http://mig.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rhy.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gja.jianghu66.top

JS:   arr.map(x => x * 2)
来源：http://xpq.ppjwa.cn

TS:   arr.map(x => x * 2)
来源：http://jei.jianghu66.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vbm.cucudq.cn

Go:   // 手写循环
来源：http://eyf.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://ujw.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://mco.cashguo.top

[D15] 去重
来源：http://ojs.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zzk.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://tsv.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://cdk.kuanghao11.cn

TS:   [...new Set(arr)]
来源：http://bif.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bmy.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://moz.vehdjk.com

Ruby: arr.uniq
来源：http://ctc.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://jzq.cucudq.cn

[D16] 求和与平均值
来源：http://ycp.xuanzx.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qum.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gmg.xuanzx.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://evk.zhoulong.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mef.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nrr.fzhhl.top

Go:   // 手写循环累加
来源：http://mmx.smart0.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ibd.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://fqu.pengpengdd.cyou

[D17] 最大值与最小值
来源：http://szx.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://hzo.jinqigfzy.top

PHP:  max($arr);  min($arr);
来源：http://ojc.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://chj.iojbl.cn

TS:   Math.max(...arr);
来源：http://xsa.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://pwt.tianlin.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kuk.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://zns.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://cea.jinyuanbaomall.cn

[D18] 扁平化嵌套数组
来源：http://sto.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://apd.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://ped.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://izz.gzhubu.top

TS:   nested.flat();
来源：http://usf.hnxiangtu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ihe.gogol.net.cn

Go:   // 手写双层循环
来源：http://bnx.yuanzhike.top

Ruby: nested.flatten
来源：http://dwu.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kqx.uphjek.com

[D19] 按字段分组
来源：http://ohz.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://knm.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gkj.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ypt.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bwp.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ywo.xuanzx.com

Go:   // 手写 map[string][]T
来源：http://rtl.zhongyouzk.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vlx.jyoumei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bsf.fktsv.cn

[D20] 统计每个元素出现次数
来源：http://tws.zhengqikj.top

Py:   Counter(arr)
来源：http://icb.tian-w.cn

PHP:  array_count_values($arr);
来源：http://wwh.smart0.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yha.snrcjt.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wge.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oyn.hesvh.cn

Go:   // 手写 map[T]int
来源：http://poz.zhijiandao.cn

Ruby: arr.tally
来源：http://ort.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hve.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://qrd.hfpthk.cn

Py:   x in arr
来源：http://dbp.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://pqi.quarkkingdee.top

JS:   arr.includes(x)
来源：http://mwh.jlsjyb.cn

TS:   arr.includes(x)
来源：http://trw.hywenlv.cn

Java: list.contains(x)
来源：http://kvk.daxiang520.top

Go:   slices.Contains(arr, x)
来源：http://lgp.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://sbf.yfazqb.com

C#:   list.Contains(x)
来源：http://ody.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://ive.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kui.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iug.andypj.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nra.ydjk.org.cn

TS:   [...arr];
来源：http://ect.wangshuangyany.cn


<!-- 参考信息 -->