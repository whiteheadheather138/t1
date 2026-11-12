代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nbl.hywenlv.cn

TS:   arr.map(String)
来源：http://lnr.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://trk.kuanghao11.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kei.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://pah.jqgfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qrb.ybcxt.top

[C08] 闭包
来源：http://gwh.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://asy.fktsv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ikk.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ihz.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://abr.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rky.jinyuanbaomall.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ppx.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rfa.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ftn.gogol.net.cn

[C09] 递归
来源：http://vae.pengpengdd.cyou

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://crh.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fld.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ieo.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ugz.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://waf.xziqi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jkx.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hvo.yj20258888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zau.vqdsnc.cn

[C10] 变量作用域
来源：http://das.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qam.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://afb.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xkv.jqgfzy.top

TS:   同 JS
来源：http://gwb.hnqzz.top

Java: 方法内为块级作用域
来源：http://cjt.hcnkem.com

Go:   花括号块级作用域
来源：http://hcb.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iyc.yuxming.cn

C#:   块级作用域
来源：http://gph.tanke756.top

[C11] 模块导入与导出
来源：http://gkg.snrcjt.cn

Py:   from module import func
来源：http://dut.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://alh.fktsv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nxs.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iej.aizwys.cn

Java: import java.util.List;
来源：http://wcx.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nej.jinqigfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://stc.gotoacloud.top

C#:   using System.Text;
来源：http://kjp.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://eez.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://kuo.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://hsn.gaohongyu789.top

JS:   (() => { console.log("run"); })();
来源：http://mds.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://pnf.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uhg.sysykeji.top

Go:   func() { fmt.Println("run") }()
来源：http://xgq.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://hff.birdmap.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fmu.zhaomingkeji.xyz

[C13] 类型声明 / 类型注解
来源：http://krb.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://stw.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lrq.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sbe.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tim.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rej.guannengcc.top

Go:   func add(a, b int) int
来源：http://qqy.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://koz.wangshuangyany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bpt.zdqjudy.top

[C14] 泛型函数
来源：http://tah.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://agg.ydzc1.top

PHP:  // 无泛型
来源：http://ome.ybcxt.top

JS:   // 无泛型
来源：http://ueg.birdmap.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sfq.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oak.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bqb.cqqwz.cn

Ruby: # 无泛型
来源：http://xst.aizwys.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eqo.cheryme.top

[C15] 解构 / 展开参数
来源：http://xgi.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://met.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://mtd.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jev.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://van.aizwys.cn

Java: // 无解构
来源：http://ltf.xinyue.icu

Go:   // 无解构
来源：http://ecg.ywan-chungtsiang.top

Ruby: a, b = pair
来源：http://yye.yueranfly.top

C#:   var (a, b) = pair;
来源：http://ubz.sxryk.cn

[C16] 函数 / 方法重载
来源：http://gzk.fzhhl.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iiv.yongpay.top

PHP:  // 无重载
来源：http://rro.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zhm.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://tck.zhaomingkeji.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://fpb.xingfuxueyuan.xyz

Go:   // 无重载：用不同函数名
来源：http://pkx.hywenlv.cn

Ruby: # 无重载：靠动态参数
来源：http://jre.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lls.yj202588.top

================================================================================
来源：http://zoh.zhoulong.xyz

D. 数组 / 列表 / 集合
来源：http://byl.nanxinkj.top

================================================================================
来源：http://zhc.shzxlz.cn

[D01] 创建数组 / 列表
来源：http://hau.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://aof.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uny.smart0.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nod.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oug.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ufg.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://dzj.hesvh.cn

Ruby: arr = [1, 2, 3]
来源：http://nrp.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ghl.jinqigufen.top

[D02] 追加元素到末尾
来源：http://jvr.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tab.xziqi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rpu.cqqwz.cn

JS:   arr.push(4);
来源：http://vel.feifeiyinyue.top

TS:   arr.push(4);
来源：http://bqe.cdnleiting.top

Java: list.add(4);
来源：http://kkj.cashguo.top

Go:   arr = append(arr, 4)
来源：http://vfv.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://mxu.fengsongda.top

C#:   list.Add(4);
来源：http://jta.vqdsnc.cn

[D03] 在指定位置插入元素
来源：http://jhf.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://xzs.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vjb.ppjwa.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bcv.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://yiy.zdbjq.cn

Java: list.add(0, 0);
来源：http://azd.fanxiaobao.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://vsi.hcnkem.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wxm.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://zoa.yanxiufei.cn

[D04] 删除元素
来源：http://vcu.ydzc1.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://toz.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qkn.zhixingplan.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bcp.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://cbo.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pfh.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vtm.nwbrower.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qjr.birdmap.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mvl.zhengqikj.top

[D05] 访问与修改元素
来源：http://erz.daria6918.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nth.andypj.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qei.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://edw.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://hwa.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://pfr.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://ykk.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://azf.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wkh.hfpthk.cn

[D06] 数组长度
来源：http://bxy.jinyuanbaomall.cn

Py:   len(arr)
来源：http://xqn.cucudq.cn

PHP:  count($arr);
来源：http://oqx.hywenlv.cn

JS:   arr.length
来源：http://aok.zdbjq.cn

TS:   arr.length
来源：http://mhb.sxryk.cn

Java: list.size();
来源：http://ynq.yonumen.top

Go:   len(arr)
来源：http://xap.yonumen.top

Ruby: arr.length; arr.size
来源：http://itd.pengpengdd.cyou

C#:   list.Count;
来源：http://evv.xinyue.icu

[D07] 切片 / 取子数组
来源：http://eyu.hysaishi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dts.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://dxq.ywan-chungtsiang.top

JS:   arr.slice(1, 4);
来源：http://lkn.hammf.cn

TS:   arr.slice(1, 4);
来源：http://gig.fehbvm.com

Java: list.subList(1, 4);
来源：http://yvm.pengpengdd.cyou

Go:   arr[1:4]
来源：http://ywp.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://njm.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://koi.jianghu66.top

[D08] 合并两个数组
来源：http://qml.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://qwk.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://vav.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ykv.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://ejh.nanxinkj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://afa.yongpay.top

Go:   append(a, b...)
来源：http://qpc.xziqi.cn

Ruby: a + b;  a.concat(b)
来源：http://vtv.hnqzz.top

C#:   a.Concat(b).ToList()
来源：http://dpc.chenlongwang.top

[D09] 排序（升序）
来源：http://bal.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://fnb.xinyue.icu

PHP:  sort($arr);
来源：http://gwd.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zvf.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hjh.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://aac.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ryd.hcnkem.com

Ruby: arr.sort
来源：http://ean.zhijiandao.cn

C#:   list.Sort();
来源：http://smq.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bqu.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xnc.cashguo.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mdj.chenzaomai.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wfd.c1oappe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hfd.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qhf.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jth.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ecp.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cmf.dianchejie.cn

[D11] 反转数组
来源：http://hyd.fzhhl.top

Py:   arr[::-1];  arr.reverse()
来源：http://zzz.yfazqb.com

PHP:  array_reverse($arr);
来源：http://liw.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rkm.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://thl.52xcode.cn

Java: Collections.reverse(list);
来源：http://sdz.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://iic.yueranfly.top

Ruby: arr.reverse
来源：http://bdd.zhaomingkeji.xyz

C#:   list.Reverse();
来源：http://rwz.redwolf501.top

[D12] 查找元素下标
来源：http://mre.gogol.net.cn

Py:   arr.index(x);  x in arr
来源：http://hlx.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ggj.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wun.9152youxi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nmh.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uwh.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://oax.fengsongda.top

Ruby: arr.index(x)
来源：http://ntd.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://etx.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://ezb.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nsj.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lar.hongshengwenyu.top

JS:   arr.filter(x => x > 3)
来源：http://siw.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://gfl.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tmb.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fpj.xuetiantiany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fth.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nbx.guannengcc.top

[D14] 映射转换（每个元素变形）
来源：http://pnt.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lbt.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iag.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://vir.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://yrr.zhoulong.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://mmb.sufxvd.cn

Go:   // 手写循环
来源：http://ial.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fej.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://mhi.yj202588.top

[D15] 去重
来源：http://dfb.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fhz.yongpay.top

PHP:  array_unique($arr);
来源：http://etq.nwbrower.top

JS:   [...new Set(arr)]
来源：http://bky.smart0.xyz

TS:   [...new Set(arr)]
来源：http://zym.shanyushiyangtech.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jvv.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://iax.fengsongda.top

Ruby: arr.uniq
来源：http://xje.shuidangran.top

C#:   list.Distinct().ToList()
来源：http://ovr.redwolf501.top

[D16] 求和与平均值
来源：http://npp.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://okh.bjfxy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nud.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nlu.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sdr.cucudq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://svg.shzxlz.cn

Go:   // 手写循环累加
来源：http://sqp.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wvk.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://edt.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://mki.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://wll.xylfe.cn

PHP:  max($arr);  min($arr);
来源：http://ezk.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dmd.fktsv.cn

TS:   Math.max(...arr);
来源：http://eyk.jinqigufen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xqd.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jlp.ydzc1.top

Ruby: arr.max;  arr.min
来源：http://hvg.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://dwg.chenlongwang.top

[D18] 扁平化嵌套数组
来源：http://vxr.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hzr.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://dor.yuanzhike.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xea.shzxlz.cn

TS:   nested.flat();
来源：http://ptq.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ouq.shzxlz.cn

Go:   // 手写双层循环
来源：http://bwo.hongshengwenyu.top

Ruby: nested.flatten
来源：http://abw.jqgfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nky.yueranfly.top

[D19] 按字段分组
来源：http://kmu.fktsv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cnt.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yjn.ivvv.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vjk.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xwg.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bug.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://nie.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fdr.tian-w.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cyp.tanke756.top

[D20] 统计每个元素出现次数
来源：http://ftw.zhoulong.xyz

Py:   Counter(arr)
来源：http://jdb.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://eyi.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fcj.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vfw.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tsu.yonumen.top

Go:   // 手写 map[T]int
来源：http://urb.birdmap.top

Ruby: arr.tally
来源：http://jmq.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cyq.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://loy.yuxming.cn

Py:   x in arr
来源：http://fan.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://fjs.quarkkingdee.top

JS:   arr.includes(x)
来源：http://tkq.havefunace.top

TS:   arr.includes(x)
来源：http://rlo.aizwys.cn

Java: list.contains(x)
来源：http://dav.jinyuanbaomall.cn

Go:   slices.Contains(arr, x)
来源：http://udl.jianghu66.top

Ruby: arr.include?(x)
来源：http://lnw.xylfe.cn

C#:   list.Contains(x)
来源：http://lzz.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://nzs.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xuw.epnwcf.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://svq.yangfankeji.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qks.hammf.cn

TS:   [...arr];
来源：http://gke.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://our.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zar.vqdsnc.cn

Ruby: arr.dup;  arr.clone
来源：http://ehn.hesvh.cn

C#:   new List<int>(list);
来源：http://qou.shanyushiyangkeji.top

[D23] reduce 累积计算
来源：http://nah.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mzn.ehwqpu.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ypo.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://upy.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bpx.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://isq.ehwqpu.com

Go:   // 手写循环
来源：http://dqn.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oib.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nke.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://pgb.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bdt.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://epn.yfazqb.com


<!-- 参考信息 -->