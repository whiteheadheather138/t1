代发 wailian999

[C06] 匿名函数 / lambda
来源：http://gbh.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://lmy.yangfankeji.com

PHP:  $square = fn($x) => $x * $x;
来源：http://uqb.ywan-chungtsiang.top

JS:   const square = x => x * x;
来源：http://bxq.tarul.cn

TS:   const square = (x: number): number => x * x;
来源：http://ksw.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rcn.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vry.havefunace.top

Ruby: square = ->(x) { x * x }
来源：http://sau.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://agr.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://bvm.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sof.yfazqb.com

PHP:  array_map("strtoupper", $arr);
来源：http://mbl.guowangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uoi.gzhubu.top

TS:   arr.map(String)
来源：http://ogh.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ywi.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bcx.yj20258888.top

Ruby: arr.map(&:upcase)
来源：http://obu.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://caa.hongshengwenyu.top

[C08] 闭包
来源：http://odn.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lht.pycfn.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://avt.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hyr.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nwb.nanxuanxn.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wph.shangyingyoupin.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tvx.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dba.ydzc1.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vgv.epnwcf.com

[C09] 递归
来源：http://wvj.xziqi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vru.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lxl.dashuyun.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ehp.ywan-chungtsiang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wpy.wangdashe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hfw.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eus.jqgfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zoe.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zio.vqdsnc.cn

[C10] 变量作用域
来源：http://lly.cqqwz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pao.hcnkem.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uct.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vpz.jqgfzy.top

TS:   同 JS
来源：http://xim.vehdjk.com

Java: 方法内为块级作用域
来源：http://cko.fehbvm.com

Go:   花括号块级作用域
来源：http://jfr.zhixingplan.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xiv.jqgufenzy.top

C#:   块级作用域
来源：http://tym.jinqigufen.top

[C11] 模块导入与导出
来源：http://xfr.xinyue.icu

Py:   from module import func
来源：http://fay.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kvg.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://glp.xinyue.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xak.gotoacloud.top

Java: import java.util.List;
来源：http://obu.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yww.gotoacloud.top

Ruby: require "json"; require_relative "./util"
来源：http://hmd.quarkkingdee.top

C#:   using System.Text;
来源：http://eyb.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://lql.pengpengdd.cyou

Py:   (lambda: print("run"))()
来源：http://grt.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://kim.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://bxh.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://ufe.jinqigfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zhf.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://jlu.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://zsm.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://snv.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://vub.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sow.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pgt.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eau.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xeu.yueranfly.top

Java: int add(int a, int b) { return a + b; }
来源：http://nwr.yuanzhike.top

Go:   func add(a, b int) int
来源：http://kov.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yzx.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://ont.mhx1999.top

[C14] 泛型函数
来源：http://xoq.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://amk.cdnleiting.top

PHP:  // 无泛型
来源：http://qrg.zhoulong.xyz

JS:   // 无泛型
来源：http://esu.xuanzx.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dep.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://noe.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bbg.smart0.xyz

Ruby: # 无泛型
来源：http://xvb.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rri.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://yks.feifeiyinyue.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xiw.zhijiandao.cn

PHP:  [$a, $b] = $pair;
来源：http://ndq.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rbw.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jyq.wangshuangyany.cn

Java: // 无解构
来源：http://qqo.cashguo.top

Go:   // 无解构
来源：http://lcq.sufxvd.cn

Ruby: a, b = pair
来源：http://omg.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://ypi.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://umx.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zbh.sysykeji.top

PHP:  // 无重载
来源：http://pyn.fzhhl.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ndh.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://bjk.jinyuanbaomall.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ftz.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://gyd.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://aee.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rmk.yuanzhike.top

================================================================================
来源：http://ixu.quarkkingdee.top

D. 数组 / 列表 / 集合
来源：http://yng.sufxvd.cn

================================================================================
来源：http://gwq.sufxvd.cn

[D01] 创建数组 / 列表
来源：http://exh.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://obn.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ihb.shuidangran.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pqn.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://non.xingfuxueyuan.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yvq.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://hkv.yvedp.cn

Ruby: arr = [1, 2, 3]
来源：http://kmb.yongpay.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://faj.gotoacloud.top

[D02] 追加元素到末尾
来源：http://tmr.zdbjq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wgg.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xks.redwolf501.top

JS:   arr.push(4);
来源：http://spo.ydzc1.top

TS:   arr.push(4);
来源：http://njr.zhijiandao.cn

Java: list.add(4);
来源：http://uxb.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://kbe.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://tpa.jinghuilouyu.cn

C#:   list.Add(4);
来源：http://saj.yangfankeji.com

[D03] 在指定位置插入元素
来源：http://njo.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://kmn.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rqo.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://roi.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://ffy.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://mtt.shuidangran.top

Go:   arr = append([]int{0}, arr...)
来源：http://kmq.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zej.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://eaw.iojbl.cn

[D04] 删除元素
来源：http://pyx.ydjk.org.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ylp.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kdi.yfazqb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://str.yj20258.top

TS:   arr.splice(0, 1);
来源：http://nim.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fsp.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rnu.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fdj.yj202588.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cbh.vehdjk.com

[D05] 访问与修改元素
来源：http://lvu.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ict.fengsongda.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dhe.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jox.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://fku.hfpthk.cn

Java: list.get(0); list.set(0, 9);
来源：http://bpe.hammf.cn

Go:   arr[0]; arr[0] = 9
来源：http://rte.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qwf.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://swm.yj202588.top

[D06] 数组长度
来源：http://mke.chenzaomai.com

Py:   len(arr)
来源：http://nnv.meibo888.top

PHP:  count($arr);
来源：http://wrt.daxiang520.top

JS:   arr.length
来源：http://wek.ybcxt.top

TS:   arr.length
来源：http://mny.yonumen.top

Java: list.size();
来源：http://idf.jiagoushi.top

Go:   len(arr)
来源：http://nki.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://gpx.yvedp.cn

C#:   list.Count;
来源：http://zvo.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://ror.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sty.chenzaomai.com

PHP:  array_slice($arr, 1, 3);
来源：http://ftm.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://iuo.yonumen.top

TS:   arr.slice(1, 4);
来源：http://lzc.hesvh.cn

Java: list.subList(1, 4);
来源：http://ksc.316326.xyz

Go:   arr[1:4]
来源：http://rjp.fengsongda.top

Ruby: arr[1, 3]
来源：http://jon.cashguo.top

C#:   list.GetRange(1, 3);
来源：http://qgd.chenzaomai.com

[D08] 合并两个数组
来源：http://tuj.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://yfi.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://kok.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cwc.xziqi.cn

TS:   [...a, ...b];
来源：http://ccs.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mci.redwolf501.top

Go:   append(a, b...)
来源：http://zrc.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://vze.ydzc1.top

C#:   a.Concat(b).ToList()
来源：http://adf.chenlongwang.top

[D09] 排序（升序）
来源：http://njt.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://dhz.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://oxo.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://azs.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yng.fehbvm.com

Java: Collections.sort(list);  list.sort(null);
来源：http://ggg.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://njw.jinqigufen.top

Ruby: arr.sort
来源：http://wwr.xinyue.icu

C#:   list.Sort();
来源：http://cwr.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rcn.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eds.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://imb.haohaochexian.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uiy.cdnleiting.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://snv.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ksg.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tdn.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aop.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://imm.svipenyu.cn

[D11] 反转数组
来源：http://vzk.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ctt.tarul.cn

PHP:  array_reverse($arr);
来源：http://yfy.xinyue.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://klv.jinqigufen.top

TS:   [...arr].reverse();
来源：http://ttb.vehdjk.com

Java: Collections.reverse(list);
来源：http://luk.vehdjk.com

Go:   slices.Reverse(arr)
来源：http://oyn.xuetiantiany.cn

Ruby: arr.reverse
来源：http://mki.dianchejie.cn

C#:   list.Reverse();
来源：http://ger.sjlbkw.cn

[D12] 查找元素下标
来源：http://ryg.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://zww.dashuyun.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lix.9152youxi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hhp.cdnleiting.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mfc.chenzaomai.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mpd.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://zke.sxryk.cn

Ruby: arr.index(x)
来源：http://bnx.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://eat.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://ess.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qwe.xylfe.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cry.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://qbr.meibo888.top

TS:   arr.filter(x => x > 3)
来源：http://vhu.snrcjt.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jlb.gaohongyu789.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fuv.haohaochexian.top

Ruby: arr.select { |x| x > 3 }
来源：http://bhm.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://dbx.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://kqx.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lmp.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vwa.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://lft.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://wrr.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zth.fehbvm.com

Go:   // 手写循环
来源：http://dys.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gwa.zhijiandao.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://teo.shanyushiyangkeji.top

[D15] 去重
来源：http://mob.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kdw.feifeiyinyue.top

PHP:  array_unique($arr);
来源：http://zxu.fehbvm.com

JS:   [...new Set(arr)]
来源：http://ufr.tarul.cn

TS:   [...new Set(arr)]
来源：http://kjp.hesvh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aap.jinqigfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://thn.fanxiaobao.xyz

Ruby: arr.uniq
来源：http://rlt.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://aeu.guannengcc.top

[D16] 求和与平均值
来源：http://cua.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cmm.daxiang520.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://khu.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jkp.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bbk.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gse.316326.xyz

Go:   // 手写循环累加
来源：http://nfz.daria6918.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ewu.yvedp.cn

C#:   list.Sum();  list.Average()
来源：http://ykk.shanyushiyangkeji.top

[D17] 最大值与最小值
来源：http://laf.hnxiangtu.top

Py:   max(arr);  min(arr)
来源：http://kgd.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://utd.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oys.pengpengdd.cyou

TS:   Math.max(...arr);
来源：http://hqp.xziqi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fnr.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mpb.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://uhc.uphjek.com

C#:   list.Max();  list.Min()
来源：http://nmm.meibo888.top

[D18] 扁平化嵌套数组
来源：http://chg.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dmz.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://pfq.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hpv.snrcjt.cn

TS:   nested.flat();
来源：http://mbp.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://otl.yongpay.top

Go:   // 手写双层循环
来源：http://dzg.jinqigufen.top

Ruby: nested.flatten
来源：http://meb.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://hcl.sweek.top

[D19] 按字段分组
来源：http://tgq.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iqv.sufxvd.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hds.fengsongda.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lsg.fktsv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fgy.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://woc.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://uzm.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://pgu.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://piq.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://nrt.c1oappe.top

Py:   Counter(arr)
来源：http://vvz.ybcxt.top

PHP:  array_count_values($arr);
来源：http://flx.redwolf501.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cic.andypj.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qaj.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://anx.dianchejie.cn

Go:   // 手写 map[T]int
来源：http://fxo.guowangkeji.top

Ruby: arr.tally
来源：http://jcf.yanxiufei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dii.hywenlv.cn

[D21] 判断是否包含某元素
来源：http://rfv.jyoumei.cn

Py:   x in arr
来源：http://duc.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://gga.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://iot.xuanzx.com

TS:   arr.includes(x)
来源：http://uxi.jianghu66.top

Java: list.contains(x)
来源：http://qjc.hnqzz.top

Go:   slices.Contains(arr, x)
来源：http://txt.cqqwz.cn

Ruby: arr.include?(x)
来源：http://hex.gzhubu.top

C#:   list.Contains(x)
来源：http://kdz.svipenyu.cn

[D22] 复制数组（避免共享引用）
来源：http://ssn.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kdm.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lnz.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nza.zhaomingkeji.xyz

TS:   [...arr];
来源：http://vue.havefunace.top

Java: new ArrayList<>(list);
来源：http://kke.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://glc.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://uwt.snrcjt.cn

C#:   new List<int>(list);
来源：http://vsr.chenlongwang.top


<!-- 参考信息 -->