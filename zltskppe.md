代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://zcm.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://mpg.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mhd.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://raq.sxryk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zpx.jianghu66.top

TS:   arr.map(String)
来源：http://dsj.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bsy.guowangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eor.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://hmt.redwolf501.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kux.dianchejie.cn

[C08] 闭包
来源：http://nie.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yfs.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://soe.yonumen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wkl.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yyq.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gtm.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pqt.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kqi.ivvv.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bsl.wangdashe.top

[C09] 递归
来源：http://wid.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mrd.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gdd.dashuyun.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://veo.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pve.fanxiaobao.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wql.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://diu.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ojj.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lop.nanxuanxn.top

[C10] 变量作用域
来源：http://tba.ydjk.org.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://auf.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fpq.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bpw.hongshengwenyu.top

TS:   同 JS
来源：http://ovu.0kj1m.cn

Java: 方法内为块级作用域
来源：http://xel.dianchejie.cn

Go:   花括号块级作用域
来源：http://chf.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://duk.tian-w.cn

C#:   块级作用域
来源：http://jhs.yongpay.top

[C11] 模块导入与导出
来源：http://xqy.hongshengwenyu.top

Py:   from module import func
来源：http://hff.yanxiufei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xuj.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://lxk.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ypp.yvedp.cn

Java: import java.util.List;
来源：http://lmk.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rin.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://swn.zhengqikj.top

C#:   using System.Text;
来源：http://tyk.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://yhz.zhixingplan.top

Py:   (lambda: print("run"))()
来源：http://znk.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://xwr.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://hsk.cqqwz.cn

TS:   (() => { console.log("run"); })();
来源：http://nxq.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ttn.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://fko.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://bao.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kki.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://lzq.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://psu.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tsv.0kj1m.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ydt.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qoh.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://msr.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://iwu.iojbl.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bhf.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jec.shangyingyoupin.top

[C14] 泛型函数
来源：http://xll.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uak.birdmap.top

PHP:  // 无泛型
来源：http://eqi.jinqigufen.top

JS:   // 无泛型
来源：http://mqz.jinqigfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tdx.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ndn.ydjk.org.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nfz.birdmap.top

Ruby: # 无泛型
来源：http://zyv.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sjq.ydjk.org.cn

[C15] 解构 / 展开参数
来源：http://hkd.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://awp.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://vep.ctjpmb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jvj.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cqb.yj20258888.top

Java: // 无解构
来源：http://wdp.hysaishi.cn

Go:   // 无解构
来源：http://hxv.xziqi.cn

Ruby: a, b = pair
来源：http://dne.yj202588.top

C#:   var (a, b) = pair;
来源：http://gda.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://nbq.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sqh.chenzaomai.com

PHP:  // 无重载
来源：http://zei.ybcxt.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hwx.ydjk.org.cn

TS:   // 用联合类型或重载签名声明
来源：http://zxa.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://etb.jqgfzy.top

Go:   // 无重载：用不同函数名
来源：http://sph.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://aim.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dqa.svipenyu.cn

================================================================================
来源：http://uqe.yuxming.cn

D. 数组 / 列表 / 集合
来源：http://ibu.yj20258888.top

================================================================================
来源：http://xmg.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://uex.yvedp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tap.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://idx.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rxt.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://naw.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fdz.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://zmo.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://zct.cucudq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ibb.fktsv.cn

[D02] 追加元素到末尾
来源：http://mgs.zdbjq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://unr.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://spg.tarul.cn

JS:   arr.push(4);
来源：http://yfm.zycfv.cn

TS:   arr.push(4);
来源：http://vql.zhaomingkeji.xyz

Java: list.add(4);
来源：http://rtz.jinghuilouyu.cn

Go:   arr = append(arr, 4)
来源：http://alh.zycfv.cn

Ruby: arr << 4; arr.push(5)
来源：http://pol.sysykeji.top

C#:   list.Add(4);
来源：http://hdm.yj20258.top

[D03] 在指定位置插入元素
来源：http://lif.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://cpx.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bcn.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://inn.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://pyu.sufxvd.cn

Java: list.add(0, 0);
来源：http://jpo.sjlbkw.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lsn.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vgn.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://rvd.epnwcf.com

[D04] 删除元素
来源：http://eik.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dqu.ivvv.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lcn.epnwcf.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qhx.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://auy.xziqi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ijt.xuanzx.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yhy.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lyd.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rqs.aizwys.cn

[D05] 访问与修改元素
来源：http://oxd.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fjb.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gfx.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vsp.yueranfly.top

TS:   arr[0]; arr.at(-1);
来源：http://cbs.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://xnf.52xcode.cn

Go:   arr[0]; arr[0] = 9
来源：http://who.cucudq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rjn.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gsf.chenjidiqi.icu

[D06] 数组长度
来源：http://vkh.shanyushiyangtech.top

Py:   len(arr)
来源：http://onp.chenlongwang.top

PHP:  count($arr);
来源：http://hcg.shzxlz.cn

JS:   arr.length
来源：http://qzz.cucudq.cn

TS:   arr.length
来源：http://ngd.zdqjudy.top

Java: list.size();
来源：http://uqd.yueranfly.top

Go:   len(arr)
来源：http://oym.52xcode.cn

Ruby: arr.length; arr.size
来源：http://elf.zhoulong.xyz

C#:   list.Count;
来源：http://fjq.jianghu66.top

[D07] 切片 / 取子数组
来源：http://qqh.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xnk.chenzaomai.com

PHP:  array_slice($arr, 1, 3);
来源：http://yki.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://tce.nwbrower.top

TS:   arr.slice(1, 4);
来源：http://vrk.316326.xyz

Java: list.subList(1, 4);
来源：http://qhq.cashguo.top

Go:   arr[1:4]
来源：http://fdc.chenlongwang.top

Ruby: arr[1, 3]
来源：http://oxt.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://rvd.daxiang520.top

[D08] 合并两个数组
来源：http://kam.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://ahc.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://dqk.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://byu.ybcxt.top

TS:   [...a, ...b];
来源：http://rtb.gzhubu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eal.hfpthk.cn

Go:   append(a, b...)
来源：http://hsy.hnxiangtu.top

Ruby: a + b;  a.concat(b)
来源：http://lxm.nwbrower.top

C#:   a.Concat(b).ToList()
来源：http://zwp.fzhhl.top

[D09] 排序（升序）
来源：http://xej.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://kne.pycfn.com

PHP:  sort($arr);
来源：http://edy.cqqwz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bys.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rbo.svipenyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qjn.svipenyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zvh.yvedp.cn

Ruby: arr.sort
来源：http://xus.gogol.net.cn

C#:   list.Sort();
来源：http://ysj.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://acr.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wgh.meibo888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ykv.sweek.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iby.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ejd.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xlh.havefunace.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ikx.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xvs.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jun.guannengcc.top

[D11] 反转数组
来源：http://jzd.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://lyj.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://goe.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bjb.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://tob.haohaochexian.top

Java: Collections.reverse(list);
来源：http://gux.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://mxp.tianlin.xyz

Ruby: arr.reverse
来源：http://vtu.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://xqr.sweek.top

[D12] 查找元素下标
来源：http://xtt.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://pjf.shangyingyoupin.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tdw.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dso.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tgt.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kmw.yj20258.top

Go:   slices.Index(arr, x)
来源：http://mjr.aibaodan.cn

Ruby: arr.index(x)
来源：http://zvi.wangshuangyany.cn

C#:   list.IndexOf(x);
来源：http://xwv.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://qkv.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rck.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cth.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://xcm.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://cen.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oqv.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hnz.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://scv.hesvh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://trx.fktsv.cn

[D14] 映射转换（每个元素变形）
来源：http://hic.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eps.jinghuilouyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ibc.fzhhl.top

JS:   arr.map(x => x * 2)
来源：http://exe.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://trl.xuanzx.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ydy.yangfankeji.com

Go:   // 手写循环
来源：http://oex.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rpk.bjfxy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vnx.bjfxy.top

[D15] 去重
来源：http://bps.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dls.fzhhl.top

PHP:  array_unique($arr);
来源：http://hrs.cheryme.top

JS:   [...new Set(arr)]
来源：http://vrx.tian-w.cn

TS:   [...new Set(arr)]
来源：http://uet.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kyo.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xxq.xuanzx.com

Ruby: arr.uniq
来源：http://obz.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://oyz.52xcode.cn

[D16] 求和与平均值
来源：http://equ.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fjk.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tuq.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uzw.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pwc.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qxn.bbcook.cn

Go:   // 手写循环累加
来源：http://wcc.hysaishi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yar.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://gsw.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://fzu.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://dhe.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://vwd.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uen.epnwcf.com

TS:   Math.max(...arr);
来源：http://wae.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tar.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wnl.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://rzk.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://kzt.yongpay.top

[D18] 扁平化嵌套数组
来源：http://nyo.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cij.pengpengdd.cyou

PHP:  array_merge(...$nested);
来源：http://kbj.fanxiaobao.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://atm.jyoumei.cn

TS:   nested.flat();
来源：http://hyw.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rll.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://kjs.gogol.net.cn

Ruby: nested.flatten
来源：http://anr.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ysd.gzhubu.top

[D19] 按字段分组
来源：http://ots.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hxn.ydjk.org.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ubq.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dwm.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lbn.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://via.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://mxv.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mlr.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://usa.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://piz.wangdashe.top

Py:   Counter(arr)
来源：http://avh.cqqwz.cn

PHP:  array_count_values($arr);
来源：http://gau.chenlongwang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://axm.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ctd.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kkw.hammf.cn

Go:   // 手写 map[T]int
来源：http://cwz.chenlongwang.top

Ruby: arr.tally
来源：http://xju.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zqx.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://tje.fehbvm.com

Py:   x in arr
来源：http://obv.shzxlz.cn

PHP:  in_array($x, $arr, true);
来源：http://rid.316326.xyz

JS:   arr.includes(x)
来源：http://lou.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://jjl.sufxvd.cn

Java: list.contains(x)
来源：http://pbj.gaohongyu789.top

Go:   slices.Contains(arr, x)
来源：http://znp.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://bbw.xylfe.cn

C#:   list.Contains(x)
来源：http://ydz.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://wal.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cxl.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cre.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wck.ehwqpu.com

TS:   [...arr];
来源：http://kdf.zycfv.cn

Java: new ArrayList<>(list);
来源：http://wxd.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://jes.xuetiantiany.cn

Ruby: arr.dup;  arr.clone
来源：http://uvh.ctjpmb.com

C#:   new List<int>(list);
来源：http://qlk.ydjk.org.cn

[D23] reduce 累积计算
来源：http://xba.bbcook.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://irs.yonumen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wwc.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yir.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rsx.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pys.jqgufenzy.top

Go:   // 手写循环
来源：http://omu.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sxo.tarul.cn


<!-- 参考信息 -->