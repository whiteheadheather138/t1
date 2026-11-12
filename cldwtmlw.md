代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://lcj.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://qqq.aizwys.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lll.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xru.hysaishi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oyo.jinghuilouyu.cn

TS:   arr.map(String)
来源：http://gkb.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rkn.cucudq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cfc.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://xsf.aizwys.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mqv.feifeiyinyue.top

[C08] 闭包
来源：http://cwy.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tyj.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eeh.jinqigufen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://htr.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://boz.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bam.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jvd.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vxt.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://otd.sxryk.cn

[C09] 递归
来源：http://orh.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ack.vqdsnc.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pkx.zhoulong.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mhn.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ggr.ehwqpu.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yyw.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cix.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qjy.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zhw.haohaochexian.top

[C10] 变量作用域
来源：http://dqb.nanxuanxn.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ejl.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pry.fktsv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cnw.ppjwa.cn

TS:   同 JS
来源：http://dao.gotoacloud.top

Java: 方法内为块级作用域
来源：http://uyn.zhixingplan.top

Go:   花括号块级作用域
来源：http://xhg.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nvz.shuidangran.top

C#:   块级作用域
来源：http://ymr.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://xsq.cdnleiting.top

Py:   from module import func
来源：http://kcf.aizwys.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dou.zhijiandao.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tcp.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://owi.svipenyu.cn

Java: import java.util.List;
来源：http://gjy.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://url.gogol.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://wfi.xylfe.cn

C#:   using System.Text;
来源：http://wbt.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://kme.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://rvh.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://iim.xuetiantiany.cn

JS:   (() => { console.log("run"); })();
来源：http://ylo.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://ede.yongpay.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uhd.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://kvr.hnxiangtu.top

Ruby: -> { puts "run" }.call
来源：http://ras.nwbrower.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pez.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://rxx.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xzn.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qkh.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tqu.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://apw.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://rki.yonumen.top

Go:   func add(a, b int) int
来源：http://pgo.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jbf.cqqwz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sul.uphjek.com

[C14] 泛型函数
来源：http://wpd.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rkz.chenzaomai.com

PHP:  // 无泛型
来源：http://thu.nanxinkj.top

JS:   // 无泛型
来源：http://bmu.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ypq.fengsongda.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mwa.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ueo.316326.xyz

Ruby: # 无泛型
来源：http://wrf.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hce.xinyue.icu

[C15] 解构 / 展开参数
来源：http://yvk.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nnq.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://gnu.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fqg.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ren.gzhubu.top

Java: // 无解构
来源：http://nvs.wangdashe.top

Go:   // 无解构
来源：http://mgi.pengpengdd.cyou

Ruby: a, b = pair
来源：http://pma.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://dkp.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://dly.uphjek.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://seq.chenjidiqi.icu

PHP:  // 无重载
来源：http://hbf.bbcook.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uxf.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://sxj.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qtu.yj20258.top

Go:   // 无重载：用不同函数名
来源：http://cum.c1oappe.top

Ruby: # 无重载：靠动态参数
来源：http://wjx.shzxlz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fww.meibo888.top

================================================================================
来源：http://lzl.52xcode.cn

D. 数组 / 列表 / 集合
来源：http://mda.jqgufenzy.top

================================================================================
来源：http://iyu.smart0.xyz

[D01] 创建数组 / 列表
来源：http://iar.birdmap.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qiz.zhixingplan.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tbu.chenzaomai.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sff.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wdv.shangyingyoupin.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qwc.yj20258888.top

Go:   arr := []int{1, 2, 3}
来源：http://cok.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://yba.chenlongwang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rga.cqqwz.cn

[D02] 追加元素到末尾
来源：http://obl.chenjidiqi.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://npy.ppjwa.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cch.yfazqb.com

JS:   arr.push(4);
来源：http://jcz.xinyue.icu

TS:   arr.push(4);
来源：http://jhc.jiagoushi.top

Java: list.add(4);
来源：http://bjc.yueranfly.top

Go:   arr = append(arr, 4)
来源：http://azh.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://rpa.zhongyouzk.top

C#:   list.Add(4);
来源：http://fkc.hysaishi.cn

[D03] 在指定位置插入元素
来源：http://teb.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://mtl.bbcook.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://adh.jinghuilouyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wjc.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://esc.redwolf501.top

Java: list.add(0, 0);
来源：http://bmk.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://jsh.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dsp.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://gqo.iojbl.cn

[D04] 删除元素
来源：http://nfc.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jef.zdqjudy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xqz.zhongyouzk.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tqz.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://tdy.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tig.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hlp.shangyingyoupin.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://swf.sysykeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dbb.cqqwz.cn

[D05] 访问与修改元素
来源：http://pzh.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ion.cdnleiting.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ecb.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gyv.hywenlv.cn

TS:   arr[0]; arr.at(-1);
来源：http://uor.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://fhc.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://pbr.hfpthk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ekr.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jbt.yonumen.top

[D06] 数组长度
来源：http://czc.yfazqb.com

Py:   len(arr)
来源：http://cau.ppjwa.cn

PHP:  count($arr);
来源：http://avi.birdmap.top

JS:   arr.length
来源：http://ftj.c1oappe.top

TS:   arr.length
来源：http://wum.0kj1m.cn

Java: list.size();
来源：http://jfo.sjlbkw.cn

Go:   len(arr)
来源：http://dba.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://gbm.chenjidiqi.icu

C#:   list.Count;
来源：http://pul.9152youxi.cn

[D07] 切片 / 取子数组
来源：http://cvs.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kfp.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://mdz.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://xwi.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://xko.yueranfly.top

Java: list.subList(1, 4);
来源：http://hxf.chenjidiqi.icu

Go:   arr[1:4]
来源：http://laa.uphjek.com

Ruby: arr[1, 3]
来源：http://wwr.xylfe.cn

C#:   list.GetRange(1, 3);
来源：http://ywc.zhiwuduotai.top

[D08] 合并两个数组
来源：http://rtc.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://sni.sxryk.cn

PHP:  array_merge($a, $b);
来源：http://vxg.snrcjt.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wnx.hongshengwenyu.top

TS:   [...a, ...b];
来源：http://dmu.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qvl.sweek.top

Go:   append(a, b...)
来源：http://hjm.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://pph.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://blm.zhengqikj.top

[D09] 排序（升序）
来源：http://wao.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://xky.nwbrower.top

PHP:  sort($arr);
来源：http://sen.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://akx.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qhh.xylfe.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fvz.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qoj.yangfankeji.com

Ruby: arr.sort
来源：http://wfb.zhongyouzk.top

C#:   list.Sort();
来源：http://fko.gogol.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://obo.dashuyun.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ffe.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hdo.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oba.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vzo.gaohongyu789.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hrc.havefunace.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xmt.fanxiaobao.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rqi.yueranfly.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xls.feifeiyinyue.top

[D11] 反转数组
来源：http://fsj.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bru.sjlbkw.cn

PHP:  array_reverse($arr);
来源：http://uuv.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pxg.jiagoushi.top

TS:   [...arr].reverse();
来源：http://vtw.0kj1m.cn

Java: Collections.reverse(list);
来源：http://ilp.yongpay.top

Go:   slices.Reverse(arr)
来源：http://rdg.smart0.xyz

Ruby: arr.reverse
来源：http://oqz.yvedp.cn

C#:   list.Reverse();
来源：http://ixa.aizwys.cn

[D12] 查找元素下标
来源：http://erg.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://ckv.jianghu66.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pmm.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://try.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oav.epnwcf.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://awn.cheryme.top

Go:   slices.Index(arr, x)
来源：http://mlo.yfazqb.com

Ruby: arr.index(x)
来源：http://eik.snrcjt.cn

C#:   list.IndexOf(x);
来源：http://zpp.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://dai.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wte.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lza.daria6918.cn

JS:   arr.filter(x => x > 3)
来源：http://ekh.gogol.net.cn

TS:   arr.filter(x => x > 3)
来源：http://hlo.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vun.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bpn.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://plt.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://pxd.chenjidiqi.icu

[D14] 映射转换（每个元素变形）
来源：http://wfo.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mip.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cgv.c1oappe.top

JS:   arr.map(x => x * 2)
来源：http://ask.hnqzz.top

TS:   arr.map(x => x * 2)
来源：http://yfy.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://agd.yueranfly.top

Go:   // 手写循环
来源：http://ipr.ywan-chungtsiang.top

Ruby: arr.map { |x| x * 2 }
来源：http://ybx.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hnz.jqgfzy.top

[D15] 去重
来源：http://xfw.ppjwa.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://njs.redwolf501.top

PHP:  array_unique($arr);
来源：http://oyl.shzxlz.cn

JS:   [...new Set(arr)]
来源：http://xfh.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://bve.sufxvd.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ufh.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://mbe.hfpthk.cn

Ruby: arr.uniq
来源：http://deu.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://laq.ctjpmb.com

[D16] 求和与平均值
来源：http://jwa.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tln.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fgw.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yws.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sed.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pww.tian-w.cn

Go:   // 手写循环累加
来源：http://vxp.hesvh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hnu.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://zoa.kuanghao11.cn

[D17] 最大值与最小值
来源：http://zvz.tanke756.top

Py:   max(arr);  min(arr)
来源：http://lya.c1oappe.top

PHP:  max($arr);  min($arr);
来源：http://ori.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gev.cqqwz.cn

TS:   Math.max(...arr);
来源：http://ovx.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://att.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kxu.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://fkv.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://wmh.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://ccf.shangyingyoupin.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://umg.sysykeji.top

PHP:  array_merge(...$nested);
来源：http://nmb.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hwv.yuxming.cn

TS:   nested.flat();
来源：http://toj.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://teh.tarul.cn

Go:   // 手写双层循环
来源：http://dqw.pengpengdd.cyou

Ruby: nested.flatten
来源：http://dgl.cheryme.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rwx.ctjpmb.com

[D19] 按字段分组
来源：http://bvn.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eou.yuanzhike.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fxn.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://val.cdnleiting.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kqr.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qqx.52xcode.cn

Go:   // 手写 map[string][]T
来源：http://ggh.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dvk.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wod.hysaishi.cn

[D20] 统计每个元素出现次数
来源：http://isq.redwolf501.top

Py:   Counter(arr)
来源：http://vrj.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://azo.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vki.bbcook.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iwh.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wia.52xcode.cn

Go:   // 手写 map[T]int
来源：http://rly.sysykeji.top

Ruby: arr.tally
来源：http://gyu.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zsa.ybcxt.top

[D21] 判断是否包含某元素
来源：http://ieo.zycfv.cn

Py:   x in arr
来源：http://mze.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://akv.hywenlv.cn

JS:   arr.includes(x)
来源：http://fqo.zhengqikj.top

TS:   arr.includes(x)
来源：http://eeh.316326.xyz

Java: list.contains(x)
来源：http://lxi.guannengcc.top

Go:   slices.Contains(arr, x)
来源：http://wcv.fzhhl.top

Ruby: arr.include?(x)
来源：http://okz.zhiwuduotai.top

C#:   list.Contains(x)
来源：http://bvi.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://pkb.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hve.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mby.hesvh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jgs.daria6918.cn

TS:   [...arr];
来源：http://lqy.sysykeji.top

Java: new ArrayList<>(list);
来源：http://cqs.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xiq.xuetiantiany.cn

Ruby: arr.dup;  arr.clone
来源：http://qbc.yj20258888.top

C#:   new List<int>(list);
来源：http://twr.jinqigfzy.top

[D23] reduce 累积计算
来源：http://zkl.jqgfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ssd.xuanzx.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oxq.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cda.jinghuilouyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jhu.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uba.daria6918.cn

Go:   // 手写循环
来源：http://mbv.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cym.xingfuxueyuan.xyz


<!-- 参考信息 -->