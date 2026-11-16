代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tvu.zhoulong.xyz

Go:   return a, b
来源：http://cwv.feifeiyinyue.top

Ruby: return a, b
来源：http://mlw.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://psh.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://nui.epnwcf.com

Py:   square = lambda x: x * x
来源：http://ezy.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bmb.bjfxy.top

JS:   const square = x => x * x;
来源：http://plk.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://xxs.jinghuilouyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wgf.chenzaomai.com

Go:   sq := func(x int) int { return x * x }
来源：http://vev.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://ctz.cdnleiting.top

C#:   Func<int, int> square = x => x * x;
来源：http://xrw.jianghu66.top

[C07] 把函数作为参数传入
来源：http://pqp.hysaishi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wuq.jinqigfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://yoo.pycfn.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nyw.andypj.xyz

TS:   arr.map(String)
来源：http://tic.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hru.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hdf.quarkkingdee.top

Ruby: arr.map(&:upcase)
来源：http://inc.xuanzx.com

C#:   arr.Select(s => s.ToUpper())
来源：http://utt.dianchejie.cn

[C08] 闭包
来源：http://ong.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://twx.zhaomingkeji.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://odt.mhx1999.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rcr.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kzs.zycfv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lof.fktsv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cod.yvedp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mho.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bpk.yuanzhike.top

[C09] 递归
来源：http://gkh.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zds.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uda.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vhb.yangfankeji.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nym.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vyl.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://psp.sysykeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://crz.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hfs.pengpengdd.cyou

[C10] 变量作用域
来源：http://eax.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sbq.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vus.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nai.c1oappe.top

TS:   同 JS
来源：http://fti.chenlongwang.top

Java: 方法内为块级作用域
来源：http://fuf.yj202588.top

Go:   花括号块级作用域
来源：http://bms.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yno.nanxinkj.top

C#:   块级作用域
来源：http://wpv.haohaochexian.top

[C11] 模块导入与导出
来源：http://qid.sweek.top

Py:   from module import func
来源：http://xku.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pgg.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hns.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lgq.hywenlv.cn

Java: import java.util.List;
来源：http://eqe.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ngj.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://fcn.zhijiandao.cn

C#:   using System.Text;
来源：http://drq.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://myn.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://rpr.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://qhe.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://olx.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://bnd.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hzv.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://wnq.sysykeji.top

Ruby: -> { puts "run" }.call
来源：http://bbw.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://zsi.jyoumei.cn

[C13] 类型声明 / 类型注解
来源：http://puw.tianlin.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hhw.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uam.tian-w.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tzx.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kge.shanyushiyangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://wml.meibo888.top

Go:   func add(a, b int) int
来源：http://bbl.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zxh.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://ebu.yj20258888.top

[C14] 泛型函数
来源：http://ofw.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dra.chenzaomai.com

PHP:  // 无泛型
来源：http://aba.sjlbkw.cn

JS:   // 无泛型
来源：http://wbv.dianchejie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rhe.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://czy.yongpay.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://utm.jiagoushi.top

Ruby: # 无泛型
来源：http://fuw.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ban.sweek.top

[C15] 解构 / 展开参数
来源：http://ktl.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://opb.ehwqpu.com

PHP:  [$a, $b] = $pair;
来源：http://hak.jiagoushi.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vny.tarul.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://smg.sxryk.cn

Java: // 无解构
来源：http://nep.jlsjyb.cn

Go:   // 无解构
来源：http://oov.jlsjyb.cn

Ruby: a, b = pair
来源：http://ngd.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://aep.smart0.xyz

[C16] 函数 / 方法重载
来源：http://gxy.fzhhl.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tdx.zdbjq.cn

PHP:  // 无重载
来源：http://cgp.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ble.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://ism.wangdashe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xdb.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://bip.xziqi.cn

Ruby: # 无重载：靠动态参数
来源：http://wtk.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rdv.wangdashe.top

================================================================================
来源：http://bfq.52xcode.cn

D. 数组 / 列表 / 集合
来源：http://xng.xuanzx.com

================================================================================
来源：http://fde.tian-w.cn

[D01] 创建数组 / 列表
来源：http://cro.jinyuanbaomall.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://euf.nanxuanxn.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xxs.9152youxi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lhq.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ixq.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ctb.aibaodan.cn

Go:   arr := []int{1, 2, 3}
来源：http://jrm.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://mku.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://neh.shuidangran.top

[D02] 追加元素到末尾
来源：http://wea.nwbrower.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nwk.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ruo.sysykeji.top

JS:   arr.push(4);
来源：http://ccp.yj20258888.top

TS:   arr.push(4);
来源：http://yyn.gzhubu.top

Java: list.add(4);
来源：http://yqx.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://ule.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://diu.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://bnb.xuanzx.com

[D03] 在指定位置插入元素
来源：http://xwh.shzxlz.cn

Py:   arr.insert(0, 0)
来源：http://vql.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iqc.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mfj.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://hzv.hcnkem.com

Java: list.add(0, 0);
来源：http://kjz.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aex.sufxvd.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ywg.hcnkem.com

C#:   list.Insert(0, 0);
来源：http://wfm.svipenyu.cn

[D04] 删除元素
来源：http://xzk.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://waq.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nya.vehdjk.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mzs.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://tvo.316326.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gbk.iojbl.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xet.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://msk.hammf.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ncl.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://rxk.ydzc1.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://syc.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://emc.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lvy.pycfn.com

TS:   arr[0]; arr.at(-1);
来源：http://mdr.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://fbi.cdnleiting.top

Go:   arr[0]; arr[0] = 9
来源：http://rlt.zhengqikj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vhl.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mio.cashguo.top

[D06] 数组长度
来源：http://afk.zdbjq.cn

Py:   len(arr)
来源：http://emv.quarkkingdee.top

PHP:  count($arr);
来源：http://yll.hammf.cn

JS:   arr.length
来源：http://fjv.52xcode.cn

TS:   arr.length
来源：http://gxk.vehdjk.com

Java: list.size();
来源：http://skb.guowangkeji.top

Go:   len(arr)
来源：http://vgz.ctjpmb.com

Ruby: arr.length; arr.size
来源：http://xgj.zdqjudy.top

C#:   list.Count;
来源：http://aft.epnwcf.com

[D07] 切片 / 取子数组
来源：http://yzb.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qgv.yvedp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hdz.meibo888.top

JS:   arr.slice(1, 4);
来源：http://vdt.ehwqpu.com

TS:   arr.slice(1, 4);
来源：http://eic.tianlin.xyz

Java: list.subList(1, 4);
来源：http://ywd.chenzaomai.com

Go:   arr[1:4]
来源：http://tti.hfpthk.cn

Ruby: arr[1, 3]
来源：http://xav.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://phu.zhijiandao.cn

[D08] 合并两个数组
来源：http://jrk.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://jlq.uphjek.com

PHP:  array_merge($a, $b);
来源：http://qyk.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://klt.hnqzz.top

TS:   [...a, ...b];
来源：http://ofj.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://anz.xylfe.cn

Go:   append(a, b...)
来源：http://kgj.wangshuangyany.cn

Ruby: a + b;  a.concat(b)
来源：http://qwa.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://kxs.shuidangran.top

[D09] 排序（升序）
来源：http://bjc.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://luv.shzxlz.cn

PHP:  sort($arr);
来源：http://xwg.smart0.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pdk.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jwn.wangdashe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jwt.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vnq.shzxlz.cn

Ruby: arr.sort
来源：http://skd.hysaishi.cn

C#:   list.Sort();
来源：http://uje.nwbrower.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hwj.chenjidiqi.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://buy.jqgufenzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uem.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ncc.mhx1999.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://okg.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nex.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qpo.tian-w.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fyj.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tdx.316326.xyz

[D11] 反转数组
来源：http://jvt.sxryk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gno.yj20258.top

PHP:  array_reverse($arr);
来源：http://nde.hfpthk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jxg.ehwqpu.com

TS:   [...arr].reverse();
来源：http://ddl.zdbjq.cn

Java: Collections.reverse(list);
来源：http://vzv.xziqi.cn

Go:   slices.Reverse(arr)
来源：http://vfu.xziqi.cn

Ruby: arr.reverse
来源：http://zke.xingfuxueyuan.xyz

C#:   list.Reverse();
来源：http://mzc.quarkkingdee.top

[D12] 查找元素下标
来源：http://kdv.cucudq.cn

Py:   arr.index(x);  x in arr
来源：http://nlr.yangfankeji.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lbm.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xcs.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://epo.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kry.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://scr.hywenlv.cn

Ruby: arr.index(x)
来源：http://muv.gogol.net.cn

C#:   list.IndexOf(x);
来源：http://cei.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://qrg.daria6918.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jgp.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qmr.mhx1999.top

JS:   arr.filter(x => x > 3)
来源：http://jiu.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://hpl.cashguo.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hfw.yuxming.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rex.kuanghao11.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mcg.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://khe.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://pud.yonumen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ylh.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rll.hysaishi.cn

JS:   arr.map(x => x * 2)
来源：http://wpi.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://ovn.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://mch.yj20258888.top

Go:   // 手写循环
来源：http://sjr.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://tdp.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ixj.zhaomingkeji.xyz

[D15] 去重
来源：http://ogs.gaohongyu789.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sbj.nanxinkj.top

PHP:  array_unique($arr);
来源：http://eop.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://clo.fengsongda.top

TS:   [...new Set(arr)]
来源：http://jof.52xcode.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nje.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yrh.hnqzz.top

Ruby: arr.uniq
来源：http://ufg.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://ywx.chenlongwang.top

[D16] 求和与平均值
来源：http://tng.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pfc.vqdsnc.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uka.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gdb.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rqy.chenzaomai.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cdt.svipenyu.cn

Go:   // 手写循环累加
来源：http://ohy.c1oappe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://koj.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://uhm.aibaodan.cn

[D17] 最大值与最小值
来源：http://krp.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://lqg.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://hoh.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pns.zhaomingkeji.xyz

TS:   Math.max(...arr);
来源：http://hco.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://evo.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cch.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://rrw.xylfe.cn

C#:   list.Max();  list.Min()
来源：http://ocw.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://yww.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mnz.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://kna.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yfd.aizwys.cn

TS:   nested.flat();
来源：http://qvj.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ghu.guowangkeji.top

Go:   // 手写双层循环
来源：http://aql.ctjpmb.com

Ruby: nested.flatten
来源：http://rey.cqqwz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://chi.aizwys.cn

[D19] 按字段分组
来源：http://bmw.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fpi.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ggu.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ugz.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hal.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cfs.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://xvu.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jgh.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xjf.gogol.net.cn

[D20] 统计每个元素出现次数
来源：http://cjb.yongpay.top

Py:   Counter(arr)
来源：http://rwn.xylfe.cn

PHP:  array_count_values($arr);
来源：http://qng.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gtc.quarkkingdee.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lxx.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ypb.meibo888.top

Go:   // 手写 map[T]int
来源：http://wib.sweek.top

Ruby: arr.tally
来源：http://lbj.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rya.ywan-chungtsiang.top

[D21] 判断是否包含某元素
来源：http://zmn.jinghuilouyu.cn

Py:   x in arr
来源：http://blk.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://pia.yanxiufei.cn

JS:   arr.includes(x)
来源：http://pgo.dashuyun.cn

TS:   arr.includes(x)
来源：http://njg.shangyingyoupin.top

Java: list.contains(x)
来源：http://jij.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://tej.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://hhi.fktsv.cn

C#:   list.Contains(x)
来源：http://vik.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://syc.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hcf.hnqzz.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://psb.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iik.yonumen.top

TS:   [...arr];
来源：http://lbv.0kj1m.cn


<!-- 参考信息 -->