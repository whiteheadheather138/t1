代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wjr.sxryk.cn

Go:   return a, b
来源：http://bsk.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://rpx.birdmap.top

C#:   return (a, b);              // ValueTuple
来源：http://zny.gzhubu.top

[C06] 匿名函数 / lambda
来源：http://mqi.tarul.cn

Py:   square = lambda x: x * x
来源：http://nvn.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pla.yueranfly.top

JS:   const square = x => x * x;
来源：http://jcg.jianghu66.top

TS:   const square = (x: number): number => x * x;
来源：http://fku.yanxiufei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iqg.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nwv.redwolf501.top

Ruby: square = ->(x) { x * x }
来源：http://lku.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://tkj.shzxlz.cn

[C07] 把函数作为参数传入
来源：http://kry.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tjt.jinghuilouyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vld.sysykeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://okc.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://bbo.sxryk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://obd.zycfv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ujr.ivvv.top

Ruby: arr.map(&:upcase)
来源：http://gxa.hongshengwenyu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vda.cucudq.cn

[C08] 闭包
来源：http://jxa.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zft.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yzm.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uun.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lhw.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uut.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ybb.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://adi.feifeiyinyue.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://byb.jqgufenzy.top

[C09] 递归
来源：http://yzf.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rdo.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lqt.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uqn.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ddt.yongpay.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uwx.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qgh.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://niu.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cyg.gaohongyu789.top

[C10] 变量作用域
来源：http://cnw.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dwk.dashuyun.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pel.iojbl.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yxb.shzxlz.cn

TS:   同 JS
来源：http://kuw.nanxinkj.top

Java: 方法内为块级作用域
来源：http://cki.tanke756.top

Go:   花括号块级作用域
来源：http://xjb.gogol.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dpq.0kj1m.cn

C#:   块级作用域
来源：http://zls.guowangkeji.top

[C11] 模块导入与导出
来源：http://fqm.mhx1999.top

Py:   from module import func
来源：http://khj.yangfankeji.com

PHP:  require "file.php";  或 use App\Service;
来源：http://cmp.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tbs.guannengcc.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gnc.yvedp.cn

Java: import java.util.List;
来源：http://rht.52xcode.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bmx.chenlongwang.top

Ruby: require "json"; require_relative "./util"
来源：http://eng.xziqi.cn

C#:   using System.Text;
来源：http://lmg.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://jup.guowangkeji.top

Py:   (lambda: print("run"))()
来源：http://mlq.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://bqq.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://rfi.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://mab.bbcook.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rso.cucudq.cn

Go:   func() { fmt.Println("run") }()
来源：http://kbv.316326.xyz

Ruby: -> { puts "run" }.call
来源：http://uvf.dianchejie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sfu.tarul.cn

[C13] 类型声明 / 类型注解
来源：http://wqy.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://byz.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rne.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ouu.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jme.haohaochexian.top

Java: int add(int a, int b) { return a + b; }
来源：http://sfl.yj202588.top

Go:   func add(a, b int) int
来源：http://xzp.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mdj.shzxlz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uvo.yuanzhike.top

[C14] 泛型函数
来源：http://swm.ywan-chungtsiang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://flb.cheryme.top

PHP:  // 无泛型
来源：http://qmf.guowangkeji.top

JS:   // 无泛型
来源：http://daj.jiagoushi.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eie.tian-w.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gwu.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ufl.ydjk.org.cn

Ruby: # 无泛型
来源：http://jww.shanyushiyangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cgh.ybcxt.top

[C15] 解构 / 展开参数
来源：http://nqs.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://agh.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://jyd.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nno.hcnkem.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qni.sysykeji.top

Java: // 无解构
来源：http://hkk.cdnleiting.top

Go:   // 无解构
来源：http://wxh.epnwcf.com

Ruby: a, b = pair
来源：http://gho.sxryk.cn

C#:   var (a, b) = pair;
来源：http://bts.xziqi.cn

[C16] 函数 / 方法重载
来源：http://msd.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://czu.hfpthk.cn

PHP:  // 无重载
来源：http://njp.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pif.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://voc.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vas.tarul.cn

Go:   // 无重载：用不同函数名
来源：http://jod.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://ccm.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hat.sweek.top

================================================================================
来源：http://wfb.kuanghao11.cn

D. 数组 / 列表 / 集合
来源：http://xwp.guowangkeji.top

================================================================================
来源：http://stn.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://zxt.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://evm.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fih.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lil.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dao.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://efj.fzhhl.top

Go:   arr := []int{1, 2, 3}
来源：http://eyf.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://zel.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ied.aibaodan.cn

[D02] 追加元素到末尾
来源：http://yox.yonumen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sms.9152youxi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ahs.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://erd.jyoumei.cn

TS:   arr.push(4);
来源：http://agi.ctjpmb.com

Java: list.add(4);
来源：http://wrz.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://avf.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://usn.zhengqikj.top

C#:   list.Add(4);
来源：http://ixv.xylfe.cn

[D03] 在指定位置插入元素
来源：http://cfa.zycfv.cn

Py:   arr.insert(0, 0)
来源：http://icl.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ute.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tju.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://xpn.daxiang520.top

Java: list.add(0, 0);
来源：http://cgx.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://pnv.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bib.zhixingplan.top

C#:   list.Insert(0, 0);
来源：http://ira.gogol.net.cn

[D04] 删除元素
来源：http://wqr.yj20258.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://shm.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vtb.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fzb.ivvv.top

TS:   arr.splice(0, 1);
来源：http://jav.yj20258.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qdd.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yjf.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://beb.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xpr.hysaishi.cn

[D05] 访问与修改元素
来源：http://gzu.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iam.tarul.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kgm.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rfx.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://chr.hnxiangtu.top

Java: list.get(0); list.set(0, 9);
来源：http://hlx.uphjek.com

Go:   arr[0]; arr[0] = 9
来源：http://gos.shuidangran.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nne.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mje.sweek.top

[D06] 数组长度
来源：http://zys.vehdjk.com

Py:   len(arr)
来源：http://qlw.nanxuanxn.top

PHP:  count($arr);
来源：http://fdj.hcnkem.com

JS:   arr.length
来源：http://udh.0kj1m.cn

TS:   arr.length
来源：http://oaq.316326.xyz

Java: list.size();
来源：http://ynw.hnxiangtu.top

Go:   len(arr)
来源：http://plq.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://jol.birdmap.top

C#:   list.Count;
来源：http://vxm.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://xea.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hts.haohaochexian.top

PHP:  array_slice($arr, 1, 3);
来源：http://ywe.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://fiv.pycfn.com

TS:   arr.slice(1, 4);
来源：http://dfx.nanxuanxn.top

Java: list.subList(1, 4);
来源：http://ojl.jyoumei.cn

Go:   arr[1:4]
来源：http://tfs.wangdashe.top

Ruby: arr[1, 3]
来源：http://lql.shangyingyoupin.top

C#:   list.GetRange(1, 3);
来源：http://lzy.gaohongyu789.top

[D08] 合并两个数组
来源：http://vgi.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://hib.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://zlc.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://szx.hesvh.cn

TS:   [...a, ...b];
来源：http://mte.hfpthk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://okr.zdqjudy.top

Go:   append(a, b...)
来源：http://cci.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://fdr.yuanzhike.top

C#:   a.Concat(b).ToList()
来源：http://puv.yj202588.top

[D09] 排序（升序）
来源：http://cex.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://wqt.guowangkeji.top

PHP:  sort($arr);
来源：http://fxi.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://snt.ybcxt.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ndi.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vgn.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ubz.chenjidiqi.icu

Ruby: arr.sort
来源：http://ajs.gotoacloud.top

C#:   list.Sort();
来源：http://bix.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fmm.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ybn.yonumen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oog.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://glx.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hzf.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://llf.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kkq.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://csv.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hyd.xylfe.cn

[D11] 反转数组
来源：http://lir.xziqi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uoe.tanke756.top

PHP:  array_reverse($arr);
来源：http://zuk.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wjr.uphjek.com

TS:   [...arr].reverse();
来源：http://bfw.yvedp.cn

Java: Collections.reverse(list);
来源：http://pwe.yanxiufei.cn

Go:   slices.Reverse(arr)
来源：http://apv.sjlbkw.cn

Ruby: arr.reverse
来源：http://tmp.yj20258.top

C#:   list.Reverse();
来源：http://htm.ydzc1.top

[D12] 查找元素下标
来源：http://lpt.yuanzhike.top

Py:   arr.index(x);  x in arr
来源：http://gnw.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qzg.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hfv.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xck.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bac.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://qfo.jianghu66.top

Ruby: arr.index(x)
来源：http://atu.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://ekg.yj20258.top

[D13] 过滤（保留满足条件的）
来源：http://nhk.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xgc.dianchejie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mcq.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://dxd.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://vkq.wangshuangyany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://unf.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tig.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://vze.hywenlv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uwe.zhengqikj.top

[D14] 映射转换（每个元素变形）
来源：http://lxe.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hor.yanxiufei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pxp.xinyue.icu

JS:   arr.map(x => x * 2)
来源：http://mwc.9152youxi.cn

TS:   arr.map(x => x * 2)
来源：http://ibc.yueranfly.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lxw.aibaodan.cn

Go:   // 手写循环
来源：http://gbv.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://den.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://rfo.pengpengdd.cyou

[D15] 去重
来源：http://suo.sjlbkw.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ysb.sufxvd.cn

PHP:  array_unique($arr);
来源：http://vbi.xylfe.cn

JS:   [...new Set(arr)]
来源：http://bdc.shuidangran.top

TS:   [...new Set(arr)]
来源：http://ttt.shuidangran.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wym.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://trn.xylfe.cn

Ruby: arr.uniq
来源：http://tot.ctjpmb.com

C#:   list.Distinct().ToList()
来源：http://qvu.yanxiufei.cn

[D16] 求和与平均值
来源：http://pbv.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zca.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fpy.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xjy.snrcjt.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dav.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yyz.c1oappe.top

Go:   // 手写循环累加
来源：http://ygp.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://web.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://xjo.andypj.xyz

[D17] 最大值与最小值
来源：http://mbt.guowangkeji.top

Py:   max(arr);  min(arr)
来源：http://sxo.yvedp.cn

PHP:  max($arr);  min($arr);
来源：http://zru.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ggy.9152youxi.cn

TS:   Math.max(...arr);
来源：http://fek.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://udf.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jeo.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://wyy.tarul.cn

C#:   list.Max();  list.Min()
来源：http://joy.cheryme.top

[D18] 扁平化嵌套数组
来源：http://omh.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kap.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://nza.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dix.daxiang520.top

TS:   nested.flat();
来源：http://ixy.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pzu.nanxinkj.top

Go:   // 手写双层循环
来源：http://wiv.zhiwuduotai.top

Ruby: nested.flatten
来源：http://toq.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://soz.tian-w.cn

[D19] 按字段分组
来源：http://lxj.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bra.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ndi.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://swr.fzhhl.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nbm.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bou.havefunace.top

Go:   // 手写 map[string][]T
来源：http://yaz.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://alc.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hiy.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://aaa.ehwqpu.com

Py:   Counter(arr)
来源：http://unb.yonumen.top

PHP:  array_count_values($arr);
来源：http://mly.vehdjk.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rho.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://czf.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fvn.pycfn.com

Go:   // 手写 map[T]int
来源：http://mhg.fanxiaobao.xyz

Ruby: arr.tally
来源：http://nel.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fdc.zhijiandao.cn

[D21] 判断是否包含某元素
来源：http://ohk.jqgufenzy.top

Py:   x in arr
来源：http://iyy.316326.xyz

PHP:  in_array($x, $arr, true);
来源：http://qvj.zdbjq.cn

JS:   arr.includes(x)
来源：http://iqk.vqdsnc.cn

TS:   arr.includes(x)
来源：http://efk.yuxming.cn

Java: list.contains(x)
来源：http://ryu.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://myp.sufxvd.cn

Ruby: arr.include?(x)
来源：http://ihe.hfpthk.cn

C#:   list.Contains(x)
来源：http://yge.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://kbn.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nbp.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hyf.zdqjudy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://teu.dashuyun.cn

TS:   [...arr];
来源：http://bew.dashuyun.cn


<!-- 参考信息 -->