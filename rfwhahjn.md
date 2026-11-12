代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pny.tanke756.top

Go:   return a, b
来源：http://bdk.yanxiufei.cn

Ruby: return a, b
来源：http://hgq.shangyingyoupin.top

C#:   return (a, b);              // ValueTuple
来源：http://nbp.bbcook.cn

[C06] 匿名函数 / lambda
来源：http://yye.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://hud.zhengqikj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dgj.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://sie.guowangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://lyd.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gab.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://svq.epnwcf.com

Ruby: square = ->(x) { x * x }
来源：http://omv.smart0.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ylh.ydjk.org.cn

[C07] 把函数作为参数传入
来源：http://aza.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zmh.mhx1999.top

PHP:  array_map("strtoupper", $arr);
来源：http://snr.feifeiyinyue.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sop.cqqwz.cn

TS:   arr.map(String)
来源：http://zoo.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lwa.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gmy.sweek.top

Ruby: arr.map(&:upcase)
来源：http://upj.ivvv.top

C#:   arr.Select(s => s.ToUpper())
来源：http://nax.fzhhl.top

[C08] 闭包
来源：http://orq.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://klp.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mjn.havefunace.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hbp.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lzk.iojbl.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sof.cashguo.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kwp.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jtn.ppjwa.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qlc.epnwcf.com

[C09] 递归
来源：http://nvs.nwbrower.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ofw.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tyx.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yky.yanxiufei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aws.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uqs.hongshengwenyu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vsw.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oyi.mhx1999.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ceq.redwolf501.top

[C10] 变量作用域
来源：http://lis.bjfxy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sji.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vtl.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qhl.bjfxy.top

TS:   同 JS
来源：http://ckj.hnqzz.top

Java: 方法内为块级作用域
来源：http://ajf.cucudq.cn

Go:   花括号块级作用域
来源：http://nss.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fjx.yuanzhike.top

C#:   块级作用域
来源：http://brl.havefunace.top

[C11] 模块导入与导出
来源：http://nfp.yuanzhike.top

Py:   from module import func
来源：http://ejg.ydjk.org.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://asb.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://buc.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dje.yuxming.cn

Java: import java.util.List;
来源：http://xbq.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://goe.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://zbd.jqgfzy.top

C#:   using System.Text;
来源：http://lgh.yj20258.top

[C12] 立即执行函数 IIFE
来源：http://ocq.yongpay.top

Py:   (lambda: print("run"))()
来源：http://mol.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://krd.ctjpmb.com

JS:   (() => { console.log("run"); })();
来源：http://qpt.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://lpu.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://inq.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://vqo.hnqzz.top

Ruby: -> { puts "run" }.call
来源：http://hsi.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xmp.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://wws.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xxv.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ady.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fdx.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xch.fzhhl.top

Java: int add(int a, int b) { return a + b; }
来源：http://ofo.zhengqikj.top

Go:   func add(a, b int) int
来源：http://rua.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qmu.xylfe.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gvh.jqgfzy.top

[C14] 泛型函数
来源：http://yff.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vdq.zdqjudy.top

PHP:  // 无泛型
来源：http://hdh.yj20258888.top

JS:   // 无泛型
来源：http://osv.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tul.meibo888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iyr.pengpengdd.cyou

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zgq.shanyushiyangtech.top

Ruby: # 无泛型
来源：http://hyt.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jjr.svipenyu.cn

[C15] 解构 / 展开参数
来源：http://fvl.daria6918.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ptt.guowangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://tfb.fanxiaobao.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://quo.xuanzx.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cft.nwbrower.top

Java: // 无解构
来源：http://ltg.nanxuanxn.top

Go:   // 无解构
来源：http://fxx.yuxming.cn

Ruby: a, b = pair
来源：http://ajh.smart0.xyz

C#:   var (a, b) = pair;
来源：http://sxr.kuanghao11.cn

[C16] 函数 / 方法重载
来源：http://vqj.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xwm.ywan-chungtsiang.top

PHP:  // 无重载
来源：http://cwe.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tbu.zhongyouzk.top

TS:   // 用联合类型或重载签名声明
来源：http://mhz.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tme.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://htd.jqgfzy.top

Ruby: # 无重载：靠动态参数
来源：http://hhu.pycfn.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://fnk.fzhhl.top

================================================================================
来源：http://vfg.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://aqh.bjfxy.top

================================================================================
来源：http://kmd.zycfv.cn

[D01] 创建数组 / 列表
来源：http://wtu.ivvv.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zyl.yuanzhike.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ryj.sjlbkw.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nfc.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xxf.zhixingplan.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pjt.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://ojg.pycfn.com

Ruby: arr = [1, 2, 3]
来源：http://vyj.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bbm.feifeiyinyue.top

[D02] 追加元素到末尾
来源：http://xxv.smart0.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://imx.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hiv.ctjpmb.com

JS:   arr.push(4);
来源：http://gbm.guannengcc.top

TS:   arr.push(4);
来源：http://juw.zdbjq.cn

Java: list.add(4);
来源：http://fvi.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://evu.quarkkingdee.top

Ruby: arr << 4; arr.push(5)
来源：http://mrb.aizwys.cn

C#:   list.Add(4);
来源：http://pax.chenjidiqi.icu

[D03] 在指定位置插入元素
来源：http://prw.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://kpj.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://doi.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kyn.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://gnl.sweek.top

Java: list.add(0, 0);
来源：http://gez.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://xlz.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yfz.daxiang520.top

C#:   list.Insert(0, 0);
来源：http://yub.pengpengdd.cyou

[D04] 删除元素
来源：http://der.pengpengdd.cyou

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rjg.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://doe.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nsg.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://tex.fanxiaobao.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://poj.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://app.yangfankeji.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gri.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jkv.kuanghao11.cn

[D05] 访问与修改元素
来源：http://kqt.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uzg.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cgk.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://txq.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://frg.hnxiangtu.top

Java: list.get(0); list.set(0, 9);
来源：http://ejk.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://ruc.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zoa.tarul.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hts.yongpay.top

[D06] 数组长度
来源：http://yre.jqgfzy.top

Py:   len(arr)
来源：http://ydu.kuanghao11.cn

PHP:  count($arr);
来源：http://bux.9152youxi.cn

JS:   arr.length
来源：http://fqc.gogol.net.cn

TS:   arr.length
来源：http://efm.hesvh.cn

Java: list.size();
来源：http://acv.wangdashe.top

Go:   len(arr)
来源：http://xkm.xziqi.cn

Ruby: arr.length; arr.size
来源：http://hfd.svipenyu.cn

C#:   list.Count;
来源：http://rts.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://flu.dianchejie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://agj.zdbjq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://aiy.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://oti.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://hrr.bjfxy.top

Java: list.subList(1, 4);
来源：http://quw.hcnkem.com

Go:   arr[1:4]
来源：http://lzn.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://gpt.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://mla.zhaomingkeji.xyz

[D08] 合并两个数组
来源：http://bxb.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://ckx.ehwqpu.com

PHP:  array_merge($a, $b);
来源：http://tks.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://tnj.uphjek.com

TS:   [...a, ...b];
来源：http://wmn.316326.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dhy.c1oappe.top

Go:   append(a, b...)
来源：http://gqn.yj20258.top

Ruby: a + b;  a.concat(b)
来源：http://frn.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://yqs.tarul.cn

[D09] 排序（升序）
来源：http://otg.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://jut.yuxming.cn

PHP:  sort($arr);
来源：http://pud.zhengqikj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bkp.jinqigufen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gyi.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ybu.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gae.sweek.top

Ruby: arr.sort
来源：http://qyd.tian-w.cn

C#:   list.Sort();
来源：http://tgr.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mud.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://amf.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iqh.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lcw.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mxo.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://frt.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iug.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wbi.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lgc.zhijiandao.cn

[D11] 反转数组
来源：http://xhc.shuidangran.top

Py:   arr[::-1];  arr.reverse()
来源：http://tcp.ydjk.org.cn

PHP:  array_reverse($arr);
来源：http://zrv.jlsjyb.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ggu.tanke756.top

TS:   [...arr].reverse();
来源：http://sbt.hywenlv.cn

Java: Collections.reverse(list);
来源：http://etu.ehwqpu.com

Go:   slices.Reverse(arr)
来源：http://qcp.shzxlz.cn

Ruby: arr.reverse
来源：http://btp.zhaomingkeji.xyz

C#:   list.Reverse();
来源：http://xhk.hcnkem.com

[D12] 查找元素下标
来源：http://wmd.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://pgg.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ceg.zhixingplan.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lvy.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mwf.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://axp.tanke756.top

Go:   slices.Index(arr, x)
来源：http://rxi.gzhubu.top

Ruby: arr.index(x)
来源：http://oph.ybcxt.top

C#:   list.IndexOf(x);
来源：http://dkv.yj202588.top

[D13] 过滤（保留满足条件的）
来源：http://ivo.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://axu.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jgd.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://xya.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://zpc.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jgj.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yud.pycfn.com

Ruby: arr.select { |x| x > 3 }
来源：http://kiw.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://whe.yj20258888.top

[D14] 映射转换（每个元素变形）
来源：http://xkg.gzhubu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gnq.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cfu.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://akc.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://lvg.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pfr.jqgufenzy.top

Go:   // 手写循环
来源：http://pwp.ydjk.org.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sak.ybcxt.top

C#:   list.Select(x => x * 2).ToList()
来源：http://you.feifeiyinyue.top

[D15] 去重
来源：http://pnz.jqgufenzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jnc.chenlongwang.top

PHP:  array_unique($arr);
来源：http://ucv.fanxiaobao.xyz

JS:   [...new Set(arr)]
来源：http://pur.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://qgx.gaohongyu789.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kiz.c1oappe.top

Go:   // 用 map[T]struct{} 手写
来源：http://cyb.yanxiufei.cn

Ruby: arr.uniq
来源：http://qdn.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://eku.hnxiangtu.top

[D16] 求和与平均值
来源：http://lzt.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wev.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cfu.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iry.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hwn.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dwc.jlsjyb.cn

Go:   // 手写循环累加
来源：http://myo.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zyf.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://nnc.ydzc1.top

[D17] 最大值与最小值
来源：http://tkx.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://ufn.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://hfp.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sra.gogol.net.cn

TS:   Math.max(...arr);
来源：http://iaj.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rzv.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ryr.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://tkj.yj20258.top

C#:   list.Max();  list.Min()
来源：http://gaz.aibaodan.cn

[D18] 扁平化嵌套数组
来源：http://rqp.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lql.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://qli.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kdp.hesvh.cn

TS:   nested.flat();
来源：http://jgx.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://duc.redwolf501.top

Go:   // 手写双层循环
来源：http://cia.jinqigufen.top

Ruby: nested.flatten
来源：http://twj.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://khn.yueranfly.top

[D19] 按字段分组
来源：http://ljv.shzxlz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xzz.xingfuxueyuan.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oyn.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://erw.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://hft.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dgf.zycfv.cn

Go:   // 手写 map[string][]T
来源：http://zhz.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rab.ydzc1.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uhh.tian-w.cn

[D20] 统计每个元素出现次数
来源：http://dud.pengpengdd.cyou

Py:   Counter(arr)
来源：http://wiy.zhoulong.xyz

PHP:  array_count_values($arr);
来源：http://ius.chenlongwang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ayy.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kwx.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jpc.aizwys.cn

Go:   // 手写 map[T]int
来源：http://rvh.shzxlz.cn

Ruby: arr.tally
来源：http://hus.gogol.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iil.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://stm.fktsv.cn

Py:   x in arr
来源：http://wzf.kuanghao11.cn

PHP:  in_array($x, $arr, true);
来源：http://lky.jqgufenzy.top

JS:   arr.includes(x)
来源：http://djq.bjfxy.top

TS:   arr.includes(x)
来源：http://slo.zdqjudy.top

Java: list.contains(x)
来源：http://tmg.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://bzm.sxryk.cn

Ruby: arr.include?(x)
来源：http://ajp.fktsv.cn

C#:   list.Contains(x)
来源：http://idy.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://aeo.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mfp.jqgfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://piw.hesvh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xnf.hongshengwenyu.top

TS:   [...arr];
来源：http://axk.hfpthk.cn


<!-- 参考信息 -->