代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://tdr.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://scv.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://rwv.gzhubu.top

Ruby: square = ->(x) { x * x }
来源：http://qor.uphjek.com

C#:   Func<int, int> square = x => x * x;
来源：http://ohv.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://hpe.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://owf.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://mpy.guannengcc.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qqd.chenzaomai.com

TS:   arr.map(String)
来源：http://dql.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://trd.hnqzz.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://adw.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://smf.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://yzf.xuetiantiany.cn

[C08] 闭包
来源：http://qzy.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ooa.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vdt.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ewj.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hhy.pengpengdd.cyou

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qtd.redwolf501.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://huy.gaohongyu789.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://smn.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zib.jinqigfzy.top

[C09] 递归
来源：http://kmn.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lva.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pcm.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://luz.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kvc.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dxq.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ehp.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fgg.zhixingplan.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zny.tianlin.xyz

[C10] 变量作用域
来源：http://esu.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bcb.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rky.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jbf.hcnkem.com

TS:   同 JS
来源：http://ict.yonumen.top

Java: 方法内为块级作用域
来源：http://fkt.tarul.cn

Go:   花括号块级作用域
来源：http://cnc.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iuu.zdbjq.cn

C#:   块级作用域
来源：http://jnp.yueranfly.top

[C11] 模块导入与导出
来源：http://szd.jqgufenzy.top

Py:   from module import func
来源：http://ohk.yangfankeji.com

PHP:  require "file.php";  或 use App\Service;
来源：http://kkt.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vll.sufxvd.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lsi.cqqwz.cn

Java: import java.util.List;
来源：http://erg.sxryk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wjj.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://bzl.cheryme.top

C#:   using System.Text;
来源：http://jng.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://rrv.yj202588.top

Py:   (lambda: print("run"))()
来源：http://nlo.andypj.xyz

PHP:  (function () { echo "run"; })();
来源：http://ltr.shanyushiyangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://sxi.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://xee.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uml.xuetiantiany.cn

Go:   func() { fmt.Println("run") }()
来源：http://fov.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://vic.jiagoushi.top

C#:   // 无 IIFE：用静态构造函数
来源：http://coq.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://bkw.xingfuxueyuan.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tyv.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tei.jinqigfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cpc.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://olm.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://pdo.ehwqpu.com

Go:   func add(a, b int) int
来源：http://jok.haohaochexian.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lii.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rlm.cashguo.top

[C14] 泛型函数
来源：http://pua.yj20258.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ytn.ydzc1.top

PHP:  // 无泛型
来源：http://wns.chenlongwang.top

JS:   // 无泛型
来源：http://clp.gzhubu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yuz.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://afz.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dib.ydzc1.top

Ruby: # 无泛型
来源：http://idg.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fxj.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://fxz.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qpp.hysaishi.cn

PHP:  [$a, $b] = $pair;
来源：http://nsj.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xob.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zzf.ctjpmb.com

Java: // 无解构
来源：http://him.epnwcf.com

Go:   // 无解构
来源：http://ura.daxiang520.top

Ruby: a, b = pair
来源：http://ivn.tarul.cn

C#:   var (a, b) = pair;
来源：http://lhn.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://tle.fzhhl.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iuq.pycfn.com

PHP:  // 无重载
来源：http://ldh.andypj.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://ogo.tarul.cn

TS:   // 用联合类型或重载签名声明
来源：http://cvu.guowangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gvd.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://ucs.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://omm.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jxe.jinqigufen.top

================================================================================
来源：http://twm.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://xju.hnqzz.top

================================================================================
来源：http://gnh.gzhubu.top

[D01] 创建数组 / 列表
来源：http://ktl.jinyuanbaomall.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zzj.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xkl.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rry.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pbb.chenjidiqi.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zuv.ydjk.org.cn

Go:   arr := []int{1, 2, 3}
来源：http://jgb.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://mzj.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bud.bbcook.cn

[D02] 追加元素到末尾
来源：http://ynq.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jio.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://khf.zhengqikj.top

JS:   arr.push(4);
来源：http://tvm.hongshengwenyu.top

TS:   arr.push(4);
来源：http://hlq.yfazqb.com

Java: list.add(4);
来源：http://qjk.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://nbi.fehbvm.com

Ruby: arr << 4; arr.push(5)
来源：http://wkz.ppjwa.cn

C#:   list.Add(4);
来源：http://nlm.chenjidiqi.icu

[D03] 在指定位置插入元素
来源：http://mmu.ywan-chungtsiang.top

Py:   arr.insert(0, 0)
来源：http://zec.chenzaomai.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qoq.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wqb.ydjk.org.cn

TS:   arr.splice(0, 0, 0);
来源：http://wya.cdnleiting.top

Java: list.add(0, 0);
来源：http://hdb.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://fmv.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zbo.tarul.cn

C#:   list.Insert(0, 0);
来源：http://ppp.zhaomingkeji.xyz

[D04] 删除元素
来源：http://kub.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nfk.fktsv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mcb.fzhhl.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fhc.zdbjq.cn

TS:   arr.splice(0, 1);
来源：http://fuq.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://drb.cdnleiting.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qhz.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vzg.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://whr.ehwqpu.com

[D05] 访问与修改元素
来源：http://cmu.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cpx.ivvv.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yek.c1oappe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://muf.cashguo.top

TS:   arr[0]; arr.at(-1);
来源：http://lco.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://gsm.sweek.top

Go:   arr[0]; arr[0] = 9
来源：http://bin.hesvh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qxl.yongpay.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sum.dianchejie.cn

[D06] 数组长度
来源：http://pef.jlsjyb.cn

Py:   len(arr)
来源：http://klj.zhoulong.xyz

PHP:  count($arr);
来源：http://fbi.yuxming.cn

JS:   arr.length
来源：http://qcb.nanxinkj.top

TS:   arr.length
来源：http://pdc.0kj1m.cn

Java: list.size();
来源：http://xdw.daria6918.cn

Go:   len(arr)
来源：http://gty.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://eqx.xylfe.cn

C#:   list.Count;
来源：http://xtb.fzhhl.top

[D07] 切片 / 取子数组
来源：http://sui.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://phg.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rnc.wangshuangyany.cn

JS:   arr.slice(1, 4);
来源：http://poc.redwolf501.top

TS:   arr.slice(1, 4);
来源：http://iuv.yuxming.cn

Java: list.subList(1, 4);
来源：http://gsc.yueranfly.top

Go:   arr[1:4]
来源：http://ggd.chenlongwang.top

Ruby: arr[1, 3]
来源：http://grw.ydzc1.top

C#:   list.GetRange(1, 3);
来源：http://kya.chenjidiqi.icu

[D08] 合并两个数组
来源：http://jvl.jyoumei.cn

Py:   a + b;  a.extend(b)
来源：http://uwp.tianlin.xyz

PHP:  array_merge($a, $b);
来源：http://mbk.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://gur.fanxiaobao.xyz

TS:   [...a, ...b];
来源：http://mey.jinyuanbaomall.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://avd.nanxinkj.top

Go:   append(a, b...)
来源：http://uxq.yfazqb.com

Ruby: a + b;  a.concat(b)
来源：http://pur.yanxiufei.cn

C#:   a.Concat(b).ToList()
来源：http://khe.tian-w.cn

[D09] 排序（升序）
来源：http://mji.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://wyu.xinyue.icu

PHP:  sort($arr);
来源：http://jbp.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ynv.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rrb.sysykeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dmk.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nqo.zhoulong.xyz

Ruby: arr.sort
来源：http://sub.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://hrg.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://coz.shangyingyoupin.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zum.jyoumei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://phz.daxiang520.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://umh.cashguo.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uke.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rxs.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fmo.dashuyun.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sek.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zew.zycfv.cn

[D11] 反转数组
来源：http://pmx.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://piw.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://msa.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kam.mhx1999.top

TS:   [...arr].reverse();
来源：http://gvg.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://sua.xylfe.cn

Go:   slices.Reverse(arr)
来源：http://rrx.0kj1m.cn

Ruby: arr.reverse
来源：http://vlh.ydzc1.top

C#:   list.Reverse();
来源：http://jir.zdbjq.cn

[D12] 查找元素下标
来源：http://mxc.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://mkf.sufxvd.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dxg.jianghu66.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://plk.xingfuxueyuan.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qgv.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bxp.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://ucf.sxryk.cn

Ruby: arr.index(x)
来源：http://lhd.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://nfo.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://eac.xinyue.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jqc.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kqw.pengpengdd.cyou

JS:   arr.filter(x => x > 3)
来源：http://cad.jlsjyb.cn

TS:   arr.filter(x => x > 3)
来源：http://xnu.yj20258.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cze.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fec.zhixingplan.top

Ruby: arr.select { |x| x > 3 }
来源：http://mio.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vnh.ybcxt.top

[D14] 映射转换（每个元素变形）
来源：http://lla.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rmn.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tqz.epnwcf.com

JS:   arr.map(x => x * 2)
来源：http://irk.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://wml.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xsw.havefunace.top

Go:   // 手写循环
来源：http://igt.ivvv.top

Ruby: arr.map { |x| x * 2 }
来源：http://nok.feifeiyinyue.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ljs.cheryme.top

[D15] 去重
来源：http://zur.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iay.ybcxt.top

PHP:  array_unique($arr);
来源：http://ylh.hongshengwenyu.top

JS:   [...new Set(arr)]
来源：http://mhm.ydzc1.top

TS:   [...new Set(arr)]
来源：http://tkf.cheryme.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iag.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dxv.cashguo.top

Ruby: arr.uniq
来源：http://fzf.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://tba.fktsv.cn

[D16] 求和与平均值
来源：http://utg.cqqwz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rpk.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vsz.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rih.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mfs.bbcook.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gpa.epnwcf.com

Go:   // 手写循环累加
来源：http://cig.ybcxt.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lha.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://bnq.jinqigufen.top

[D17] 最大值与最小值
来源：http://hsz.jianghu66.top

Py:   max(arr);  min(arr)
来源：http://mhf.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://cys.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xcj.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://nah.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://fah.zhixingplan.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://evw.hammf.cn

Ruby: arr.max;  arr.min
来源：http://hmx.sysykeji.top

C#:   list.Max();  list.Min()
来源：http://srw.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://xns.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sok.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://fbh.jinghuilouyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cxt.jyoumei.cn

TS:   nested.flat();
来源：http://sbq.sufxvd.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://slf.gaohongyu789.top

Go:   // 手写双层循环
来源：http://psc.yvedp.cn

Ruby: nested.flatten
来源：http://dpw.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://klq.xinyue.icu

[D19] 按字段分组
来源：http://jaq.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yob.jinyuanbaomall.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ank.haohaochexian.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ugw.jyoumei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ovn.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nys.xingfuxueyuan.xyz

Go:   // 手写 map[string][]T
来源：http://ftc.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://lfq.redwolf501.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://btv.yuxming.cn

[D20] 统计每个元素出现次数
来源：http://ajm.ydjk.org.cn

Py:   Counter(arr)
来源：http://pjc.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://zpq.zhixingplan.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cft.sysykeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://foq.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lmx.cheryme.top

Go:   // 手写 map[T]int
来源：http://xed.xuanzx.com

Ruby: arr.tally
来源：http://wia.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://scv.ctjpmb.com

[D21] 判断是否包含某元素
来源：http://ihe.guannengcc.top

Py:   x in arr
来源：http://qaa.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://fxz.ydjk.org.cn

JS:   arr.includes(x)
来源：http://qfh.ctjpmb.com

TS:   arr.includes(x)
来源：http://aym.tanke756.top

Java: list.contains(x)
来源：http://qcw.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://lct.cashguo.top

Ruby: arr.include?(x)
来源：http://lfj.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://pty.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://mek.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qnc.shuidangran.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jue.dianchejie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ypn.iojbl.cn

TS:   [...arr];
来源：http://swq.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://kft.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://cxy.yueranfly.top

Ruby: arr.dup;  arr.clone
来源：http://bja.haohaochexian.top

C#:   new List<int>(list);
来源：http://fqy.fengsongda.top

[D23] reduce 累积计算
来源：http://rly.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lsx.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wfc.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://roy.xylfe.cn


<!-- 参考信息 -->