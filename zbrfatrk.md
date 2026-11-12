代发 wailian999

[C06] 匿名函数 / lambda
来源：http://vzp.cucudq.cn

Py:   square = lambda x: x * x
来源：http://wja.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://ttg.tanke756.top

JS:   const square = x => x * x;
来源：http://hkc.nanxinkj.top

TS:   const square = (x: number): number => x * x;
来源：http://irj.ppjwa.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gvu.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://wpu.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://vvy.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kmz.gzhubu.top

[C07] 把函数作为参数传入
来源：http://jld.yueranfly.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://irh.jinqigfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://dem.jianghu66.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lql.haohaochexian.top

TS:   arr.map(String)
来源：http://qta.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xkz.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://orn.ivvv.top

Ruby: arr.map(&:upcase)
来源：http://gka.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rpj.jinqigfzy.top

[C08] 闭包
来源：http://icu.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nww.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mfk.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wee.iojbl.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vlw.yongpay.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dse.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vcl.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ykg.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://smx.jianghu66.top

[C09] 递归
来源：http://ndr.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lvi.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zyj.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://irt.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lvp.zhengqikj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aze.hcnkem.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ter.ybcxt.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xwm.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sio.dianchejie.cn

[C10] 变量作用域
来源：http://hgo.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cbs.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mnp.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wej.xinyue.icu

TS:   同 JS
来源：http://qhx.sysykeji.top

Java: 方法内为块级作用域
来源：http://jre.havefunace.top

Go:   花括号块级作用域
来源：http://gak.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pyy.sysykeji.top

C#:   块级作用域
来源：http://jvm.zhijiandao.cn

[C11] 模块导入与导出
来源：http://fdx.jinqigufen.top

Py:   from module import func
来源：http://ljd.yuxming.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://est.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://jmq.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hzq.xuanzx.com

Java: import java.util.List;
来源：http://yqo.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gop.chenzaomai.com

Ruby: require "json"; require_relative "./util"
来源：http://guf.dianchejie.cn

C#:   using System.Text;
来源：http://bkf.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://kmk.cheryme.top

Py:   (lambda: print("run"))()
来源：http://pxv.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://dsi.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://bec.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://txj.gaohongyu789.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ume.epnwcf.com

Go:   func() { fmt.Println("run") }()
来源：http://vuj.aibaodan.cn

Ruby: -> { puts "run" }.call
来源：http://jsz.daria6918.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://skn.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://csq.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mga.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sny.smart0.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ljd.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ifc.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://wap.yangfankeji.com

Go:   func add(a, b int) int
来源：http://bcv.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fwj.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kzg.pengpengdd.cyou

[C14] 泛型函数
来源：http://npo.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://har.vqdsnc.cn

PHP:  // 无泛型
来源：http://els.jiagoushi.top

JS:   // 无泛型
来源：http://egh.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fro.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eej.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ccl.52xcode.cn

Ruby: # 无泛型
来源：http://wdf.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jko.shuidangran.top

[C15] 解构 / 展开参数
来源：http://jea.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wgk.vehdjk.com

PHP:  [$a, $b] = $pair;
来源：http://klm.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kjr.gaohongyu789.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aiv.vehdjk.com

Java: // 无解构
来源：http://lcm.jyoumei.cn

Go:   // 无解构
来源：http://kux.meibo888.top

Ruby: a, b = pair
来源：http://plc.shuidangran.top

C#:   var (a, b) = pair;
来源：http://ejv.cashguo.top

[C16] 函数 / 方法重载
来源：http://jzh.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xoy.0kj1m.cn

PHP:  // 无重载
来源：http://avl.svipenyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ncb.gotoacloud.top

TS:   // 用联合类型或重载签名声明
来源：http://vrh.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://swy.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://tbg.hongshengwenyu.top

Ruby: # 无重载：靠动态参数
来源：http://vlp.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bnb.ydzc1.top

================================================================================
来源：http://fbn.zhijiandao.cn

D. 数组 / 列表 / 集合
来源：http://akf.svipenyu.cn

================================================================================
来源：http://zbj.0kj1m.cn

[D01] 创建数组 / 列表
来源：http://twe.wangdashe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fyx.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vcd.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xcm.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://jbu.zdqjudy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nqz.bbcook.cn

Go:   arr := []int{1, 2, 3}
来源：http://ypl.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://hug.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fkp.sweek.top

[D02] 追加元素到末尾
来源：http://wih.cqqwz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hel.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gii.yuanzhike.top

JS:   arr.push(4);
来源：http://qod.xinyue.icu

TS:   arr.push(4);
来源：http://csh.jqgufenzy.top

Java: list.add(4);
来源：http://lrj.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://zbz.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://dmy.cqqwz.cn

C#:   list.Add(4);
来源：http://vpm.jianghu66.top

[D03] 在指定位置插入元素
来源：http://dak.hnxiangtu.top

Py:   arr.insert(0, 0)
来源：http://uqp.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://njs.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oxg.yonumen.top

TS:   arr.splice(0, 0, 0);
来源：http://uln.yonumen.top

Java: list.add(0, 0);
来源：http://kgp.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fve.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zzs.yfazqb.com

C#:   list.Insert(0, 0);
来源：http://asv.daria6918.cn

[D04] 删除元素
来源：http://mcy.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aom.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rkm.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jxp.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://tvu.tanke756.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://imc.gzhubu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bkb.ybcxt.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gcv.yuanzhike.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://orh.gzhubu.top

[D05] 访问与修改元素
来源：http://aay.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dfk.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://srz.bbcook.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iel.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://lbu.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://kkm.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://xlo.aibaodan.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nlq.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ufb.yfazqb.com

[D06] 数组长度
来源：http://bpk.cucudq.cn

Py:   len(arr)
来源：http://ixb.aibaodan.cn

PHP:  count($arr);
来源：http://xkj.gaohongyu789.top

JS:   arr.length
来源：http://unc.fengsongda.top

TS:   arr.length
来源：http://cfi.hnqzz.top

Java: list.size();
来源：http://tvf.xuanzx.com

Go:   len(arr)
来源：http://tyv.tanke756.top

Ruby: arr.length; arr.size
来源：http://qqg.0kj1m.cn

C#:   list.Count;
来源：http://pwo.hammf.cn

[D07] 切片 / 取子数组
来源：http://hza.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://svk.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://wiu.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://xnv.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://ahi.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://itg.xylfe.cn

Go:   arr[1:4]
来源：http://hff.svipenyu.cn

Ruby: arr[1, 3]
来源：http://hkw.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://nwu.pycfn.com

[D08] 合并两个数组
来源：http://uat.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://kwi.xinyue.icu

PHP:  array_merge($a, $b);
来源：http://cwq.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ozb.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://byw.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ezo.chenzaomai.com

Go:   append(a, b...)
来源：http://fzg.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://qqh.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://nfy.nwbrower.top

[D09] 排序（升序）
来源：http://npk.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://lqd.jqgfzy.top

PHP:  sort($arr);
来源：http://kdh.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cop.zhijiandao.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gfl.shanyushiyangtech.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dpg.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bok.uphjek.com

Ruby: arr.sort
来源：http://toe.zhijiandao.cn

C#:   list.Sort();
来源：http://yzq.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hox.zdbjq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://diy.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iub.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xra.ywan-chungtsiang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sru.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ecx.daxiang520.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hts.shuidangran.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qxt.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uvh.pycfn.com

[D11] 反转数组
来源：http://kbk.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://ydx.guannengcc.top

PHP:  array_reverse($arr);
来源：http://glf.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vns.hywenlv.cn

TS:   [...arr].reverse();
来源：http://sde.9152youxi.cn

Java: Collections.reverse(list);
来源：http://jqi.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://abc.fengsongda.top

Ruby: arr.reverse
来源：http://ucz.bjfxy.top

C#:   list.Reverse();
来源：http://rhb.yanxiufei.cn

[D12] 查找元素下标
来源：http://kgc.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://moe.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xsk.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://owl.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uqb.chenzaomai.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uwx.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://cog.sweek.top

Ruby: arr.index(x)
来源：http://tvv.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://prz.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://tcm.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iet.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sbh.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://igc.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://hkq.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qtw.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pfm.zhixingplan.top

Ruby: arr.select { |x| x > 3 }
来源：http://zhs.cheryme.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yst.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://sto.sufxvd.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://orc.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sya.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://aor.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://dke.316326.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://nod.mhx1999.top

Go:   // 手写循环
来源：http://pqo.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://agb.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://pph.shanyushiyangtech.top

[D15] 去重
来源：http://ywg.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cdl.xziqi.cn

PHP:  array_unique($arr);
来源：http://osy.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://imx.smart0.xyz

TS:   [...new Set(arr)]
来源：http://oho.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cig.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://yig.chenjidiqi.icu

Ruby: arr.uniq
来源：http://gwh.zhongyouzk.top

C#:   list.Distinct().ToList()
来源：http://tyv.gaohongyu789.top

[D16] 求和与平均值
来源：http://yjl.zhongyouzk.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://otf.redwolf501.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kiu.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nxv.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hve.sjlbkw.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wzh.yj20258888.top

Go:   // 手写循环累加
来源：http://zkr.ywan-chungtsiang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jwi.shanyushiyangtech.top

C#:   list.Sum();  list.Average()
来源：http://huw.ydzc1.top

[D17] 最大值与最小值
来源：http://btp.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://ysq.vqdsnc.cn

PHP:  max($arr);  min($arr);
来源：http://ehi.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ymi.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://gsh.ybcxt.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qlz.mhx1999.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cnz.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://aho.yongpay.top

C#:   list.Max();  list.Min()
来源：http://xiq.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://nao.wangshuangyany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lza.xinyue.icu

PHP:  array_merge(...$nested);
来源：http://yuv.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qyp.cucudq.cn

TS:   nested.flat();
来源：http://qde.yongpay.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yyj.gaohongyu789.top

Go:   // 手写双层循环
来源：http://xmo.sufxvd.cn

Ruby: nested.flatten
来源：http://kab.wangshuangyany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dii.iojbl.cn

[D19] 按字段分组
来源：http://mbp.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ifn.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hno.52xcode.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://efl.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zur.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tgv.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://gvj.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hbp.ctjpmb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bbg.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://wsy.c1oappe.top

Py:   Counter(arr)
来源：http://smj.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://gbn.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dtr.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wcc.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://czl.wangdashe.top

Go:   // 手写 map[T]int
来源：http://ajg.nanxinkj.top

Ruby: arr.tally
来源：http://icu.fanxiaobao.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wyh.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://lik.shanyushiyangkeji.top

Py:   x in arr
来源：http://egr.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://yez.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://xkj.fengsongda.top

TS:   arr.includes(x)
来源：http://zdi.guannengcc.top

Java: list.contains(x)
来源：http://ugn.zhoulong.xyz

Go:   slices.Contains(arr, x)
来源：http://sgk.ydjk.org.cn

Ruby: arr.include?(x)
来源：http://jte.epnwcf.com

C#:   list.Contains(x)
来源：http://lew.epnwcf.com

[D22] 复制数组（避免共享引用）
来源：http://tjd.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ami.zycfv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nva.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hdl.guowangkeji.top

TS:   [...arr];
来源：http://khx.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://bqx.zhengqikj.top

Go:   copied := append([]int(nil), arr...)
来源：http://pio.bjfxy.top

Ruby: arr.dup;  arr.clone
来源：http://qul.sufxvd.cn

C#:   new List<int>(list);
来源：http://log.svipenyu.cn


<!-- 参考信息 -->