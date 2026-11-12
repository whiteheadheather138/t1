代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mpf.quarkkingdee.top

Go:   return a, b
来源：http://nrf.zhongyouzk.top

Ruby: return a, b
来源：http://oai.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://nes.bjfxy.top

[C06] 匿名函数 / lambda
来源：http://cku.mhx1999.top

Py:   square = lambda x: x * x
来源：http://kzr.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ada.daxiang520.top

JS:   const square = x => x * x;
来源：http://gtj.jinyuanbaomall.cn

TS:   const square = (x: number): number => x * x;
来源：http://niw.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://naz.yj202588.top

Go:   sq := func(x int) int { return x * x }
来源：http://itw.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://pes.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://jtg.cheryme.top

[C07] 把函数作为参数传入
来源：http://efy.jyoumei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pwy.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://jzz.nanxuanxn.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://emo.cqqwz.cn

TS:   arr.map(String)
来源：http://hbj.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mwu.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://llf.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://utg.shangyingyoupin.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jsu.gogol.net.cn

[C08] 闭包
来源：http://efl.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cfs.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hia.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://occ.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yag.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mrg.cdnleiting.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oty.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aoz.xuetiantiany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cvk.nanxuanxn.top

[C09] 递归
来源：http://ujz.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rqi.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://loi.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cup.zhoulong.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yvl.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://trn.snrcjt.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://apy.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pjr.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bsn.jyoumei.cn

[C10] 变量作用域
来源：http://uhz.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mnz.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mhy.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lqy.birdmap.top

TS:   同 JS
来源：http://rtl.jiagoushi.top

Java: 方法内为块级作用域
来源：http://hon.zycfv.cn

Go:   花括号块级作用域
来源：http://mfh.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qir.wangshuangyany.cn

C#:   块级作用域
来源：http://wcx.zhixingplan.top

[C11] 模块导入与导出
来源：http://adt.daxiang520.top

Py:   from module import func
来源：http://ied.shanyushiyangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xgv.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yvy.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sxt.yuxming.cn

Java: import java.util.List;
来源：http://yrp.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qdr.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://ewy.sjlbkw.cn

C#:   using System.Text;
来源：http://qfj.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://cot.guowangkeji.top

Py:   (lambda: print("run"))()
来源：http://zke.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://mwv.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://zst.fengsongda.top

TS:   (() => { console.log("run"); })();
来源：http://znc.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gal.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://ycv.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://sbq.zhixingplan.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kpc.hysaishi.cn

[C13] 类型声明 / 类型注解
来源：http://gmo.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ldk.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://afs.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jtb.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tcz.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://txh.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://qfc.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qjx.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://agh.gogol.net.cn

[C14] 泛型函数
来源：http://xda.mhx1999.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blw.fehbvm.com

PHP:  // 无泛型
来源：http://ftc.tianlin.xyz

JS:   // 无泛型
来源：http://udf.guowangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hga.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jad.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://atg.gogol.net.cn

Ruby: # 无泛型
来源：http://jhg.9152youxi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://waq.tarul.cn

[C15] 解构 / 展开参数
来源：http://ikr.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qdd.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://ivf.sxryk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wph.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://znm.yj202588.top

Java: // 无解构
来源：http://oss.quarkkingdee.top

Go:   // 无解构
来源：http://vvy.fzhhl.top

Ruby: a, b = pair
来源：http://qab.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://yow.ctjpmb.com

[C16] 函数 / 方法重载
来源：http://dmr.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rzc.xziqi.cn

PHP:  // 无重载
来源：http://oeq.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ukw.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://eba.andypj.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://bzw.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://emk.hnqzz.top

Ruby: # 无重载：靠动态参数
来源：http://fsn.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sar.xingfuxueyuan.xyz

================================================================================
来源：http://kax.cheryme.top

D. 数组 / 列表 / 集合
来源：http://fvq.zhaomingkeji.xyz

================================================================================
来源：http://nat.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://ser.gzhubu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://eop.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vgt.yongpay.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iiv.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gft.bjfxy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lla.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://nnu.havefunace.top

Ruby: arr = [1, 2, 3]
来源：http://gsy.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ojt.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://vff.yuanzhike.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ihw.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gho.feifeiyinyue.top

JS:   arr.push(4);
来源：http://ban.nwbrower.top

TS:   arr.push(4);
来源：http://qtz.zhaomingkeji.xyz

Java: list.add(4);
来源：http://qge.fanxiaobao.xyz

Go:   arr = append(arr, 4)
来源：http://peh.zhoulong.xyz

Ruby: arr << 4; arr.push(5)
来源：http://vie.fzhhl.top

C#:   list.Add(4);
来源：http://cmq.fehbvm.com

[D03] 在指定位置插入元素
来源：http://wdd.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://xyu.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iap.yvedp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ysq.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://cjs.hnxiangtu.top

Java: list.add(0, 0);
来源：http://vwy.shuidangran.top

Go:   arr = append([]int{0}, arr...)
来源：http://qha.tianlin.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sxx.tanke756.top

C#:   list.Insert(0, 0);
来源：http://rzn.yj20258888.top

[D04] 删除元素
来源：http://ibv.yanxiufei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://szo.ivvv.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ydb.redwolf501.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gag.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://zud.xinyue.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tjn.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fua.ppjwa.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bwt.xziqi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vbq.yueranfly.top

[D05] 访问与修改元素
来源：http://phq.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xbm.c1oappe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://atu.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vmu.bbcook.cn

TS:   arr[0]; arr.at(-1);
来源：http://hvh.andypj.xyz

Java: list.get(0); list.set(0, 9);
来源：http://gba.haohaochexian.top

Go:   arr[0]; arr[0] = 9
来源：http://fae.jqgfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ikx.xinyue.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ewa.fktsv.cn

[D06] 数组长度
来源：http://lqz.c1oappe.top

Py:   len(arr)
来源：http://ggp.iojbl.cn

PHP:  count($arr);
来源：http://wdi.pengpengdd.cyou

JS:   arr.length
来源：http://npj.ctjpmb.com

TS:   arr.length
来源：http://sdx.meibo888.top

Java: list.size();
来源：http://luy.andypj.xyz

Go:   len(arr)
来源：http://iuo.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://nee.guowangkeji.top

C#:   list.Count;
来源：http://sxj.ywan-chungtsiang.top

[D07] 切片 / 取子数组
来源：http://ktq.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xte.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vjo.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://mcy.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://zyj.cheryme.top

Java: list.subList(1, 4);
来源：http://gjg.wangshuangyany.cn

Go:   arr[1:4]
来源：http://usp.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://pwr.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://qfe.uphjek.com

[D08] 合并两个数组
来源：http://hqd.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://oyp.zdbjq.cn

PHP:  array_merge($a, $b);
来源：http://adm.quarkkingdee.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xzk.yj202588.top

TS:   [...a, ...b];
来源：http://iuq.xylfe.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://frs.yj202588.top

Go:   append(a, b...)
来源：http://epv.shanyushiyangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://wiv.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://pzy.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://wdm.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://plb.sjlbkw.cn

PHP:  sort($arr);
来源：http://oxq.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mpc.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://slk.birdmap.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lvt.pycfn.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kyv.yj20258888.top

Ruby: arr.sort
来源：http://tqg.cdnleiting.top

C#:   list.Sort();
来源：http://wmx.hysaishi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vda.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://phc.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eim.yj20258.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sjt.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://csn.shzxlz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hus.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ekx.haohaochexian.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qfl.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vws.nwbrower.top

[D11] 反转数组
来源：http://eje.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kty.yj20258.top

PHP:  array_reverse($arr);
来源：http://hgl.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://axk.hfpthk.cn

TS:   [...arr].reverse();
来源：http://jqi.sysykeji.top

Java: Collections.reverse(list);
来源：http://iuf.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://kpm.yanxiufei.cn

Ruby: arr.reverse
来源：http://jjb.kuanghao11.cn

C#:   list.Reverse();
来源：http://cvy.tarul.cn

[D12] 查找元素下标
来源：http://brk.zdbjq.cn

Py:   arr.index(x);  x in arr
来源：http://dlw.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lqm.bbcook.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kcb.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zkf.xylfe.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jzw.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://lnn.tanke756.top

Ruby: arr.index(x)
来源：http://exa.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://twe.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://ike.9152youxi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jlb.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uff.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://wuy.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://fil.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uzx.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://roe.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://pjh.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qbu.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://ppe.c1oappe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://utx.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nxu.cashguo.top

JS:   arr.map(x => x * 2)
来源：http://utg.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://nvf.jiagoushi.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ftv.xziqi.cn

Go:   // 手写循环
来源：http://hif.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://mav.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eyg.daxiang520.top

[D15] 去重
来源：http://dly.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cbx.pengpengdd.cyou

PHP:  array_unique($arr);
来源：http://lus.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://igx.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://iev.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://swz.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kyb.jyoumei.cn

Ruby: arr.uniq
来源：http://pna.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://mje.kuanghao11.cn

[D16] 求和与平均值
来源：http://uaj.hywenlv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nio.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://snr.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uxq.jqgufenzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pyu.0kj1m.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ism.zhengqikj.top

Go:   // 手写循环累加
来源：http://jku.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lfu.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://ahl.52xcode.cn

[D17] 最大值与最小值
来源：http://nyk.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://lim.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://xib.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rxv.9152youxi.cn

TS:   Math.max(...arr);
来源：http://yyv.yanxiufei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zeo.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ymo.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://ohr.dashuyun.cn

C#:   list.Max();  list.Min()
来源：http://gig.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://uzw.xuanzx.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sex.mhx1999.top

PHP:  array_merge(...$nested);
来源：http://khb.yongpay.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xwu.hammf.cn

TS:   nested.flat();
来源：http://ewi.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hlb.tianlin.xyz

Go:   // 手写双层循环
来源：http://vyb.yfazqb.com

Ruby: nested.flatten
来源：http://wrs.dashuyun.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://khi.52xcode.cn

[D19] 按字段分组
来源：http://xhs.sxryk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://shh.epnwcf.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pfk.xuanzx.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cof.shanyushiyangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ytx.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sif.cdnleiting.top

Go:   // 手写 map[string][]T
来源：http://fwb.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ekg.ehwqpu.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yup.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://smz.tianlin.xyz

Py:   Counter(arr)
来源：http://tze.shanyushiyangtech.top

PHP:  array_count_values($arr);
来源：http://ifj.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ukz.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pbg.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fds.yfazqb.com

Go:   // 手写 map[T]int
来源：http://ziz.zhongyouzk.top

Ruby: arr.tally
来源：http://poe.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nvi.yueranfly.top

[D21] 判断是否包含某元素
来源：http://din.shzxlz.cn

Py:   x in arr
来源：http://agn.chenjidiqi.icu

PHP:  in_array($x, $arr, true);
来源：http://oqr.shanyushiyangtech.top

JS:   arr.includes(x)
来源：http://fth.c1oappe.top

TS:   arr.includes(x)
来源：http://ivl.c1oappe.top

Java: list.contains(x)
来源：http://jrd.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://cko.aizwys.cn

Ruby: arr.include?(x)
来源：http://srr.shuidangran.top

C#:   list.Contains(x)
来源：http://gbs.epnwcf.com

[D22] 复制数组（避免共享引用）
来源：http://fmw.zycfv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://stu.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nfw.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fjp.hysaishi.cn

TS:   [...arr];
来源：http://rsl.yj20258.top


<!-- 参考信息 -->