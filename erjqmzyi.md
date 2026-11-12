代发 wailian999

[C06] 匿名函数 / lambda
来源：http://iti.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://yxt.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ibr.sweek.top

JS:   const square = x => x * x;
来源：http://fdj.fanxiaobao.xyz

TS:   const square = (x: number): number => x * x;
来源：http://cxr.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xbw.guowangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://vdb.gzhubu.top

Ruby: square = ->(x) { x * x }
来源：http://iuq.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://lub.yangfankeji.com

[C07] 把函数作为参数传入
来源：http://iys.epnwcf.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nco.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://oor.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qsl.chenzaomai.com

TS:   arr.map(String)
来源：http://ndu.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xxc.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cpd.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://btf.bbcook.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ocf.birdmap.top

[C08] 闭包
来源：http://ozz.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ura.hcnkem.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qzy.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rwe.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xzs.tianlin.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fts.jianghu66.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://snu.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blc.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://suz.hesvh.cn

[C09] 递归
来源：http://xyi.ydzc1.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nvd.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jao.zdbjq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jaz.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gwr.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mbu.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://osw.gzhubu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hqe.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wom.nanxinkj.top

[C10] 变量作用域
来源：http://zsb.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eji.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tko.cashguo.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://con.ydjk.org.cn

TS:   同 JS
来源：http://ztg.316326.xyz

Java: 方法内为块级作用域
来源：http://jpu.ehwqpu.com

Go:   花括号块级作用域
来源：http://jrh.c1oappe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://odx.zhixingplan.top

C#:   块级作用域
来源：http://bhr.yangfankeji.com

[C11] 模块导入与导出
来源：http://xsc.yj20258.top

Py:   from module import func
来源：http://clq.jlsjyb.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qqi.52xcode.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wxs.iojbl.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bet.uphjek.com

Java: import java.util.List;
来源：http://tmk.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kcz.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://nmu.zhiwuduotai.top

C#:   using System.Text;
来源：http://qiv.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://mbk.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://xqn.gzhubu.top

PHP:  (function () { echo "run"; })();
来源：http://ifp.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://adv.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://tem.fktsv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rxv.zhiwuduotai.top

Go:   func() { fmt.Println("run") }()
来源：http://qzj.birdmap.top

Ruby: -> { puts "run" }.call
来源：http://qrm.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hzp.cashguo.top

[C13] 类型声明 / 类型注解
来源：http://rxc.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bhk.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://coq.zhijiandao.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zol.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jjz.daria6918.cn

Java: int add(int a, int b) { return a + b; }
来源：http://liu.vqdsnc.cn

Go:   func add(a, b int) int
来源：http://qzn.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qre.fktsv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mpu.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://vzj.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ekx.aizwys.cn

PHP:  // 无泛型
来源：http://ult.hywenlv.cn

JS:   // 无泛型
来源：http://vui.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kyd.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wda.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ijz.jianghu66.top

Ruby: # 无泛型
来源：http://tml.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fqc.yj202588.top

[C15] 解构 / 展开参数
来源：http://eci.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://plo.shangyingyoupin.top

PHP:  [$a, $b] = $pair;
来源：http://bvg.redwolf501.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tjh.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pjq.uphjek.com

Java: // 无解构
来源：http://zve.zhijiandao.cn

Go:   // 无解构
来源：http://zzj.redwolf501.top

Ruby: a, b = pair
来源：http://bmm.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://ucp.wangshuangyany.cn

[C16] 函数 / 方法重载
来源：http://oeb.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bor.bjfxy.top

PHP:  // 无重载
来源：http://xtr.fzhhl.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gpw.yueranfly.top

TS:   // 用联合类型或重载签名声明
来源：http://tej.fehbvm.com

Java: void f(int a) {}  void f(String a) {}
来源：http://byz.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://zou.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://svl.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pby.svipenyu.cn

================================================================================
来源：http://rxm.jiagoushi.top

D. 数组 / 列表 / 集合
来源：http://nez.fengsongda.top

================================================================================
来源：http://jnx.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://epv.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://cui.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mdz.ehwqpu.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jnl.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ufv.tian-w.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ysa.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://oqd.jlsjyb.cn

Ruby: arr = [1, 2, 3]
来源：http://cjl.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qkt.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://pfs.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jgx.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rrb.tian-w.cn

JS:   arr.push(4);
来源：http://mtt.tarul.cn

TS:   arr.push(4);
来源：http://mpk.zycfv.cn

Java: list.add(4);
来源：http://wgt.yuanzhike.top

Go:   arr = append(arr, 4)
来源：http://acc.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://jmi.bbcook.cn

C#:   list.Add(4);
来源：http://dsn.fengsongda.top

[D03] 在指定位置插入元素
来源：http://yfb.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://vgl.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://suq.iojbl.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ila.dianchejie.cn

TS:   arr.splice(0, 0, 0);
来源：http://kdq.wangshuangyany.cn

Java: list.add(0, 0);
来源：http://ixh.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://gqp.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bhy.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://xwj.zycfv.cn

[D04] 删除元素
来源：http://qwj.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hqq.daxiang520.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wea.zhijiandao.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yio.jinqigufen.top

TS:   arr.splice(0, 1);
来源：http://top.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uwm.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mla.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://asx.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xsj.jqgufenzy.top

[D05] 访问与修改元素
来源：http://tch.chenlongwang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pjn.zdqjudy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ppe.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iyp.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://daj.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://yan.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://yxm.andypj.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ast.haohaochexian.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jrl.nanxuanxn.top

[D06] 数组长度
来源：http://jkn.yuanzhike.top

Py:   len(arr)
来源：http://bqo.ybcxt.top

PHP:  count($arr);
来源：http://ysb.fehbvm.com

JS:   arr.length
来源：http://ade.guannengcc.top

TS:   arr.length
来源：http://plf.bjfxy.top

Java: list.size();
来源：http://sck.fktsv.cn

Go:   len(arr)
来源：http://yqb.ybcxt.top

Ruby: arr.length; arr.size
来源：http://sxt.pycfn.com

C#:   list.Count;
来源：http://wdv.hammf.cn

[D07] 切片 / 取子数组
来源：http://dmt.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bde.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://swj.birdmap.top

JS:   arr.slice(1, 4);
来源：http://nuu.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://ybx.zdqjudy.top

Java: list.subList(1, 4);
来源：http://opn.quarkkingdee.top

Go:   arr[1:4]
来源：http://zmu.cashguo.top

Ruby: arr[1, 3]
来源：http://kda.zhijiandao.cn

C#:   list.GetRange(1, 3);
来源：http://mzg.sweek.top

[D08] 合并两个数组
来源：http://zee.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://qua.hammf.cn

PHP:  array_merge($a, $b);
来源：http://isi.zhoulong.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://chc.yfazqb.com

TS:   [...a, ...b];
来源：http://gto.pycfn.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tlj.yj20258.top

Go:   append(a, b...)
来源：http://mvo.ivvv.top

Ruby: a + b;  a.concat(b)
来源：http://zsj.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://tge.wangdashe.top

[D09] 排序（升序）
来源：http://rgn.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://opq.pycfn.com

PHP:  sort($arr);
来源：http://svv.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://anr.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kxi.shanyushiyangtech.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jxd.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uaf.sjlbkw.cn

Ruby: arr.sort
来源：http://nzj.cheryme.top

C#:   list.Sort();
来源：http://ivi.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://hhs.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cfo.zhiwuduotai.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fxp.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wbc.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dxi.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vjp.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kph.jinyuanbaomall.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://grt.gogol.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://trs.hcnkem.com

[D11] 反转数组
来源：http://xqc.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://wor.uphjek.com

PHP:  array_reverse($arr);
来源：http://awa.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://upi.shangyingyoupin.top

TS:   [...arr].reverse();
来源：http://alw.hcnkem.com

Java: Collections.reverse(list);
来源：http://qlc.jlsjyb.cn

Go:   slices.Reverse(arr)
来源：http://xgn.cheryme.top

Ruby: arr.reverse
来源：http://rfo.aizwys.cn

C#:   list.Reverse();
来源：http://dzi.zhoulong.xyz

[D12] 查找元素下标
来源：http://ujv.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://sug.sjlbkw.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eqh.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wfa.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ozm.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uxt.jiagoushi.top

Go:   slices.Index(arr, x)
来源：http://ikz.0kj1m.cn

Ruby: arr.index(x)
来源：http://wrx.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://pai.fzhhl.top

[D13] 过滤（保留满足条件的）
来源：http://evt.shuidangran.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xja.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nyc.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://snr.zhijiandao.cn

TS:   arr.filter(x => x > 3)
来源：http://utn.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wfy.havefunace.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xuv.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ong.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ozk.jinqigfzy.top

[D14] 映射转换（每个元素变形）
来源：http://csy.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nxq.sweek.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ndh.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://kyk.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://fmc.ywan-chungtsiang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://whi.zdbjq.cn

Go:   // 手写循环
来源：http://npm.guannengcc.top

Ruby: arr.map { |x| x * 2 }
来源：http://fox.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rwb.52xcode.cn

[D15] 去重
来源：http://ljn.ivvv.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jgt.cucudq.cn

PHP:  array_unique($arr);
来源：http://etr.tian-w.cn

JS:   [...new Set(arr)]
来源：http://lmf.aizwys.cn

TS:   [...new Set(arr)]
来源：http://gqn.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dhc.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wwd.cqqwz.cn

Ruby: arr.uniq
来源：http://woh.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://wka.zhixingplan.top

[D16] 求和与平均值
来源：http://zdf.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tsr.zdbjq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kdz.jinqigfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rve.yongpay.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wnx.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rdw.birdmap.top

Go:   // 手写循环累加
来源：http://xxy.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mjl.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://zff.redwolf501.top

[D17] 最大值与最小值
来源：http://gkd.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://lbz.hongshengwenyu.top

PHP:  max($arr);  min($arr);
来源：http://ipx.shanyushiyangtech.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qlo.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://kib.bjfxy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bab.jinghuilouyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tgf.havefunace.top

Ruby: arr.max;  arr.min
来源：http://kwh.dianchejie.cn

C#:   list.Max();  list.Min()
来源：http://ffn.hongshengwenyu.top

[D18] 扁平化嵌套数组
来源：http://drt.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cqp.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://xab.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xql.xuanzx.com

TS:   nested.flat();
来源：http://agd.xingfuxueyuan.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qlh.316326.xyz

Go:   // 手写双层循环
来源：http://srn.gaohongyu789.top

Ruby: nested.flatten
来源：http://qiz.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://acw.yvedp.cn

[D19] 按字段分组
来源：http://wmm.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://swq.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qes.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pol.fzhhl.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cte.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ral.gotoacloud.top

Go:   // 手写 map[string][]T
来源：http://roq.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fvc.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uwh.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://ryc.shuidangran.top

Py:   Counter(arr)
来源：http://kqc.9152youxi.cn

PHP:  array_count_values($arr);
来源：http://fda.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://caz.bjfxy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nbh.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eio.hnqzz.top

Go:   // 手写 map[T]int
来源：http://wwl.snrcjt.cn

Ruby: arr.tally
来源：http://zim.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kvl.yongpay.top

[D21] 判断是否包含某元素
来源：http://ehn.yj202588.top

Py:   x in arr
来源：http://ixz.yonumen.top

PHP:  in_array($x, $arr, true);
来源：http://anu.jqgufenzy.top

JS:   arr.includes(x)
来源：http://ula.hesvh.cn

TS:   arr.includes(x)
来源：http://xbg.nanxinkj.top

Java: list.contains(x)
来源：http://oqx.guannengcc.top

Go:   slices.Contains(arr, x)
来源：http://qhn.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://ttw.dianchejie.cn

C#:   list.Contains(x)
来源：http://yto.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://roi.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wea.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uxb.cqqwz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://apr.ybcxt.top

TS:   [...arr];
来源：http://jsk.svipenyu.cn

Java: new ArrayList<>(list);
来源：http://gxb.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ujk.shangyingyoupin.top

Ruby: arr.dup;  arr.clone
来源：http://ebb.jinqigfzy.top

C#:   new List<int>(list);
来源：http://msq.vqdsnc.cn


<!-- 参考信息 -->