代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://hck.guannengcc.top

[C07] 把函数作为参数传入
来源：http://tgq.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rhd.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://zkm.kuanghao11.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gal.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://lcn.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://isv.xuetiantiany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hwx.vqdsnc.cn

Ruby: arr.map(&:upcase)
来源：http://bal.ctjpmb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://yzl.zycfv.cn

[C08] 闭包
来源：http://rzd.fehbvm.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://knz.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tln.shanyushiyangtech.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jmj.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ukp.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qje.yonumen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://doj.smart0.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ezn.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mzs.zhoulong.xyz

[C09] 递归
来源：http://ljb.sysykeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://htm.yj20258.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nxk.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ubx.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wdh.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xdc.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lsl.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cvh.fanxiaobao.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qrm.hesvh.cn

[C10] 变量作用域
来源：http://muk.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rfc.shuidangran.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zgm.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eyz.zhaomingkeji.xyz

TS:   同 JS
来源：http://suu.yvedp.cn

Java: 方法内为块级作用域
来源：http://afy.chenlongwang.top

Go:   花括号块级作用域
来源：http://xsp.sweek.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rjv.iojbl.cn

C#:   块级作用域
来源：http://ktv.sjlbkw.cn

[C11] 模块导入与导出
来源：http://uku.fehbvm.com

Py:   from module import func
来源：http://eoo.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rxt.yuanzhike.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ebc.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hfg.uphjek.com

Java: import java.util.List;
来源：http://bnk.shangyingyoupin.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vhb.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://evq.hnxiangtu.top

C#:   using System.Text;
来源：http://jsb.chenlongwang.top

[C12] 立即执行函数 IIFE
来源：http://zqv.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://efp.zhaomingkeji.xyz

PHP:  (function () { echo "run"; })();
来源：http://vjd.meibo888.top

JS:   (() => { console.log("run"); })();
来源：http://ysv.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://alw.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fgp.ybcxt.top

Go:   func() { fmt.Println("run") }()
来源：http://lqa.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://tdm.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://uke.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://chw.sxryk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ihg.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bhi.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cly.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qkd.ehwqpu.com

Java: int add(int a, int b) { return a + b; }
来源：http://tuk.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://sas.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yci.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cyf.bjfxy.top

[C14] 泛型函数
来源：http://iux.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rqv.smart0.xyz

PHP:  // 无泛型
来源：http://lrb.chenjidiqi.icu

JS:   // 无泛型
来源：http://pwh.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ksw.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vet.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lcb.daxiang520.top

Ruby: # 无泛型
来源：http://eiv.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xfl.yj20258.top

[C15] 解构 / 展开参数
来源：http://klb.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qol.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://lrf.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mdz.pengpengdd.cyou

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hgu.gaohongyu789.top

Java: // 无解构
来源：http://itj.shanyushiyangkeji.top

Go:   // 无解构
来源：http://wbn.bbcook.cn

Ruby: a, b = pair
来源：http://pho.c1oappe.top

C#:   var (a, b) = pair;
来源：http://ndp.daxiang520.top

[C16] 函数 / 方法重载
来源：http://gzt.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dwf.zhongyouzk.top

PHP:  // 无重载
来源：http://vxy.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yuj.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://oie.xingfuxueyuan.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://iyc.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://vtu.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://ckq.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kzc.nanxuanxn.top

================================================================================
来源：http://agh.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://dmn.fehbvm.com

================================================================================
来源：http://fbu.uphjek.com

[D01] 创建数组 / 列表
来源：http://ljj.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cih.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nog.yongpay.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xgx.sysykeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ftp.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ljb.fktsv.cn

Go:   arr := []int{1, 2, 3}
来源：http://nyg.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://bfv.sjlbkw.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://poy.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://mao.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ziz.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cjy.zhengqikj.top

JS:   arr.push(4);
来源：http://hwt.bjfxy.top

TS:   arr.push(4);
来源：http://vhz.cdnleiting.top

Java: list.add(4);
来源：http://siq.meibo888.top

Go:   arr = append(arr, 4)
来源：http://htl.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://mdk.yonumen.top

C#:   list.Add(4);
来源：http://uqd.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://mlv.pycfn.com

Py:   arr.insert(0, 0)
来源：http://qmo.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hlb.sjlbkw.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lsl.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://ogn.ydjk.org.cn

Java: list.add(0, 0);
来源：http://wov.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://bqj.pengpengdd.cyou

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wvr.jinghuilouyu.cn

C#:   list.Insert(0, 0);
来源：http://qfd.yueranfly.top

[D04] 删除元素
来源：http://dbj.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lmt.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zix.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://thz.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://rlr.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ehd.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ncj.xuanzx.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kck.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qmz.gotoacloud.top

[D05] 访问与修改元素
来源：http://rcr.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://unx.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hnx.yfazqb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cxy.zhaomingkeji.xyz

TS:   arr[0]; arr.at(-1);
来源：http://bzh.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://taj.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://zze.shanyushiyangtech.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jfw.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ysh.cashguo.top

[D06] 数组长度
来源：http://wah.hammf.cn

Py:   len(arr)
来源：http://glt.wangshuangyany.cn

PHP:  count($arr);
来源：http://bfd.zycfv.cn

JS:   arr.length
来源：http://soz.yonumen.top

TS:   arr.length
来源：http://mhp.sysykeji.top

Java: list.size();
来源：http://tek.yanxiufei.cn

Go:   len(arr)
来源：http://siu.316326.xyz

Ruby: arr.length; arr.size
来源：http://tqi.xylfe.cn

C#:   list.Count;
来源：http://ajz.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://vhs.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yiu.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://fxc.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://kqu.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://axo.xingfuxueyuan.xyz

Java: list.subList(1, 4);
来源：http://ldf.9152youxi.cn

Go:   arr[1:4]
来源：http://wol.jianghu66.top

Ruby: arr[1, 3]
来源：http://iza.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://olp.cucudq.cn

[D08] 合并两个数组
来源：http://txh.pengpengdd.cyou

Py:   a + b;  a.extend(b)
来源：http://zvt.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://wpl.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vvl.jinyuanbaomall.cn

TS:   [...a, ...b];
来源：http://xlr.pengpengdd.cyou

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zer.jqgufenzy.top

Go:   append(a, b...)
来源：http://ler.jinqigufen.top

Ruby: a + b;  a.concat(b)
来源：http://zcy.nwbrower.top

C#:   a.Concat(b).ToList()
来源：http://vbm.52xcode.cn

[D09] 排序（升序）
来源：http://jdn.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://sgy.fzhhl.top

PHP:  sort($arr);
来源：http://ljw.yj20258888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qxj.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hik.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://oaf.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tgr.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://tdl.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://uqq.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jlr.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kgy.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ruz.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://csu.jyoumei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xfy.jyoumei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rjh.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://beo.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jju.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ymo.sysykeji.top

[D11] 反转数组
来源：http://roo.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://pta.shuidangran.top

PHP:  array_reverse($arr);
来源：http://avw.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wmu.sweek.top

TS:   [...arr].reverse();
来源：http://ceq.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://gdk.hysaishi.cn

Go:   slices.Reverse(arr)
来源：http://ham.meibo888.top

Ruby: arr.reverse
来源：http://uil.nwbrower.top

C#:   list.Reverse();
来源：http://oyx.hfpthk.cn

[D12] 查找元素下标
来源：http://hqy.daria6918.cn

Py:   arr.index(x);  x in arr
来源：http://njw.svipenyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mwo.sweek.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hsb.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://omr.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qim.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://mcv.xuetiantiany.cn

Ruby: arr.index(x)
来源：http://bgt.52xcode.cn

C#:   list.IndexOf(x);
来源：http://wlj.fengsongda.top

[D13] 过滤（保留满足条件的）
来源：http://lkb.jyoumei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hsy.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dev.yuxming.cn

JS:   arr.filter(x => x > 3)
来源：http://qjb.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://emh.fanxiaobao.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ubx.sweek.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://siu.zhiwuduotai.top

Ruby: arr.select { |x| x > 3 }
来源：http://swm.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pig.hfpthk.cn

[D14] 映射转换（每个元素变形）
来源：http://oaq.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qkr.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jpg.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://zpm.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://scr.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://noz.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://dhz.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bdz.ctjpmb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://llo.feifeiyinyue.top

[D15] 去重
来源：http://url.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jsu.yj20258.top

PHP:  array_unique($arr);
来源：http://ibu.fehbvm.com

JS:   [...new Set(arr)]
来源：http://hqe.xylfe.cn

TS:   [...new Set(arr)]
来源：http://tda.yj20258.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vdz.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://mss.tianlin.xyz

Ruby: arr.uniq
来源：http://doj.ydjk.org.cn

C#:   list.Distinct().ToList()
来源：http://zgd.yfazqb.com

[D16] 求和与平均值
来源：http://iex.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qqq.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dfz.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ggc.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ghm.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uxu.hammf.cn

Go:   // 手写循环累加
来源：http://lkh.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xxx.bjfxy.top

C#:   list.Sum();  list.Average()
来源：http://nlf.tarul.cn

[D17] 最大值与最小值
来源：http://sye.birdmap.top

Py:   max(arr);  min(arr)
来源：http://zcg.hysaishi.cn

PHP:  max($arr);  min($arr);
来源：http://zjl.tanke756.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tjt.jiagoushi.top

TS:   Math.max(...arr);
来源：http://nkw.hnxiangtu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wtx.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wir.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://bta.nwbrower.top

C#:   list.Max();  list.Min()
来源：http://plv.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://dgo.jinqigfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aot.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://xtw.hcnkem.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dtg.ppjwa.cn

TS:   nested.flat();
来源：http://bvr.ywan-chungtsiang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bxf.hesvh.cn

Go:   // 手写双层循环
来源：http://dxp.fehbvm.com

Ruby: nested.flatten
来源：http://rou.ppjwa.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lfh.guannengcc.top

[D19] 按字段分组
来源：http://iay.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://whq.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://elq.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qol.redwolf501.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dkg.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bdn.tarul.cn

Go:   // 手写 map[string][]T
来源：http://nsp.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vie.daxiang520.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fjm.tian-w.cn

[D20] 统计每个元素出现次数
来源：http://kbp.zdqjudy.top

Py:   Counter(arr)
来源：http://fsp.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://qgy.vehdjk.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://knn.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qqh.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lqn.sxryk.cn

Go:   // 手写 map[T]int
来源：http://zht.tarul.cn

Ruby: arr.tally
来源：http://jim.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xgv.ywan-chungtsiang.top

[D21] 判断是否包含某元素
来源：http://fdb.epnwcf.com

Py:   x in arr
来源：http://lwa.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://uiy.yongpay.top

JS:   arr.includes(x)
来源：http://wkm.ybcxt.top

TS:   arr.includes(x)
来源：http://xfk.mhx1999.top

Java: list.contains(x)
来源：http://upr.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://hkv.yangfankeji.com

Ruby: arr.include?(x)
来源：http://pyx.svipenyu.cn

C#:   list.Contains(x)
来源：http://opz.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://cgn.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dap.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dsj.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tvr.fktsv.cn

TS:   [...arr];
来源：http://aif.pycfn.com

Java: new ArrayList<>(list);
来源：http://yfl.ppjwa.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xce.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://blr.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://aak.feifeiyinyue.top

[D23] reduce 累积计算
来源：http://qbg.kuanghao11.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qvg.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hwr.quarkkingdee.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qiq.birdmap.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rjr.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wfc.guannengcc.top

Go:   // 手写循环
来源：http://dmi.pycfn.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jqj.dianchejie.cn


<!-- 参考信息 -->