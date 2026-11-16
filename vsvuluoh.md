代发 wailian999

[C06] 匿名函数 / lambda
来源：http://vec.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://mha.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://eel.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://suj.yonumen.top

TS:   const square = (x: number): number => x * x;
来源：http://vht.tianlin.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://row.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kiz.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://rqb.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kyo.zhiwuduotai.top

[C07] 把函数作为参数传入
来源：http://tot.yonumen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bmy.shuidangran.top

PHP:  array_map("strtoupper", $arr);
来源：http://gae.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cnz.kuanghao11.cn

TS:   arr.map(String)
来源：http://ekw.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jjr.chenjidiqi.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mhq.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://pjn.xziqi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://apj.sufxvd.cn

[C08] 闭包
来源：http://wjf.ydzc1.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nff.cqqwz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nhp.yvedp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rci.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://alm.pengpengdd.cyou

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tzt.yonumen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://evv.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zfp.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qkx.havefunace.top

[C09] 递归
来源：http://tfx.zycfv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ais.ybcxt.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wra.chenjidiqi.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ruh.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uok.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mae.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pde.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sin.cdnleiting.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dup.tarul.cn

[C10] 变量作用域
来源：http://ous.zhijiandao.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yno.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://igp.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sqa.yonumen.top

TS:   同 JS
来源：http://zmo.haohaochexian.top

Java: 方法内为块级作用域
来源：http://zgv.sysykeji.top

Go:   花括号块级作用域
来源：http://tuo.epnwcf.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iwv.xinyue.icu

C#:   块级作用域
来源：http://wjq.vehdjk.com

[C11] 模块导入与导出
来源：http://hgz.hywenlv.cn

Py:   from module import func
来源：http://ktb.gogol.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kdb.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kmh.ctjpmb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xpb.yj20258888.top

Java: import java.util.List;
来源：http://elv.shangyingyoupin.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uqw.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://aju.316326.xyz

C#:   using System.Text;
来源：http://knt.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://oug.ybcxt.top

Py:   (lambda: print("run"))()
来源：http://rrd.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://foe.jyoumei.cn

JS:   (() => { console.log("run"); })();
来源：http://ezl.shzxlz.cn

TS:   (() => { console.log("run"); })();
来源：http://ums.yangfankeji.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://clm.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://xmr.gogol.net.cn

Ruby: -> { puts "run" }.call
来源：http://dur.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zjz.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://tda.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dsd.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ijk.daria6918.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kuz.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lke.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://ows.mhx1999.top

Go:   func add(a, b int) int
来源：http://xur.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qms.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://rzm.yonumen.top

[C14] 泛型函数
来源：http://hdc.cqqwz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xzv.hnqzz.top

PHP:  // 无泛型
来源：http://aor.daxiang520.top

JS:   // 无泛型
来源：http://drc.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ozn.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pkj.bjfxy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://otr.guannengcc.top

Ruby: # 无泛型
来源：http://cry.ehwqpu.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wui.quarkkingdee.top

[C15] 解构 / 展开参数
来源：http://xzp.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fws.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://anz.tian-w.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gar.gotoacloud.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zse.pycfn.com

Java: // 无解构
来源：http://dnw.shuidangran.top

Go:   // 无解构
来源：http://xxn.yangfankeji.com

Ruby: a, b = pair
来源：http://nay.cqqwz.cn

C#:   var (a, b) = pair;
来源：http://vna.xuanzx.com

[C16] 函数 / 方法重载
来源：http://vvw.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tzl.aibaodan.cn

PHP:  // 无重载
来源：http://qli.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://whb.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://yaz.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://brj.jinqigfzy.top

Go:   // 无重载：用不同函数名
来源：http://vdv.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://tla.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lpp.zdbjq.cn

================================================================================
来源：http://ndx.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://mnp.bbcook.cn

================================================================================
来源：http://slj.yvedp.cn

[D01] 创建数组 / 列表
来源：http://ldn.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dhv.chenzaomai.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ghy.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qch.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kan.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ltr.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://ytg.zhengqikj.top

Ruby: arr = [1, 2, 3]
来源：http://yfz.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ysv.dashuyun.cn

[D02] 追加元素到末尾
来源：http://wda.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xhz.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lea.hywenlv.cn

JS:   arr.push(4);
来源：http://urb.bbcook.cn

TS:   arr.push(4);
来源：http://jmu.fengsongda.top

Java: list.add(4);
来源：http://qdk.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://gct.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://dgo.gaohongyu789.top

C#:   list.Add(4);
来源：http://cgi.yj20258.top

[D03] 在指定位置插入元素
来源：http://npb.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://ssd.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fcu.ppjwa.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rmc.shzxlz.cn

TS:   arr.splice(0, 0, 0);
来源：http://rwp.ybcxt.top

Java: list.add(0, 0);
来源：http://ilq.yangfankeji.com

Go:   arr = append([]int{0}, arr...)
来源：http://iqu.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pns.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://zjc.zhijiandao.cn

[D04] 删除元素
来源：http://lsb.yj20258888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://spn.tian-w.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hru.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://skk.sufxvd.cn

TS:   arr.splice(0, 1);
来源：http://hua.xinyue.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ank.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pwb.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gll.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aov.chenlongwang.top

[D05] 访问与修改元素
来源：http://vxg.birdmap.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://amh.yangfankeji.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://asx.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rtg.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://cec.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://sqi.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://zpc.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cxw.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ieh.epnwcf.com

[D06] 数组长度
来源：http://hjj.fanxiaobao.xyz

Py:   len(arr)
来源：http://ubk.xinyue.icu

PHP:  count($arr);
来源：http://vmh.nwbrower.top

JS:   arr.length
来源：http://qgt.cucudq.cn

TS:   arr.length
来源：http://fvk.meibo888.top

Java: list.size();
来源：http://vpe.guannengcc.top

Go:   len(arr)
来源：http://uqx.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://fvs.fehbvm.com

C#:   list.Count;
来源：http://duo.yonumen.top

[D07] 切片 / 取子数组
来源：http://hxf.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://umq.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://ayg.gaohongyu789.top

JS:   arr.slice(1, 4);
来源：http://gdk.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://ryj.fzhhl.top

Java: list.subList(1, 4);
来源：http://kfw.bjfxy.top

Go:   arr[1:4]
来源：http://fbg.gzhubu.top

Ruby: arr[1, 3]
来源：http://kgc.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://vgt.quarkkingdee.top

[D08] 合并两个数组
来源：http://tvf.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://dwy.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://izd.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://gun.mhx1999.top

TS:   [...a, ...b];
来源：http://wye.fehbvm.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gfl.0kj1m.cn

Go:   append(a, b...)
来源：http://kku.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://tpo.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://mxn.ppjwa.cn

[D09] 排序（升序）
来源：http://spa.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://nvk.jinqigfzy.top

PHP:  sort($arr);
来源：http://wao.sufxvd.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hen.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wgy.uphjek.com

Java: Collections.sort(list);  list.sort(null);
来源：http://cdf.epnwcf.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uhs.ppjwa.cn

Ruby: arr.sort
来源：http://qcz.cucudq.cn

C#:   list.Sort();
来源：http://gxp.tian-w.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ijj.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fnp.redwolf501.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://egu.yj202588.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wyy.uphjek.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dsx.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bks.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://djo.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xux.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ljr.ehwqpu.com

[D11] 反转数组
来源：http://brs.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://smf.kuanghao11.cn

PHP:  array_reverse($arr);
来源：http://ikv.fengsongda.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xwd.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://jbq.0kj1m.cn

Java: Collections.reverse(list);
来源：http://jhz.wangshuangyany.cn

Go:   slices.Reverse(arr)
来源：http://tta.9152youxi.cn

Ruby: arr.reverse
来源：http://mbw.ppjwa.cn

C#:   list.Reverse();
来源：http://vus.yfazqb.com

[D12] 查找元素下标
来源：http://huq.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://jwe.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mno.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://adr.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://reh.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ovc.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://wun.yonumen.top

Ruby: arr.index(x)
来源：http://xjr.hongshengwenyu.top

C#:   list.IndexOf(x);
来源：http://wcq.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://smc.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ywx.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oux.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://azb.zhixingplan.top

TS:   arr.filter(x => x > 3)
来源：http://ybe.yuanzhike.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mfp.meibo888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kqm.yj20258.top

Ruby: arr.select { |x| x > 3 }
来源：http://fki.jiagoushi.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pob.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://lck.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nwj.ydjk.org.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yki.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://esj.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://pmk.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sqi.c1oappe.top

Go:   // 手写循环
来源：http://gis.xuetiantiany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yfy.hcnkem.com

C#:   list.Select(x => x * 2).ToList()
来源：http://bqa.dashuyun.cn

[D15] 去重
来源：http://ysn.sjlbkw.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wfy.vehdjk.com

PHP:  array_unique($arr);
来源：http://slp.tanke756.top

JS:   [...new Set(arr)]
来源：http://emw.yonumen.top

TS:   [...new Set(arr)]
来源：http://tyy.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mik.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zkv.gaohongyu789.top

Ruby: arr.uniq
来源：http://wre.fengsongda.top

C#:   list.Distinct().ToList()
来源：http://kca.c1oappe.top

[D16] 求和与平均值
来源：http://vwr.snrcjt.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qbw.tianlin.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hsa.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eyv.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rhm.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ybc.snrcjt.cn

Go:   // 手写循环累加
来源：http://rcx.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://srg.chenzaomai.com

C#:   list.Sum();  list.Average()
来源：http://dxd.cheryme.top

[D17] 最大值与最小值
来源：http://fvj.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://nvf.yfazqb.com

PHP:  max($arr);  min($arr);
来源：http://skc.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fwh.yj202588.top

TS:   Math.max(...arr);
来源：http://wef.yfazqb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://dbd.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://otb.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://qyj.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://jrd.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://dop.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://syq.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://jpy.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pnu.ybcxt.top

TS:   nested.flat();
来源：http://xwa.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://moz.vqdsnc.cn

Go:   // 手写双层循环
来源：http://njz.aibaodan.cn

Ruby: nested.flatten
来源：http://fga.svipenyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bsn.yuanzhike.top

[D19] 按字段分组
来源：http://vnp.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dhu.tian-w.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://noi.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xsi.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://per.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lwl.hongshengwenyu.top

Go:   // 手写 map[string][]T
来源：http://wiz.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wxh.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ctv.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://tjj.gogol.net.cn

Py:   Counter(arr)
来源：http://vuo.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://tzh.jqgufenzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rez.mhx1999.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hko.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aoa.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://avu.yuanzhike.top

Ruby: arr.tally
来源：http://jhi.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rmi.fehbvm.com

[D21] 判断是否包含某元素
来源：http://bnh.shanyushiyangkeji.top

Py:   x in arr
来源：http://pwa.ywan-chungtsiang.top

PHP:  in_array($x, $arr, true);
来源：http://nym.shuidangran.top

JS:   arr.includes(x)
来源：http://pls.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://vha.yvedp.cn

Java: list.contains(x)
来源：http://wxx.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://inq.316326.xyz

Ruby: arr.include?(x)
来源：http://ikw.xuanzx.com

C#:   list.Contains(x)
来源：http://gji.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://yux.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lln.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ccn.dianchejie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bam.shanyushiyangtech.top

TS:   [...arr];
来源：http://zus.tarul.cn

Java: new ArrayList<>(list);
来源：http://ace.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://klm.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://fcj.zdbjq.cn

C#:   new List<int>(list);
来源：http://hce.jqgufenzy.top


<!-- 参考信息 -->