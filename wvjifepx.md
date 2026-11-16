代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://api.fengsongda.top

Go:   return a, b
来源：http://kud.jqgfzy.top

Ruby: return a, b
来源：http://xnc.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://kmv.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://yux.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://bff.fengsongda.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cbl.dashuyun.cn

JS:   const square = x => x * x;
来源：http://cie.shuidangran.top

TS:   const square = (x: number): number => x * x;
来源：http://uld.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gjv.jinqigufen.top

Go:   sq := func(x int) int { return x * x }
来源：http://ebz.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://mjj.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yye.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://yfu.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ior.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zbc.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nyy.jqgfzy.top

TS:   arr.map(String)
来源：http://sui.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ddz.ydjk.org.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://avx.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://hmm.snrcjt.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rgu.andypj.xyz

[C08] 闭包
来源：http://uzc.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ujh.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qds.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gkn.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vxn.ctjpmb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ive.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sov.snrcjt.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dcu.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://psy.cdnleiting.top

[C09] 递归
来源：http://jva.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mus.cucudq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cgs.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://njw.xuanzx.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gpj.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aja.yuxming.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mfm.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jqk.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://etb.cashguo.top

[C10] 变量作用域
来源：http://nbt.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jzs.pengpengdd.cyou

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aqw.kuanghao11.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://doj.nwbrower.top

TS:   同 JS
来源：http://emw.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://lne.ctjpmb.com

Go:   花括号块级作用域
来源：http://ipx.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nqv.hesvh.cn

C#:   块级作用域
来源：http://ijd.nwbrower.top

[C11] 模块导入与导出
来源：http://wpv.aizwys.cn

Py:   from module import func
来源：http://jpl.yangfankeji.com

PHP:  require "file.php";  或 use App\Service;
来源：http://aly.sweek.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bbp.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://aqp.iojbl.cn

Java: import java.util.List;
来源：http://hnx.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qoa.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://veo.tarul.cn

C#:   using System.Text;
来源：http://wij.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://nrc.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://dmj.xziqi.cn

PHP:  (function () { echo "run"; })();
来源：http://xng.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://bds.xylfe.cn

TS:   (() => { console.log("run"); })();
来源：http://ffx.zdqjudy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pvk.0kj1m.cn

Go:   func() { fmt.Println("run") }()
来源：http://gqz.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://lrm.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cfy.yongpay.top

[C13] 类型声明 / 类型注解
来源：http://fxa.cdnleiting.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mma.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ztl.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fou.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rfk.jqgufenzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://roj.hywenlv.cn

Go:   func add(a, b int) int
来源：http://loi.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jeb.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vmq.daria6918.cn

[C14] 泛型函数
来源：http://vhc.fengsongda.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ged.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://kxm.hnxiangtu.top

JS:   // 无泛型
来源：http://tte.dashuyun.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pxg.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cor.wangdashe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wru.ivvv.top

Ruby: # 无泛型
来源：http://qjg.ydjk.org.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vep.aibaodan.cn

[C15] 解构 / 展开参数
来源：http://sau.jinqigufen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://exl.wangdashe.top

PHP:  [$a, $b] = $pair;
来源：http://jnh.yuanzhike.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fsz.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://boh.ehwqpu.com

Java: // 无解构
来源：http://loh.dashuyun.cn

Go:   // 无解构
来源：http://nxl.jlsjyb.cn

Ruby: a, b = pair
来源：http://pku.shanyushiyangtech.top

C#:   var (a, b) = pair;
来源：http://zyv.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://erm.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jur.hnxiangtu.top

PHP:  // 无重载
来源：http://vnz.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://upv.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://ixo.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ivk.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://sdu.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://hfe.cucudq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xxx.sufxvd.cn

================================================================================
来源：http://xkm.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://cjc.yj20258888.top

================================================================================
来源：http://cko.316326.xyz

[D01] 创建数组 / 列表
来源：http://twf.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qas.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gge.cashguo.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ozx.zdbjq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://els.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://grm.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://xlg.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://mqi.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lza.cashguo.top

[D02] 追加元素到末尾
来源：http://ffd.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bhp.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sbg.svipenyu.cn

JS:   arr.push(4);
来源：http://xez.smart0.xyz

TS:   arr.push(4);
来源：http://bkl.ehwqpu.com

Java: list.add(4);
来源：http://ghm.jinqigufen.top

Go:   arr = append(arr, 4)
来源：http://kfb.epnwcf.com

Ruby: arr << 4; arr.push(5)
来源：http://onp.shangyingyoupin.top

C#:   list.Add(4);
来源：http://qoq.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://pyh.wangdashe.top

Py:   arr.insert(0, 0)
来源：http://oqu.feifeiyinyue.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ehu.hysaishi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rzo.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://ffi.hysaishi.cn

Java: list.add(0, 0);
来源：http://gqq.yj20258.top

Go:   arr = append([]int{0}, arr...)
来源：http://egc.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qjp.jinghuilouyu.cn

C#:   list.Insert(0, 0);
来源：http://wka.tian-w.cn

[D04] 删除元素
来源：http://ryd.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://puj.feifeiyinyue.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hmh.pengpengdd.cyou

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kdb.zhengqikj.top

TS:   arr.splice(0, 1);
来源：http://knu.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lnk.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ywc.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://egk.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sbc.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://sue.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uqj.gaohongyu789.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dfz.xingfuxueyuan.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nfb.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://hob.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://drd.shzxlz.cn

Go:   arr[0]; arr[0] = 9
来源：http://gaz.aibaodan.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nqi.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://alk.redwolf501.top

[D06] 数组长度
来源：http://mpn.ywan-chungtsiang.top

Py:   len(arr)
来源：http://hof.tian-w.cn

PHP:  count($arr);
来源：http://ybq.cucudq.cn

JS:   arr.length
来源：http://nwa.zhoulong.xyz

TS:   arr.length
来源：http://gdz.fanxiaobao.xyz

Java: list.size();
来源：http://xjb.hcnkem.com

Go:   len(arr)
来源：http://erb.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://vta.chenlongwang.top

C#:   list.Count;
来源：http://wfo.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://tfv.zhengqikj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eiz.yvedp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://faj.bbcook.cn

JS:   arr.slice(1, 4);
来源：http://lrw.aizwys.cn

TS:   arr.slice(1, 4);
来源：http://ksx.svipenyu.cn

Java: list.subList(1, 4);
来源：http://xrh.dashuyun.cn

Go:   arr[1:4]
来源：http://ztd.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://gcq.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://ajn.xuetiantiany.cn

[D08] 合并两个数组
来源：http://hei.hfpthk.cn

Py:   a + b;  a.extend(b)
来源：http://pfe.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://pik.redwolf501.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xku.ydjk.org.cn

TS:   [...a, ...b];
来源：http://hga.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sqh.tarul.cn

Go:   append(a, b...)
来源：http://pju.chenjidiqi.icu

Ruby: a + b;  a.concat(b)
来源：http://ven.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://vax.havefunace.top

[D09] 排序（升序）
来源：http://mnj.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://tpy.zdbjq.cn

PHP:  sort($arr);
来源：http://atn.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fpn.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fjo.tianlin.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://hzr.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hov.aibaodan.cn

Ruby: arr.sort
来源：http://tpo.andypj.xyz

C#:   list.Sort();
来源：http://jsc.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zqm.bjfxy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oxi.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ikw.yonumen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wsm.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wfw.jyoumei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qpg.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ene.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xtr.sweek.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qvq.yanxiufei.cn

[D11] 反转数组
来源：http://rvf.sweek.top

Py:   arr[::-1];  arr.reverse()
来源：http://yxx.guannengcc.top

PHP:  array_reverse($arr);
来源：http://vip.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kup.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://qeh.sjlbkw.cn

Java: Collections.reverse(list);
来源：http://rct.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://tru.cheryme.top

Ruby: arr.reverse
来源：http://wkf.wangshuangyany.cn

C#:   list.Reverse();
来源：http://bzu.nanxuanxn.top

[D12] 查找元素下标
来源：http://aly.yuanzhike.top

Py:   arr.index(x);  x in arr
来源：http://ppb.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://epd.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nuw.ehwqpu.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ixp.havefunace.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://unj.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://kac.feifeiyinyue.top

Ruby: arr.index(x)
来源：http://sqk.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://kfv.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://tkm.xingfuxueyuan.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://msl.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nmq.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://gmm.cqqwz.cn

TS:   arr.filter(x => x > 3)
来源：http://crv.mhx1999.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fyh.316326.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zuz.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://tgl.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gvx.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://ijn.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ogy.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lmd.ydjk.org.cn

JS:   arr.map(x => x * 2)
来源：http://mva.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://lou.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jcm.hammf.cn

Go:   // 手写循环
来源：http://cqe.0kj1m.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jod.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vxd.tianlin.xyz

[D15] 去重
来源：http://uji.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uyy.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://phj.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://ihs.jianghu66.top

TS:   [...new Set(arr)]
来源：http://nnk.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kas.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://eor.sxryk.cn

Ruby: arr.uniq
来源：http://mgo.zdqjudy.top

C#:   list.Distinct().ToList()
来源：http://tnm.smart0.xyz

[D16] 求和与平均值
来源：http://jwf.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uzs.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uom.nanxuanxn.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sse.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ruo.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tnn.snrcjt.cn

Go:   // 手写循环累加
来源：http://xud.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tpr.jianghu66.top

C#:   list.Sum();  list.Average()
来源：http://aez.vehdjk.com

[D17] 最大值与最小值
来源：http://fwc.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://lai.hcnkem.com

PHP:  max($arr);  min($arr);
来源：http://lqf.aizwys.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ria.nwbrower.top

TS:   Math.max(...arr);
来源：http://agh.bjfxy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://oge.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xor.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://ihs.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://omk.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://hgy.zdbjq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qry.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://rhb.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://grs.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://zcx.nanxuanxn.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://erb.jinyuanbaomall.cn

Go:   // 手写双层循环
来源：http://rhy.sxryk.cn

Ruby: nested.flatten
来源：http://lmj.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://elx.sjlbkw.cn

[D19] 按字段分组
来源：http://uts.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nyj.tarul.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yvb.birdmap.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qyv.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ypv.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yhs.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://qnv.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qvf.ehwqpu.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cgt.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://rjj.chenjidiqi.icu

Py:   Counter(arr)
来源：http://bls.haohaochexian.top

PHP:  array_count_values($arr);
来源：http://par.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rey.yuanzhike.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ifp.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kry.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://fib.birdmap.top

Ruby: arr.tally
来源：http://hwx.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fsf.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://opr.svipenyu.cn

Py:   x in arr
来源：http://xsg.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://qvt.tian-w.cn

JS:   arr.includes(x)
来源：http://ork.dianchejie.cn

TS:   arr.includes(x)
来源：http://vnp.fktsv.cn

Java: list.contains(x)
来源：http://lfz.wangshuangyany.cn

Go:   slices.Contains(arr, x)
来源：http://mvm.fktsv.cn

Ruby: arr.include?(x)
来源：http://xwf.cdnleiting.top

C#:   list.Contains(x)
来源：http://qod.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://lne.zhengqikj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kcx.hammf.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wdo.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wyv.tanke756.top

TS:   [...arr];
来源：http://yci.guowangkeji.top


<!-- 参考信息 -->