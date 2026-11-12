代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ugv.cucudq.cn

TS:   arr.map(String)
来源：http://kef.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bjy.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hbn.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://yxw.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://upy.guowangkeji.top

[C08] 闭包
来源：http://pri.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wwd.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oeh.aibaodan.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://off.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yjn.ctjpmb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ddo.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gnt.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bjh.ppjwa.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pbg.pengpengdd.cyou

[C09] 递归
来源：http://vhj.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dui.xziqi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rzl.xuanzx.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wzq.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kld.xinyue.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bbj.zhongyouzk.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mcn.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rcq.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uer.hcnkem.com

[C10] 变量作用域
来源：http://mjc.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wrd.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rkf.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uxx.fengsongda.top

TS:   同 JS
来源：http://fff.nwbrower.top

Java: 方法内为块级作用域
来源：http://fzo.ydzc1.top

Go:   花括号块级作用域
来源：http://sgt.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://edn.jinyuanbaomall.cn

C#:   块级作用域
来源：http://slj.c1oappe.top

[C11] 模块导入与导出
来源：http://zfr.andypj.xyz

Py:   from module import func
来源：http://msh.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yhh.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://oqq.hcnkem.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tzf.ctjpmb.com

Java: import java.util.List;
来源：http://bbh.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yhj.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://pbc.fengsongda.top

C#:   using System.Text;
来源：http://zwu.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://wtx.hysaishi.cn

Py:   (lambda: print("run"))()
来源：http://gpo.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://dba.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://xmz.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://icw.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rtw.cheryme.top

Go:   func() { fmt.Println("run") }()
来源：http://tux.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://ryc.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bxi.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://fcz.iojbl.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lnp.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rcf.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lpk.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xgu.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xjx.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://unm.jinghuilouyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://usx.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://drl.xinyue.icu

[C14] 泛型函数
来源：http://srt.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://evj.jqgufenzy.top

PHP:  // 无泛型
来源：http://ecd.jinqigfzy.top

JS:   // 无泛型
来源：http://oat.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zax.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pqu.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dxw.guannengcc.top

Ruby: # 无泛型
来源：http://vfn.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ojq.wangdashe.top

[C15] 解构 / 展开参数
来源：http://rae.xylfe.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lhu.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://jhr.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://udv.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xqc.yuxming.cn

Java: // 无解构
来源：http://usw.guannengcc.top

Go:   // 无解构
来源：http://txg.hcnkem.com

Ruby: a, b = pair
来源：http://mbp.mhx1999.top

C#:   var (a, b) = pair;
来源：http://lea.hongshengwenyu.top

[C16] 函数 / 方法重载
来源：http://wzs.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mya.ehwqpu.com

PHP:  // 无重载
来源：http://ctp.yj20258.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rty.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://fme.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://sbl.jinqigufen.top

Go:   // 无重载：用不同函数名
来源：http://tpx.9152youxi.cn

Ruby: # 无重载：靠动态参数
来源：http://vza.wangshuangyany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bko.quarkkingdee.top

================================================================================
来源：http://ywd.jinghuilouyu.cn

D. 数组 / 列表 / 集合
来源：http://sej.sufxvd.cn

================================================================================
来源：http://nwu.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://dbe.wangshuangyany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tca.zhixingplan.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cqp.hongshengwenyu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yxi.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qpg.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zge.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://ffj.haohaochexian.top

Ruby: arr = [1, 2, 3]
来源：http://uop.wangshuangyany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eno.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://qtu.52xcode.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lsu.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xxb.kuanghao11.cn

JS:   arr.push(4);
来源：http://bxa.yvedp.cn

TS:   arr.push(4);
来源：http://gqz.yvedp.cn

Java: list.add(4);
来源：http://dfn.jianghu66.top

Go:   arr = append(arr, 4)
来源：http://rgl.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://veo.epnwcf.com

C#:   list.Add(4);
来源：http://mul.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://piu.zhengqikj.top

Py:   arr.insert(0, 0)
来源：http://acu.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ujz.sweek.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bvi.sxryk.cn

TS:   arr.splice(0, 0, 0);
来源：http://mfc.fanxiaobao.xyz

Java: list.add(0, 0);
来源：http://nre.jianghu66.top

Go:   arr = append([]int{0}, arr...)
来源：http://wzu.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://afo.fehbvm.com

C#:   list.Insert(0, 0);
来源：http://ljx.jiagoushi.top

[D04] 删除元素
来源：http://wre.xuetiantiany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dne.epnwcf.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bvo.gaohongyu789.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oxd.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://sva.fanxiaobao.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ngn.sufxvd.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mky.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ego.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oep.tianlin.xyz

[D05] 访问与修改元素
来源：http://jvk.chenzaomai.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mxf.jqgufenzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hqm.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hbz.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://fhq.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://xgq.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://spe.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jsl.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://shw.xylfe.cn

[D06] 数组长度
来源：http://vsm.wangdashe.top

Py:   len(arr)
来源：http://hyn.haohaochexian.top

PHP:  count($arr);
来源：http://bql.xziqi.cn

JS:   arr.length
来源：http://lid.tarul.cn

TS:   arr.length
来源：http://udv.yuxming.cn

Java: list.size();
来源：http://thj.guannengcc.top

Go:   len(arr)
来源：http://qyp.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://ukl.0kj1m.cn

C#:   list.Count;
来源：http://rnm.sweek.top

[D07] 切片 / 取子数组
来源：http://xli.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zgy.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rdw.meibo888.top

JS:   arr.slice(1, 4);
来源：http://nmi.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://hpd.guowangkeji.top

Java: list.subList(1, 4);
来源：http://fjk.feifeiyinyue.top

Go:   arr[1:4]
来源：http://nuq.bbcook.cn

Ruby: arr[1, 3]
来源：http://xfh.birdmap.top

C#:   list.GetRange(1, 3);
来源：http://uqn.chenjidiqi.icu

[D08] 合并两个数组
来源：http://mdp.sysykeji.top

Py:   a + b;  a.extend(b)
来源：http://vjm.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://bkm.mhx1999.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vkg.hnqzz.top

TS:   [...a, ...b];
来源：http://udy.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yop.mhx1999.top

Go:   append(a, b...)
来源：http://emy.yonumen.top

Ruby: a + b;  a.concat(b)
来源：http://tec.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://tup.ivvv.top

[D09] 排序（升序）
来源：http://qle.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://szo.0kj1m.cn

PHP:  sort($arr);
来源：http://tgx.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://llp.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://obn.xuanzx.com

Java: Collections.sort(list);  list.sort(null);
来源：http://khu.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hcv.pengpengdd.cyou

Ruby: arr.sort
来源：http://mef.xuetiantiany.cn

C#:   list.Sort();
来源：http://ehy.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tie.aizwys.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oyx.cqqwz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://prr.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zkf.9152youxi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lwp.kuanghao11.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xzw.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ueq.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kik.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://faj.uphjek.com

[D11] 反转数组
来源：http://gtl.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://mnf.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://zyp.wangshuangyany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rji.shuidangran.top

TS:   [...arr].reverse();
来源：http://dga.jqgfzy.top

Java: Collections.reverse(list);
来源：http://rfj.vqdsnc.cn

Go:   slices.Reverse(arr)
来源：http://aau.redwolf501.top

Ruby: arr.reverse
来源：http://tsr.jlsjyb.cn

C#:   list.Reverse();
来源：http://gpy.daria6918.cn

[D12] 查找元素下标
来源：http://xfu.gogol.net.cn

Py:   arr.index(x);  x in arr
来源：http://ngq.cqqwz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gcz.sweek.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gfb.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uwa.yj20258888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zdf.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://gyz.yangfankeji.com

Ruby: arr.index(x)
来源：http://akl.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://ndl.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://zaz.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kgq.jianghu66.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cuv.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://yxx.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://kvr.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qmw.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rnz.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://eea.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bdm.zhixingplan.top

[D14] 映射转换（每个元素变形）
来源：http://bzg.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lbm.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bea.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://qhz.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://lvk.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bdg.yfazqb.com

Go:   // 手写循环
来源：http://ryp.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://lar.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://guv.kuanghao11.cn

[D15] 去重
来源：http://vdl.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://seh.sxryk.cn

PHP:  array_unique($arr);
来源：http://fop.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://pay.bjfxy.top

TS:   [...new Set(arr)]
来源：http://ulp.zycfv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yrr.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nav.ctjpmb.com

Ruby: arr.uniq
来源：http://jkr.hnxiangtu.top

C#:   list.Distinct().ToList()
来源：http://ilc.52xcode.cn

[D16] 求和与平均值
来源：http://fnm.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zgz.aibaodan.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jqd.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dbb.snrcjt.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pas.havefunace.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iiy.yfazqb.com

Go:   // 手写循环累加
来源：http://ghe.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iah.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://bzr.yangfankeji.com

[D17] 最大值与最小值
来源：http://bbj.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://ajx.fehbvm.com

PHP:  max($arr);  min($arr);
来源：http://ext.hesvh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://osv.sysykeji.top

TS:   Math.max(...arr);
来源：http://lqe.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://sjv.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://agk.gogol.net.cn

Ruby: arr.max;  arr.min
来源：http://ecq.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://nwh.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://vro.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xog.jianghu66.top

PHP:  array_merge(...$nested);
来源：http://htl.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dwh.nanxuanxn.top

TS:   nested.flat();
来源：http://zfr.guannengcc.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hyp.yj202588.top

Go:   // 手写双层循环
来源：http://qjm.aibaodan.cn

Ruby: nested.flatten
来源：http://vjs.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pys.dashuyun.cn

[D19] 按字段分组
来源：http://xoi.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tzj.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://caa.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kuo.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://rrr.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lgu.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://cvv.jinghuilouyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uym.kuanghao11.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yra.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://wok.yj20258.top

Py:   Counter(arr)
来源：http://ojv.vehdjk.com

PHP:  array_count_values($arr);
来源：http://wtd.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pgz.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ghv.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zpy.xuanzx.com

Go:   // 手写 map[T]int
来源：http://cny.zhiwuduotai.top

Ruby: arr.tally
来源：http://gqw.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nju.tarul.cn

[D21] 判断是否包含某元素
来源：http://cra.hnxiangtu.top

Py:   x in arr
来源：http://rzb.chenjidiqi.icu

PHP:  in_array($x, $arr, true);
来源：http://mks.svipenyu.cn

JS:   arr.includes(x)
来源：http://eqx.yvedp.cn

TS:   arr.includes(x)
来源：http://dkl.hysaishi.cn

Java: list.contains(x)
来源：http://spn.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://neq.aibaodan.cn

Ruby: arr.include?(x)
来源：http://hww.yj202588.top

C#:   list.Contains(x)
来源：http://zlc.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://erg.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ndq.yj202588.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tmd.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://efq.cucudq.cn

TS:   [...arr];
来源：http://vkw.xziqi.cn

Java: new ArrayList<>(list);
来源：http://xdo.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://vmj.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://icp.iojbl.cn

C#:   new List<int>(list);
来源：http://odj.tian-w.cn

[D23] reduce 累积计算
来源：http://rpn.chenzaomai.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aeo.kuanghao11.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qrm.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iuc.yongpay.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ice.cqqwz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qwv.0kj1m.cn

Go:   // 手写循环
来源：http://esn.c1oappe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mpd.zhaomingkeji.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lbd.feifeiyinyue.top

[D24] 字典 / Map 基本操作
来源：http://enn.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://brm.sweek.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://umc.ivvv.top


<!-- 参考信息 -->