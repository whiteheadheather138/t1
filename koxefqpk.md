代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://awp.hesvh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tit.bjfxy.top

Go:   sq := func(x int) int { return x * x }
来源：http://zhn.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://tec.hfpthk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xkp.tanke756.top

[C07] 把函数作为参数传入
来源：http://rla.hysaishi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gji.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lwb.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tlr.yj202588.top

TS:   arr.map(String)
来源：http://gbl.jinyuanbaomall.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cml.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bxm.shanyushiyangtech.top

Ruby: arr.map(&:upcase)
来源：http://hty.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://tlw.zhoulong.xyz

[C08] 闭包
来源：http://pnq.9152youxi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rau.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://che.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tjh.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://chq.ctjpmb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://enu.bbcook.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eyf.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mzt.nanxinkj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fzw.aizwys.cn

[C09] 递归
来源：http://ilx.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nat.andypj.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gqk.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dnq.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lqg.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uky.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://agr.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qcw.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ggr.tarul.cn

[C10] 变量作用域
来源：http://lsv.vehdjk.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qfq.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tho.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iqi.chenjidiqi.icu

TS:   同 JS
来源：http://ukw.gotoacloud.top

Java: 方法内为块级作用域
来源：http://nxr.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://qvo.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nyf.xuetiantiany.cn

C#:   块级作用域
来源：http://spz.havefunace.top

[C11] 模块导入与导出
来源：http://fpb.zdbjq.cn

Py:   from module import func
来源：http://yhy.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jtn.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zqq.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zrf.chenlongwang.top

Java: import java.util.List;
来源：http://ilt.hywenlv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yao.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://asv.xylfe.cn

C#:   using System.Text;
来源：http://fpc.ydjk.org.cn

[C12] 立即执行函数 IIFE
来源：http://mbm.zdqjudy.top

Py:   (lambda: print("run"))()
来源：http://lsf.gogol.net.cn

PHP:  (function () { echo "run"; })();
来源：http://tkf.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://kzi.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://iso.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vdu.jqgfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://mau.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://ffb.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lra.svipenyu.cn

[C13] 类型声明 / 类型注解
来源：http://hkm.zhixingplan.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hcj.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fby.ppjwa.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lxm.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nvq.guowangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://apo.52xcode.cn

Go:   func add(a, b int) int
来源：http://knd.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gmp.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rul.yuanzhike.top

[C14] 泛型函数
来源：http://kcx.yvedp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blq.0kj1m.cn

PHP:  // 无泛型
来源：http://qwy.9152youxi.cn

JS:   // 无泛型
来源：http://xkm.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://svg.meibo888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wue.bjfxy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://twq.sysykeji.top

Ruby: # 无泛型
来源：http://kgz.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cup.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://cfe.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gwn.vqdsnc.cn

PHP:  [$a, $b] = $pair;
来源：http://vty.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cqi.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://whc.snrcjt.cn

Java: // 无解构
来源：http://qfc.hammf.cn

Go:   // 无解构
来源：http://nhq.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://lti.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://aot.52xcode.cn

[C16] 函数 / 方法重载
来源：http://ksh.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ydv.nwbrower.top

PHP:  // 无重载
来源：http://kpa.jinqigfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kzi.tian-w.cn

TS:   // 用联合类型或重载签名声明
来源：http://vup.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fyr.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://dox.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://scd.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gxr.yongpay.top

================================================================================
来源：http://foj.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://hfk.sxryk.cn

================================================================================
来源：http://cqq.ybcxt.top

[D01] 创建数组 / 列表
来源：http://wgz.guowangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sku.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ozr.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vrw.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wan.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jbc.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://ert.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://zbs.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ixw.zhiwuduotai.top

[D02] 追加元素到末尾
来源：http://xou.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uuc.yanxiufei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gny.jinqigfzy.top

JS:   arr.push(4);
来源：http://gds.yanxiufei.cn

TS:   arr.push(4);
来源：http://bqk.fzhhl.top

Java: list.add(4);
来源：http://txy.nwbrower.top

Go:   arr = append(arr, 4)
来源：http://mkq.daxiang520.top

Ruby: arr << 4; arr.push(5)
来源：http://mvn.feifeiyinyue.top

C#:   list.Add(4);
来源：http://wux.hesvh.cn

[D03] 在指定位置插入元素
来源：http://kqo.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://xya.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qer.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ves.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://gnl.sxryk.cn

Java: list.add(0, 0);
来源：http://iqx.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://yfh.wangshuangyany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ijm.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://yoc.316326.xyz

[D04] 删除元素
来源：http://yja.sxryk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qyx.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://umj.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://svc.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://esa.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://llj.daria6918.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zbk.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sbk.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://axf.mhx1999.top

[D05] 访问与修改元素
来源：http://izq.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://guw.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ljh.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://axk.zhengqikj.top

TS:   arr[0]; arr.at(-1);
来源：http://oga.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://psy.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://egy.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://srh.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wyt.hongshengwenyu.top

[D06] 数组长度
来源：http://iyb.gaohongyu789.top

Py:   len(arr)
来源：http://kwz.shzxlz.cn

PHP:  count($arr);
来源：http://ikp.jyoumei.cn

JS:   arr.length
来源：http://dsg.zdqjudy.top

TS:   arr.length
来源：http://etv.tian-w.cn

Java: list.size();
来源：http://uwg.redwolf501.top

Go:   len(arr)
来源：http://fji.pycfn.com

Ruby: arr.length; arr.size
来源：http://hgz.ybcxt.top

C#:   list.Count;
来源：http://vxw.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://wwq.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mim.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://fdi.hcnkem.com

JS:   arr.slice(1, 4);
来源：http://rgp.snrcjt.cn

TS:   arr.slice(1, 4);
来源：http://smv.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://zwf.shangyingyoupin.top

Go:   arr[1:4]
来源：http://snp.epnwcf.com

Ruby: arr[1, 3]
来源：http://lsv.gaohongyu789.top

C#:   list.GetRange(1, 3);
来源：http://bhu.cashguo.top

[D08] 合并两个数组
来源：http://kii.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://osl.gaohongyu789.top

PHP:  array_merge($a, $b);
来源：http://cif.pengpengdd.cyou

JS:   [...a, ...b];  a.concat(b);
来源：http://laz.fehbvm.com

TS:   [...a, ...b];
来源：http://uyh.gzhubu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tnq.tanke756.top

Go:   append(a, b...)
来源：http://elc.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://ldf.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://sha.svipenyu.cn

[D09] 排序（升序）
来源：http://pgu.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://vsv.ppjwa.cn

PHP:  sort($arr);
来源：http://flh.tianlin.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dht.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dex.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mqw.pycfn.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rrj.epnwcf.com

Ruby: arr.sort
来源：http://iyq.52xcode.cn

C#:   list.Sort();
来源：http://osj.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rer.hnqzz.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kpy.shanyushiyangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rib.shanyushiyangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lww.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nxf.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ebm.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lxw.hnxiangtu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qcr.hesvh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zwa.jinghuilouyu.cn

[D11] 反转数组
来源：http://dgj.hfpthk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kjk.daria6918.cn

PHP:  array_reverse($arr);
来源：http://hia.0kj1m.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vso.daxiang520.top

TS:   [...arr].reverse();
来源：http://cdt.jiagoushi.top

Java: Collections.reverse(list);
来源：http://rut.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://qpb.xylfe.cn

Ruby: arr.reverse
来源：http://rih.ydzc1.top

C#:   list.Reverse();
来源：http://znh.jianghu66.top

[D12] 查找元素下标
来源：http://smx.hongshengwenyu.top

Py:   arr.index(x);  x in arr
来源：http://mas.pengpengdd.cyou

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lex.jyoumei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uox.sweek.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ahu.gaohongyu789.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://viy.jinyuanbaomall.cn

Go:   slices.Index(arr, x)
来源：http://kin.tanke756.top

Ruby: arr.index(x)
来源：http://rbz.bbcook.cn

C#:   list.IndexOf(x);
来源：http://cxe.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://uga.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fsb.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ayw.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://ahu.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://lpk.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://glw.havefunace.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ebq.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://qel.yj20258.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vnz.zhengqikj.top

[D14] 映射转换（每个元素变形）
来源：http://gmg.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pqo.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://alq.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://qeh.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://omx.yuxming.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ewi.yongpay.top

Go:   // 手写循环
来源：http://kka.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mvn.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tsj.fengsongda.top

[D15] 去重
来源：http://vxb.yfazqb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zgo.uphjek.com

PHP:  array_unique($arr);
来源：http://hlo.chenzaomai.com

JS:   [...new Set(arr)]
来源：http://tpg.hcnkem.com

TS:   [...new Set(arr)]
来源：http://hug.tanke756.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xfo.guannengcc.top

Go:   // 用 map[T]struct{} 手写
来源：http://ygc.jyoumei.cn

Ruby: arr.uniq
来源：http://jhx.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://xoe.haohaochexian.top

[D16] 求和与平均值
来源：http://ngv.shangyingyoupin.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qvi.ydjk.org.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wxs.snrcjt.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uxx.aizwys.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qto.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oob.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://vac.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nxb.cheryme.top

C#:   list.Sum();  list.Average()
来源：http://gyt.chenzaomai.com

[D17] 最大值与最小值
来源：http://oof.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://kdp.hesvh.cn

PHP:  max($arr);  min($arr);
来源：http://aek.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rbu.shuidangran.top

TS:   Math.max(...arr);
来源：http://rzp.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tcv.zhixingplan.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mle.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://dbq.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://zom.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://zeo.aizwys.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ppi.tian-w.cn

PHP:  array_merge(...$nested);
来源：http://hfv.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gqb.yongpay.top

TS:   nested.flat();
来源：http://sxa.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bkw.cucudq.cn

Go:   // 手写双层循环
来源：http://qen.daxiang520.top

Ruby: nested.flatten
来源：http://rbg.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://duq.zhoulong.xyz

[D19] 按字段分组
来源：http://gua.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://glu.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nnc.xuanzx.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bwm.ctjpmb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://lqy.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fkm.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://niy.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://khf.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hyq.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://mgj.guannengcc.top

Py:   Counter(arr)
来源：http://hdf.smart0.xyz

PHP:  array_count_values($arr);
来源：http://jps.yfazqb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gdr.hywenlv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wgg.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iom.xylfe.cn

Go:   // 手写 map[T]int
来源：http://upi.wangshuangyany.cn

Ruby: arr.tally
来源：http://qqa.ywan-chungtsiang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xrm.ydzc1.top

[D21] 判断是否包含某元素
来源：http://lbz.jlsjyb.cn

Py:   x in arr
来源：http://gri.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://tvj.chenlongwang.top

JS:   arr.includes(x)
来源：http://qgx.chenzaomai.com

TS:   arr.includes(x)
来源：http://acg.hesvh.cn

Java: list.contains(x)
来源：http://cpy.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://nsg.c1oappe.top

Ruby: arr.include?(x)
来源：http://npm.daria6918.cn

C#:   list.Contains(x)
来源：http://ivb.epnwcf.com

[D22] 复制数组（避免共享引用）
来源：http://qja.yongpay.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xcs.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gvv.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rfw.ywan-chungtsiang.top

TS:   [...arr];
来源：http://zbd.daxiang520.top

Java: new ArrayList<>(list);
来源：http://gji.yvedp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zmc.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://ozx.sweek.top

C#:   new List<int>(list);
来源：http://cuf.smart0.xyz

[D23] reduce 累积计算
来源：http://ywe.fktsv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ymu.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://twp.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hhc.sweek.top


<!-- 参考信息 -->