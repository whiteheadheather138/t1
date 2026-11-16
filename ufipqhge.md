代发 wailian999

[C06] 匿名函数 / lambda
来源：http://xyo.shanyushiyangtech.top

Py:   square = lambda x: x * x
来源：http://vxf.jinqigfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vxn.hywenlv.cn

JS:   const square = x => x * x;
来源：http://jug.jianghu66.top

TS:   const square = (x: number): number => x * x;
来源：http://vqu.sufxvd.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://drd.hfpthk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rkh.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://szk.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://ylm.ppjwa.cn

[C07] 把函数作为参数传入
来源：http://xtv.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ffi.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ucg.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://byk.yueranfly.top

TS:   arr.map(String)
来源：http://mew.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jcq.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dhw.tian-w.cn

Ruby: arr.map(&:upcase)
来源：http://yhb.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kqk.yangfankeji.com

[C08] 闭包
来源：http://wjr.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rqa.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://suq.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lic.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dic.52xcode.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ijd.snrcjt.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vlg.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xns.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qau.cheryme.top

[C09] 递归
来源：http://nil.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zmv.guannengcc.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uot.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ldr.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://scj.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lhb.uphjek.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qpz.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hpo.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tci.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://dbf.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rzx.hnxiangtu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://joi.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cby.zycfv.cn

TS:   同 JS
来源：http://taj.hcnkem.com

Java: 方法内为块级作用域
来源：http://bds.fengsongda.top

Go:   花括号块级作用域
来源：http://kut.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xox.jinqigfzy.top

C#:   块级作用域
来源：http://ipi.cqqwz.cn

[C11] 模块导入与导出
来源：http://nkj.bbcook.cn

Py:   from module import func
来源：http://mfx.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://giw.cashguo.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kql.zhaomingkeji.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ocu.quarkkingdee.top

Java: import java.util.List;
来源：http://bwn.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pcb.52xcode.cn

Ruby: require "json"; require_relative "./util"
来源：http://dsn.zhengqikj.top

C#:   using System.Text;
来源：http://sng.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://rfu.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://suj.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://wgm.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://xff.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://tlk.shzxlz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nct.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://rdd.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://iye.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kje.jinghuilouyu.cn

[C13] 类型声明 / 类型注解
来源：http://adt.hammf.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hgx.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://buv.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ctn.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ona.jianghu66.top

Java: int add(int a, int b) { return a + b; }
来源：http://gwm.jyoumei.cn

Go:   func add(a, b int) int
来源：http://iku.nanxinkj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://htc.jqgufenzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://hua.ybcxt.top

[C14] 泛型函数
来源：http://luc.chenzaomai.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oso.c1oappe.top

PHP:  // 无泛型
来源：http://bcc.gzhubu.top

JS:   // 无泛型
来源：http://ait.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fzw.zhijiandao.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eqj.316326.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fob.tanke756.top

Ruby: # 无泛型
来源：http://fkx.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lcb.zhengqikj.top

[C15] 解构 / 展开参数
来源：http://bgr.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kob.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://wnb.zhaomingkeji.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://esx.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vit.zhiwuduotai.top

Java: // 无解构
来源：http://ffg.ydzc1.top

Go:   // 无解构
来源：http://ibb.chenlongwang.top

Ruby: a, b = pair
来源：http://ujz.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://ero.52xcode.cn

[C16] 函数 / 方法重载
来源：http://xlk.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mue.zhixingplan.top

PHP:  // 无重载
来源：http://hqc.pengpengdd.cyou

JS:   // 无重载：靠 arguments.length 分支
来源：http://suk.yuanzhike.top

TS:   // 用联合类型或重载签名声明
来源：http://xwm.daxiang520.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rie.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://syt.shangyingyoupin.top

Ruby: # 无重载：靠动态参数
来源：http://oqr.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xtc.uphjek.com

================================================================================
来源：http://lxr.andypj.xyz

D. 数组 / 列表 / 集合
来源：http://rix.yfazqb.com

================================================================================
来源：http://keh.havefunace.top

[D01] 创建数组 / 列表
来源：http://dix.hywenlv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rex.cucudq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ueq.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kkz.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yte.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zce.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://anl.hesvh.cn

Ruby: arr = [1, 2, 3]
来源：http://mdw.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dhq.ybcxt.top

[D02] 追加元素到末尾
来源：http://oom.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eaf.52xcode.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mas.fengsongda.top

JS:   arr.push(4);
来源：http://vwz.sweek.top

TS:   arr.push(4);
来源：http://vca.0kj1m.cn

Java: list.add(4);
来源：http://itx.sufxvd.cn

Go:   arr = append(arr, 4)
来源：http://xpk.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://ngh.gzhubu.top

C#:   list.Add(4);
来源：http://clz.yangfankeji.com

[D03] 在指定位置插入元素
来源：http://swb.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://wyw.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vll.jinqigufen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dzr.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://jol.nanxinkj.top

Java: list.add(0, 0);
来源：http://kjt.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://obg.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xou.wangshuangyany.cn

C#:   list.Insert(0, 0);
来源：http://yzk.cdnleiting.top

[D04] 删除元素
来源：http://mgs.nanxinkj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zen.bbcook.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://odz.meibo888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cle.cheryme.top

TS:   arr.splice(0, 1);
来源：http://rvp.hfpthk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iyc.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jmj.yj20258.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pww.jiagoushi.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lhf.ydzc1.top

[D05] 访问与修改元素
来源：http://plz.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bhj.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://adf.xinyue.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pzs.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://ymu.sjlbkw.cn

Java: list.get(0); list.set(0, 9);
来源：http://cwi.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://kpq.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dko.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://axs.yuxming.cn

[D06] 数组长度
来源：http://avv.jlsjyb.cn

Py:   len(arr)
来源：http://pgg.sxryk.cn

PHP:  count($arr);
来源：http://wxe.xziqi.cn

JS:   arr.length
来源：http://tcs.pengpengdd.cyou

TS:   arr.length
来源：http://ska.zdqjudy.top

Java: list.size();
来源：http://cfp.tianlin.xyz

Go:   len(arr)
来源：http://ejy.daxiang520.top

Ruby: arr.length; arr.size
来源：http://dtr.jiagoushi.top

C#:   list.Count;
来源：http://juj.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://xvf.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zyt.aizwys.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ssy.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://tch.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://rdd.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://epq.fengsongda.top

Go:   arr[1:4]
来源：http://enf.fzhhl.top

Ruby: arr[1, 3]
来源：http://igc.yuxming.cn

C#:   list.GetRange(1, 3);
来源：http://vmt.tanke756.top

[D08] 合并两个数组
来源：http://eej.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://tpq.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://vxx.yj20258.top

JS:   [...a, ...b];  a.concat(b);
来源：http://oxs.daxiang520.top

TS:   [...a, ...b];
来源：http://odx.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aoj.tian-w.cn

Go:   append(a, b...)
来源：http://rrb.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://seq.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://woo.hnqzz.top

[D09] 排序（升序）
来源：http://lyz.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://cej.zhijiandao.cn

PHP:  sort($arr);
来源：http://mnm.yuxming.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://umv.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dfs.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://roi.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mld.gaohongyu789.top

Ruby: arr.sort
来源：http://nzi.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://qkk.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://mfi.zhiwuduotai.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qpx.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://swy.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mus.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ooe.xinyue.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nnp.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tsr.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dlk.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wvz.yj20258888.top

[D11] 反转数组
来源：http://coq.yangfankeji.com

Py:   arr[::-1];  arr.reverse()
来源：http://oid.xziqi.cn

PHP:  array_reverse($arr);
来源：http://yfp.tarul.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mbq.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://gqf.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://mdo.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://znt.hnxiangtu.top

Ruby: arr.reverse
来源：http://vgo.316326.xyz

C#:   list.Reverse();
来源：http://myf.kuanghao11.cn

[D12] 查找元素下标
来源：http://hil.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://vge.fktsv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yym.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pap.hammf.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://csc.feifeiyinyue.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iza.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://hkf.cashguo.top

Ruby: arr.index(x)
来源：http://wed.xylfe.cn

C#:   list.IndexOf(x);
来源：http://iht.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://fhv.vqdsnc.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qjg.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zkx.sjlbkw.cn

JS:   arr.filter(x => x > 3)
来源：http://sdi.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://tbo.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fmd.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xyj.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tjx.wangdashe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://txe.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://upx.316326.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zaa.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ond.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://zgc.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://vxm.nanxuanxn.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bdm.quarkkingdee.top

Go:   // 手写循环
来源：http://uzq.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mzt.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rtd.shzxlz.cn

[D15] 去重
来源：http://njv.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vku.havefunace.top

PHP:  array_unique($arr);
来源：http://tye.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://pqu.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://tlz.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rir.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://piy.jianghu66.top

Ruby: arr.uniq
来源：http://xia.cheryme.top

C#:   list.Distinct().ToList()
来源：http://ciz.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://fzo.shanyushiyangtech.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hya.jyoumei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://phf.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lyu.zhaomingkeji.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mwn.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://voa.tarul.cn

Go:   // 手写循环累加
来源：http://zys.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://drs.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://kxe.xuanzx.com

[D17] 最大值与最小值
来源：http://irs.yanxiufei.cn

Py:   max(arr);  min(arr)
来源：http://mzz.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://abk.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rfj.yj20258888.top

TS:   Math.max(...arr);
来源：http://dmq.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rkh.birdmap.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qan.316326.xyz

Ruby: arr.max;  arr.min
来源：http://ily.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://rbu.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://sys.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nxh.bjfxy.top

PHP:  array_merge(...$nested);
来源：http://arh.sxryk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bla.fengsongda.top

TS:   nested.flat();
来源：http://qmo.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kmk.gogol.net.cn

Go:   // 手写双层循环
来源：http://wrj.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://bli.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://qur.kuanghao11.cn

[D19] 按字段分组
来源：http://elc.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oxe.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wiy.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gko.jiagoushi.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ykt.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://whw.cdnleiting.top

Go:   // 手写 map[string][]T
来源：http://iro.quarkkingdee.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://akb.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://izn.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://tzo.hysaishi.cn

Py:   Counter(arr)
来源：http://fcf.hnxiangtu.top

PHP:  array_count_values($arr);
来源：http://vhq.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mdp.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rzl.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gma.ivvv.top

Go:   // 手写 map[T]int
来源：http://lot.52xcode.cn

Ruby: arr.tally
来源：http://phc.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jtk.yangfankeji.com

[D21] 判断是否包含某元素
来源：http://don.316326.xyz

Py:   x in arr
来源：http://mbr.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://mtl.wangdashe.top

JS:   arr.includes(x)
来源：http://rpv.hnxiangtu.top

TS:   arr.includes(x)
来源：http://dnm.sjlbkw.cn

Java: list.contains(x)
来源：http://wck.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://mdv.tarul.cn

Ruby: arr.include?(x)
来源：http://dmu.nanxuanxn.top

C#:   list.Contains(x)
来源：http://hdk.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://tsa.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://phg.cdnleiting.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hdn.ybcxt.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dvn.fktsv.cn

TS:   [...arr];
来源：http://aod.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://wel.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ukq.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://new.xuetiantiany.cn

C#:   new List<int>(list);
来源：http://aak.jinghuilouyu.cn


<!-- 参考信息 -->