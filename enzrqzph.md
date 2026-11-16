代发 wailian999

[C06] 匿名函数 / lambda
来源：http://uvg.gotoacloud.top

Py:   square = lambda x: x * x
来源：http://ijq.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zbv.52xcode.cn

JS:   const square = x => x * x;
来源：http://xhg.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://nbi.gaohongyu789.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://meg.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://gqo.jqgufenzy.top

Ruby: square = ->(x) { x * x }
来源：http://xse.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://xdp.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://jkr.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iqe.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://scw.shanyushiyangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hby.zhiwuduotai.top

TS:   arr.map(String)
来源：http://sgc.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://crq.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://otr.bjfxy.top

Ruby: arr.map(&:upcase)
来源：http://bkd.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ijw.xingfuxueyuan.xyz

[C08] 闭包
来源：http://haq.hnxiangtu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nbs.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wqs.shzxlz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dkg.tarul.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kyp.aizwys.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rqz.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dlc.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://law.fengsongda.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nfp.quarkkingdee.top

[C09] 递归
来源：http://bxk.tianlin.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zin.jyoumei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pgv.guowangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ddo.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xip.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://leq.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://els.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ezo.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vuw.jqgfzy.top

[C10] 变量作用域
来源：http://qxs.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://czu.chenlongwang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lqn.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qrb.cqqwz.cn

TS:   同 JS
来源：http://lup.tianlin.xyz

Java: 方法内为块级作用域
来源：http://qhl.zhengqikj.top

Go:   花括号块级作用域
来源：http://kar.hesvh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yuw.0kj1m.cn

C#:   块级作用域
来源：http://uij.snrcjt.cn

[C11] 模块导入与导出
来源：http://lkr.aibaodan.cn

Py:   from module import func
来源：http://jra.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wbp.yonumen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ekx.52xcode.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ito.yangfankeji.com

Java: import java.util.List;
来源：http://ymq.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fyt.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://vzx.cashguo.top

C#:   using System.Text;
来源：http://iwx.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://qeq.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://qvf.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://jif.xingfuxueyuan.xyz

JS:   (() => { console.log("run"); })();
来源：http://qzj.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://caa.hesvh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vps.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://cuk.birdmap.top

Ruby: -> { puts "run" }.call
来源：http://nxm.hnxiangtu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gmv.gzhubu.top

[C13] 类型声明 / 类型注解
来源：http://bne.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kno.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fib.xinyue.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xxr.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ose.fengsongda.top

Java: int add(int a, int b) { return a + b; }
来源：http://yvf.cashguo.top

Go:   func add(a, b int) int
来源：http://tul.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cgj.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://gkx.nanxuanxn.top

[C14] 泛型函数
来源：http://iqy.jiagoushi.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xca.xuetiantiany.cn

PHP:  // 无泛型
来源：http://yil.pycfn.com

JS:   // 无泛型
来源：http://mdz.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://etq.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iib.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jit.yonumen.top

Ruby: # 无泛型
来源：http://sdt.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qlu.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://pru.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qau.jqgfzy.top

PHP:  [$a, $b] = $pair;
来源：http://ulq.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xwi.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rkh.pycfn.com

Java: // 无解构
来源：http://lsm.pengpengdd.cyou

Go:   // 无解构
来源：http://ebg.yj20258888.top

Ruby: a, b = pair
来源：http://qbg.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://hsp.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://fxi.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tmj.cucudq.cn

PHP:  // 无重载
来源：http://pup.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qpk.xuanzx.com

TS:   // 用联合类型或重载签名声明
来源：http://bbe.yvedp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dwc.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://ziv.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://fwe.smart0.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://afz.iojbl.cn

================================================================================
来源：http://jaw.nanxinkj.top

D. 数组 / 列表 / 集合
来源：http://wnb.gotoacloud.top

================================================================================
来源：http://iyv.nanxuanxn.top

[D01] 创建数组 / 列表
来源：http://pht.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xqs.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eaq.yuanzhike.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tqw.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ocn.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ttm.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://fsn.tian-w.cn

Ruby: arr = [1, 2, 3]
来源：http://hrw.xziqi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hki.zhengqikj.top

[D02] 追加元素到末尾
来源：http://swv.hesvh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://suy.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nok.zhixingplan.top

JS:   arr.push(4);
来源：http://rms.dianchejie.cn

TS:   arr.push(4);
来源：http://rtx.fzhhl.top

Java: list.add(4);
来源：http://ycc.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://pax.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://xcq.ydjk.org.cn

C#:   list.Add(4);
来源：http://yeq.jianghu66.top

[D03] 在指定位置插入元素
来源：http://wjh.yj20258888.top

Py:   arr.insert(0, 0)
来源：http://apo.gaohongyu789.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dkr.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zck.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://ppc.wangdashe.top

Java: list.add(0, 0);
来源：http://dla.svipenyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bhk.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ote.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://yxt.tianlin.xyz

[D04] 删除元素
来源：http://kbb.shangyingyoupin.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pcb.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nzm.yangfankeji.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://peh.xziqi.cn

TS:   arr.splice(0, 1);
来源：http://oyq.svipenyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uhl.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cdx.ybcxt.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dzj.fengsongda.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://myt.iojbl.cn

[D05] 访问与修改元素
来源：http://tjm.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rtx.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ahz.cdnleiting.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qos.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://mvn.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://nqh.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://jnz.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://unr.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://biq.zdqjudy.top

[D06] 数组长度
来源：http://kjj.snrcjt.cn

Py:   len(arr)
来源：http://sfe.pengpengdd.cyou

PHP:  count($arr);
来源：http://ffs.316326.xyz

JS:   arr.length
来源：http://mzj.tarul.cn

TS:   arr.length
来源：http://zqh.aibaodan.cn

Java: list.size();
来源：http://qrv.daria6918.cn

Go:   len(arr)
来源：http://aur.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://lks.nwbrower.top

C#:   list.Count;
来源：http://mub.xziqi.cn

[D07] 切片 / 取子数组
来源：http://soj.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tur.jinghuilouyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://abt.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://kmf.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://fca.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://jpr.zhengqikj.top

Go:   arr[1:4]
来源：http://tba.yvedp.cn

Ruby: arr[1, 3]
来源：http://kkf.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://gcg.tian-w.cn

[D08] 合并两个数组
来源：http://vsu.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://iys.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://yxh.cheryme.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ntr.sysykeji.top

TS:   [...a, ...b];
来源：http://cor.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pit.vehdjk.com

Go:   append(a, b...)
来源：http://ibg.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://utb.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://gpe.dianchejie.cn

[D09] 排序（升序）
来源：http://rew.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://twy.quarkkingdee.top

PHP:  sort($arr);
来源：http://krn.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vrq.wangshuangyany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wux.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hkv.ppjwa.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blk.redwolf501.top

Ruby: arr.sort
来源：http://nkt.tanke756.top

C#:   list.Sort();
来源：http://rek.tian-w.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tlu.hongshengwenyu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ydx.jiagoushi.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ztn.ctjpmb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rxh.jiagoushi.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fzn.yj202588.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://exy.nwbrower.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pvr.iojbl.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gsf.wangshuangyany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://huy.hcnkem.com

[D11] 反转数组
来源：http://zcd.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://eja.gzhubu.top

PHP:  array_reverse($arr);
来源：http://ndx.ivvv.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://znf.gotoacloud.top

TS:   [...arr].reverse();
来源：http://nmn.hammf.cn

Java: Collections.reverse(list);
来源：http://bim.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://swk.yj20258888.top

Ruby: arr.reverse
来源：http://baj.smart0.xyz

C#:   list.Reverse();
来源：http://hnx.havefunace.top

[D12] 查找元素下标
来源：http://bwt.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://oev.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tli.sxryk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nec.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dse.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ifb.cdnleiting.top

Go:   slices.Index(arr, x)
来源：http://vjg.hcnkem.com

Ruby: arr.index(x)
来源：http://pld.jianghu66.top

C#:   list.IndexOf(x);
来源：http://wwi.daxiang520.top

[D13] 过滤（保留满足条件的）
来源：http://lof.shuidangran.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tjo.mhx1999.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ijl.jqgufenzy.top

JS:   arr.filter(x => x > 3)
来源：http://xxh.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://wtz.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jdt.yj202588.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dpj.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://jgd.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://hgu.vqdsnc.cn

[D14] 映射转换（每个元素变形）
来源：http://lov.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xrj.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xwg.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://ftf.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://fsr.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kmn.bjfxy.top

Go:   // 手写循环
来源：http://hbu.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ahm.zhixingplan.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zrn.mhx1999.top

[D15] 去重
来源：http://tbo.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://roy.mhx1999.top

PHP:  array_unique($arr);
来源：http://frf.shuidangran.top

JS:   [...new Set(arr)]
来源：http://hge.jianghu66.top

TS:   [...new Set(arr)]
来源：http://fgc.yueranfly.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xyf.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://byf.xinyue.icu

Ruby: arr.uniq
来源：http://fwo.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://uzu.dashuyun.cn

[D16] 求和与平均值
来源：http://hif.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bhc.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kba.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jok.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jcf.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xhy.nanxinkj.top

Go:   // 手写循环累加
来源：http://mwv.guowangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mnp.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://qmz.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://bjm.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://abt.tian-w.cn

PHP:  max($arr);  min($arr);
来源：http://mgf.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ikl.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://inn.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ciy.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wnf.sxryk.cn

Ruby: arr.max;  arr.min
来源：http://xay.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://ndy.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://snf.hesvh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://azr.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://dph.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dtr.xingfuxueyuan.xyz

TS:   nested.flat();
来源：http://gbg.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fzk.ybcxt.top

Go:   // 手写双层循环
来源：http://sjw.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://ijj.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rhx.hnqzz.top

[D19] 按字段分组
来源：http://vwq.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mgg.jinyuanbaomall.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bdu.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xto.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://phy.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bsx.mhx1999.top

Go:   // 手写 map[string][]T
来源：http://fxq.shanyushiyangtech.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://adp.tian-w.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ivj.gotoacloud.top

[D20] 统计每个元素出现次数
来源：http://ikv.fengsongda.top

Py:   Counter(arr)
来源：http://hoo.epnwcf.com

PHP:  array_count_values($arr);
来源：http://iqh.smart0.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://myv.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ogk.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kai.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://fmu.zhiwuduotai.top

Ruby: arr.tally
来源：http://aar.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://smc.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://smd.jlsjyb.cn

Py:   x in arr
来源：http://ztg.chenzaomai.com

PHP:  in_array($x, $arr, true);
来源：http://goi.yonumen.top

JS:   arr.includes(x)
来源：http://ypa.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://svm.mhx1999.top

Java: list.contains(x)
来源：http://qie.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://zqi.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://sbg.jyoumei.cn

C#:   list.Contains(x)
来源：http://amz.gogol.net.cn

[D22] 复制数组（避免共享引用）
来源：http://exq.jinghuilouyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cwf.dashuyun.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://asl.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rbs.xuetiantiany.cn

TS:   [...arr];
来源：http://dop.yj202588.top

Java: new ArrayList<>(list);
来源：http://wcq.yj202588.top

Go:   copied := append([]int(nil), arr...)
来源：http://zzi.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://bit.9152youxi.cn

C#:   new List<int>(list);
来源：http://nlg.bbcook.cn


<!-- 参考信息 -->