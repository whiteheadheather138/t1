代发 wailian999

[C06] 匿名函数 / lambda
来源：http://nah.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://sro.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://vox.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://mac.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://oig.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ujf.shzxlz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xnm.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://etv.sysykeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://bhg.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://dwd.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vvj.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://pmh.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iyj.hysaishi.cn

TS:   arr.map(String)
来源：http://jhx.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jda.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tvi.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://lvw.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yan.jyoumei.cn

[C08] 闭包
来源：http://czn.meibo888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zbk.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rsr.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dvg.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://viz.cdnleiting.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vrj.cdnleiting.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dud.hongshengwenyu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rnj.birdmap.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vpc.shanyushiyangkeji.top

[C09] 递归
来源：http://zao.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fod.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lxf.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qgh.yanxiufei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://axf.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cxt.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://arj.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gzr.yonumen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mnh.jiagoushi.top

[C10] 变量作用域
来源：http://cfp.pycfn.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zbe.sufxvd.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rtv.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kjk.jiagoushi.top

TS:   同 JS
来源：http://tcr.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://tde.iojbl.cn

Go:   花括号块级作用域
来源：http://ibs.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tah.hfpthk.cn

C#:   块级作用域
来源：http://elh.iojbl.cn

[C11] 模块导入与导出
来源：http://syn.hcnkem.com

Py:   from module import func
来源：http://orf.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zgk.nanxinkj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tdw.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xhv.hywenlv.cn

Java: import java.util.List;
来源：http://waf.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vgz.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://dhm.meibo888.top

C#:   using System.Text;
来源：http://hji.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://civ.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://tmp.pengpengdd.cyou

PHP:  (function () { echo "run"; })();
来源：http://hwp.wangdashe.top

JS:   (() => { console.log("run"); })();
来源：http://yra.ivvv.top

TS:   (() => { console.log("run"); })();
来源：http://jhx.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xfj.yj20258.top

Go:   func() { fmt.Println("run") }()
来源：http://icv.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://cpg.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://htc.ppjwa.cn

[C13] 类型声明 / 类型注解
来源：http://jle.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fnp.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mfn.havefunace.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zkj.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lek.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://nzb.yj20258.top

Go:   func add(a, b int) int
来源：http://dgh.ywan-chungtsiang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sba.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://kqq.chenjidiqi.icu

[C14] 泛型函数
来源：http://hon.jinghuilouyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jeu.hcnkem.com

PHP:  // 无泛型
来源：http://veh.gotoacloud.top

JS:   // 无泛型
来源：http://nic.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kry.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cvv.birdmap.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pxq.iojbl.cn

Ruby: # 无泛型
来源：http://gwc.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mhu.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://cow.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ihw.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://npt.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zxa.ybcxt.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bjg.hesvh.cn

Java: // 无解构
来源：http://nrc.hywenlv.cn

Go:   // 无解构
来源：http://pqb.andypj.xyz

Ruby: a, b = pair
来源：http://tfy.xinyue.icu

C#:   var (a, b) = pair;
来源：http://etk.yueranfly.top

[C16] 函数 / 方法重载
来源：http://ocw.uphjek.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vpj.xuetiantiany.cn

PHP:  // 无重载
来源：http://zca.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ces.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://ejr.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xpv.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://khc.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://mlb.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://boj.hnqzz.top

================================================================================
来源：http://vdx.nwbrower.top

D. 数组 / 列表 / 集合
来源：http://vkh.fehbvm.com

================================================================================
来源：http://tws.tian-w.cn

[D01] 创建数组 / 列表
来源：http://czk.svipenyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jho.hnqzz.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bjq.fzhhl.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wmt.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mvv.chenlongwang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rpr.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://rvi.hcnkem.com

Ruby: arr = [1, 2, 3]
来源：http://atf.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xme.haohaochexian.top

[D02] 追加元素到末尾
来源：http://wvb.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://exf.kuanghao11.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rda.chenzaomai.com

JS:   arr.push(4);
来源：http://qvu.yuxming.cn

TS:   arr.push(4);
来源：http://cmw.sysykeji.top

Java: list.add(4);
来源：http://hho.nwbrower.top

Go:   arr = append(arr, 4)
来源：http://cwc.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://dkd.svipenyu.cn

C#:   list.Add(4);
来源：http://wqj.tian-w.cn

[D03] 在指定位置插入元素
来源：http://mqs.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://cwz.tarul.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ofd.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://woq.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://fzp.guowangkeji.top

Java: list.add(0, 0);
来源：http://skq.jianghu66.top

Go:   arr = append([]int{0}, arr...)
来源：http://uel.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ntc.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://zmc.chenlongwang.top

[D04] 删除元素
来源：http://xot.redwolf501.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sxq.daxiang520.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iwp.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hua.zhixingplan.top

TS:   arr.splice(0, 1);
来源：http://tzv.fanxiaobao.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://plc.tarul.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pzp.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://evs.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xvz.ppjwa.cn

[D05] 访问与修改元素
来源：http://tgy.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kpx.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ate.316326.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pkd.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://rvd.cqqwz.cn

Java: list.get(0); list.set(0, 9);
来源：http://ktb.vehdjk.com

Go:   arr[0]; arr[0] = 9
来源：http://yhb.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eyj.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ffq.guowangkeji.top

[D06] 数组长度
来源：http://gar.fzhhl.top

Py:   len(arr)
来源：http://gtk.feifeiyinyue.top

PHP:  count($arr);
来源：http://pxk.quarkkingdee.top

JS:   arr.length
来源：http://rbo.xziqi.cn

TS:   arr.length
来源：http://gku.chenlongwang.top

Java: list.size();
来源：http://jcy.jyoumei.cn

Go:   len(arr)
来源：http://czg.fengsongda.top

Ruby: arr.length; arr.size
来源：http://vod.cqqwz.cn

C#:   list.Count;
来源：http://tvh.daria6918.cn

[D07] 切片 / 取子数组
来源：http://hjz.jinghuilouyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rxe.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://yxs.0kj1m.cn

JS:   arr.slice(1, 4);
来源：http://lkz.shanyushiyangtech.top

TS:   arr.slice(1, 4);
来源：http://ztc.smart0.xyz

Java: list.subList(1, 4);
来源：http://yzv.tian-w.cn

Go:   arr[1:4]
来源：http://mha.jianghu66.top

Ruby: arr[1, 3]
来源：http://zpv.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://zju.redwolf501.top

[D08] 合并两个数组
来源：http://byz.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://uno.tarul.cn

PHP:  array_merge($a, $b);
来源：http://wvz.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://ewc.fanxiaobao.xyz

TS:   [...a, ...b];
来源：http://plu.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ana.aibaodan.cn

Go:   append(a, b...)
来源：http://aro.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://szb.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://gdy.jianghu66.top

[D09] 排序（升序）
来源：http://nyf.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://xsi.guannengcc.top

PHP:  sort($arr);
来源：http://thq.chenzaomai.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lvx.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ior.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kiv.aibaodan.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yck.daria6918.cn

Ruby: arr.sort
来源：http://taf.sjlbkw.cn

C#:   list.Sort();
来源：http://zxt.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cuq.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hgf.cdnleiting.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://irk.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vwt.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pcb.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nfg.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ttd.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wzq.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://psw.zhixingplan.top

[D11] 反转数组
来源：http://hxw.shuidangran.top

Py:   arr[::-1];  arr.reverse()
来源：http://pgb.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://yzw.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xyl.yangfankeji.com

TS:   [...arr].reverse();
来源：http://pkx.ydzc1.top

Java: Collections.reverse(list);
来源：http://knl.yangfankeji.com

Go:   slices.Reverse(arr)
来源：http://cbz.tanke756.top

Ruby: arr.reverse
来源：http://ecc.zdbjq.cn

C#:   list.Reverse();
来源：http://yvx.xuanzx.com

[D12] 查找元素下标
来源：http://ctp.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://mof.gaohongyu789.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sve.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://djd.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qyu.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lom.yj20258.top

Go:   slices.Index(arr, x)
来源：http://enr.ybcxt.top

Ruby: arr.index(x)
来源：http://alv.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://sud.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://dao.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://foj.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://whp.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://lrk.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://wkl.xinyue.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ybz.zhaomingkeji.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://who.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://iqk.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jzf.hfpthk.cn

[D14] 映射转换（每个元素变形）
来源：http://pbu.fehbvm.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xbn.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lhs.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://ndu.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://lhq.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://anf.gzhubu.top

Go:   // 手写循环
来源：http://nbv.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jdx.shzxlz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wly.ydjk.org.cn

[D15] 去重
来源：http://xer.iojbl.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sju.ydzc1.top

PHP:  array_unique($arr);
来源：http://oub.kuanghao11.cn

JS:   [...new Set(arr)]
来源：http://gqs.andypj.xyz

TS:   [...new Set(arr)]
来源：http://gwi.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zet.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://fjn.kuanghao11.cn

Ruby: arr.uniq
来源：http://mcx.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://kkm.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://rvp.yfazqb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gcw.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bcu.bbcook.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lgz.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kqm.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cnb.chenjidiqi.icu

Go:   // 手写循环累加
来源：http://ckh.sxryk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pyl.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://pva.epnwcf.com

[D17] 最大值与最小值
来源：http://ayd.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://nko.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://fnw.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cvg.meibo888.top

TS:   Math.max(...arr);
来源：http://xab.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bim.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wck.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://hjj.birdmap.top

C#:   list.Max();  list.Min()
来源：http://nuo.sufxvd.cn

[D18] 扁平化嵌套数组
来源：http://oce.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kfm.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://bnl.jinghuilouyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ngu.sjlbkw.cn

TS:   nested.flat();
来源：http://lfw.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sww.yongpay.top

Go:   // 手写双层循环
来源：http://rvv.aibaodan.cn

Ruby: nested.flatten
来源：http://try.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jra.dianchejie.cn

[D19] 按字段分组
来源：http://dut.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://euf.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://thx.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ffx.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bis.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aqo.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://buo.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vab.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vux.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://bug.nanxuanxn.top

Py:   Counter(arr)
来源：http://phh.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://eyr.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rss.andypj.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lpo.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xlm.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://bpm.hysaishi.cn

Ruby: arr.tally
来源：http://koj.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tsa.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://qbm.mhx1999.top

Py:   x in arr
来源：http://vim.ybcxt.top

PHP:  in_array($x, $arr, true);
来源：http://mse.zhijiandao.cn

JS:   arr.includes(x)
来源：http://iym.andypj.xyz

TS:   arr.includes(x)
来源：http://ipz.zhiwuduotai.top

Java: list.contains(x)
来源：http://whh.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://boa.sufxvd.cn

Ruby: arr.include?(x)
来源：http://hzq.tarul.cn

C#:   list.Contains(x)
来源：http://aft.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://svv.shangyingyoupin.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sms.jinqigfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qhy.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rhe.bjfxy.top

TS:   [...arr];
来源：http://nrw.svipenyu.cn

Java: new ArrayList<>(list);
来源：http://xtx.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://tkx.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://agk.mhx1999.top

C#:   new List<int>(list);
来源：http://fwm.ywan-chungtsiang.top


<!-- 参考信息 -->