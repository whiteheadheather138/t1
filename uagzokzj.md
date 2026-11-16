代发 wailian999

Py:   return a, b
来源：http://dbw.yuanzhike.top

PHP:  return [$a, $b];
来源：http://dkj.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dyk.zhijiandao.cn

TS:   return { a, b };
来源：http://hhi.9152youxi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ybn.redwolf501.top

Go:   return a, b
来源：http://gtx.wangdashe.top

Ruby: return a, b
来源：http://qbu.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://mth.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://rbk.sxryk.cn

Py:   square = lambda x: x * x
来源：http://aja.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ves.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://exx.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://hry.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://drh.yangfankeji.com

Go:   sq := func(x int) int { return x * x }
来源：http://llh.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://lhx.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://vta.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://ncv.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vmt.havefunace.top

PHP:  array_map("strtoupper", $arr);
来源：http://zsu.pycfn.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mga.zdqjudy.top

TS:   arr.map(String)
来源：http://fbs.sufxvd.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wjm.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dyt.yuxming.cn

Ruby: arr.map(&:upcase)
来源：http://zic.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://azt.zycfv.cn

[C08] 闭包
来源：http://bck.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tiv.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xuf.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gqq.shanyushiyangtech.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mfr.316326.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nje.sufxvd.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ctt.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gth.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gss.xylfe.cn

[C09] 递归
来源：http://fii.bjfxy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mcz.epnwcf.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qsz.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sfx.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vzn.ehwqpu.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fpm.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jng.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iws.ydjk.org.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mqo.sweek.top

[C10] 变量作用域
来源：http://mpl.vehdjk.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rdv.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kqj.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xzu.cashguo.top

TS:   同 JS
来源：http://kvm.nanxinkj.top

Java: 方法内为块级作用域
来源：http://xag.fanxiaobao.xyz

Go:   花括号块级作用域
来源：http://hux.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uww.xuanzx.com

C#:   块级作用域
来源：http://kkm.52xcode.cn

[C11] 模块导入与导出
来源：http://nrn.jianghu66.top

Py:   from module import func
来源：http://rkz.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xjz.52xcode.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jzr.yvedp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://efo.sysykeji.top

Java: import java.util.List;
来源：http://mue.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jad.gzhubu.top

Ruby: require "json"; require_relative "./util"
来源：http://vck.jqgufenzy.top

C#:   using System.Text;
来源：http://ffd.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://dyu.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://gug.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://dhl.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://knr.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://wog.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xam.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://nsg.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://juj.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://hnz.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://iao.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jts.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gnx.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ref.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ryb.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://zmc.bbcook.cn

Go:   func add(a, b int) int
来源：http://zox.vqdsnc.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pwz.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://nfz.chenjidiqi.icu

[C14] 泛型函数
来源：http://gdw.zdbjq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fbg.zhongyouzk.top

PHP:  // 无泛型
来源：http://dpq.bbcook.cn

JS:   // 无泛型
来源：http://hav.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jzx.jianghu66.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ddk.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vke.tian-w.cn

Ruby: # 无泛型
来源：http://qtd.jqgufenzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jpl.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://iiv.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://soc.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://smh.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pqw.yanxiufei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pfe.daria6918.cn

Java: // 无解构
来源：http://ldx.jinyuanbaomall.cn

Go:   // 无解构
来源：http://pxn.tian-w.cn

Ruby: a, b = pair
来源：http://gjp.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://enx.tarul.cn

[C16] 函数 / 方法重载
来源：http://hpl.svipenyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://toa.chenzaomai.com

PHP:  // 无重载
来源：http://kyr.sysykeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ilb.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://zoj.guannengcc.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kcd.cqqwz.cn

Go:   // 无重载：用不同函数名
来源：http://vsi.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://huj.hfpthk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lfn.jiagoushi.top

================================================================================
来源：http://ott.feifeiyinyue.top

D. 数组 / 列表 / 集合
来源：http://emi.vqdsnc.cn

================================================================================
来源：http://esy.yangfankeji.com

[D01] 创建数组 / 列表
来源：http://vju.aizwys.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qqj.birdmap.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pnq.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dbt.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://and.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bbl.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://xyq.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://bqo.wangshuangyany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lea.bbcook.cn

[D02] 追加元素到末尾
来源：http://oiu.zycfv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tuz.snrcjt.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iuz.ydjk.org.cn

JS:   arr.push(4);
来源：http://nsy.zhengqikj.top

TS:   arr.push(4);
来源：http://uxt.xylfe.cn

Java: list.add(4);
来源：http://llr.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://mxg.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://twv.yj202588.top

C#:   list.Add(4);
来源：http://vkr.hammf.cn

[D03] 在指定位置插入元素
来源：http://brl.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://enu.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://szc.kuanghao11.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://okp.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://dlv.jyoumei.cn

Java: list.add(0, 0);
来源：http://bcc.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bol.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oku.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://cjz.jinqigfzy.top

[D04] 删除元素
来源：http://zbp.shangyingyoupin.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://erm.hnqzz.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mjj.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yvv.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://cgy.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hmv.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eue.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ybs.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qie.gaohongyu789.top

[D05] 访问与修改元素
来源：http://mnm.ppjwa.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://asq.hesvh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zmx.hnqzz.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vyt.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://lpk.jiagoushi.top

Java: list.get(0); list.set(0, 9);
来源：http://qil.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://ohf.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gxx.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qqw.fehbvm.com

[D06] 数组长度
来源：http://fsb.snrcjt.cn

Py:   len(arr)
来源：http://vsj.zhoulong.xyz

PHP:  count($arr);
来源：http://ecn.yanxiufei.cn

JS:   arr.length
来源：http://aez.aizwys.cn

TS:   arr.length
来源：http://zfr.dashuyun.cn

Java: list.size();
来源：http://yhj.feifeiyinyue.top

Go:   len(arr)
来源：http://nbe.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://lpa.gotoacloud.top

C#:   list.Count;
来源：http://ysk.vehdjk.com

[D07] 切片 / 取子数组
来源：http://mfw.xuanzx.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ccz.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://ndi.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://waj.vehdjk.com

TS:   arr.slice(1, 4);
来源：http://dhh.yj20258.top

Java: list.subList(1, 4);
来源：http://zfk.gogol.net.cn

Go:   arr[1:4]
来源：http://dan.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://ylj.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://gaq.daria6918.cn

[D08] 合并两个数组
来源：http://zij.hnxiangtu.top

Py:   a + b;  a.extend(b)
来源：http://tjn.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://nyx.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pky.cucudq.cn

TS:   [...a, ...b];
来源：http://jkz.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://muz.vqdsnc.cn

Go:   append(a, b...)
来源：http://dan.gaohongyu789.top

Ruby: a + b;  a.concat(b)
来源：http://ddt.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://sww.52xcode.cn

[D09] 排序（升序）
来源：http://gxx.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://dcw.chenjidiqi.icu

PHP:  sort($arr);
来源：http://qqn.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kbe.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ovj.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jix.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pxr.gotoacloud.top

Ruby: arr.sort
来源：http://olv.yangfankeji.com

C#:   list.Sort();
来源：http://sxl.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rkv.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kjq.pengpengdd.cyou

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ggr.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dxt.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sep.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tnf.hesvh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dya.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ntc.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pdz.yj202588.top

[D11] 反转数组
来源：http://ksl.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://ctv.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://lmf.sxryk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ibi.andypj.xyz

TS:   [...arr].reverse();
来源：http://kjt.fzhhl.top

Java: Collections.reverse(list);
来源：http://arm.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://xee.jinqigufen.top

Ruby: arr.reverse
来源：http://hmq.hfpthk.cn

C#:   list.Reverse();
来源：http://jgk.yuxming.cn

[D12] 查找元素下标
来源：http://dfj.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://tee.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lbe.jianghu66.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dqa.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qkq.hywenlv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tgd.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://lmp.daria6918.cn

Ruby: arr.index(x)
来源：http://gfh.ctjpmb.com

C#:   list.IndexOf(x);
来源：http://yoc.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://jnn.yongpay.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://asd.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ump.hongshengwenyu.top

JS:   arr.filter(x => x > 3)
来源：http://gte.tian-w.cn

TS:   arr.filter(x => x > 3)
来源：http://gsj.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ztb.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blg.zdbjq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bvt.jqgufenzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fkw.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://cxq.yvedp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vup.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tlb.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://ysf.hongshengwenyu.top

TS:   arr.map(x => x * 2)
来源：http://hjk.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://sgx.sufxvd.cn

Go:   // 手写循环
来源：http://iaw.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://zmf.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vfj.cheryme.top

[D15] 去重
来源：http://czp.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ktx.shanyushiyangkeji.top

PHP:  array_unique($arr);
来源：http://olg.xziqi.cn

JS:   [...new Set(arr)]
来源：http://jjn.fengsongda.top

TS:   [...new Set(arr)]
来源：http://syd.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xie.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://qpt.fehbvm.com

Ruby: arr.uniq
来源：http://xsz.uphjek.com

C#:   list.Distinct().ToList()
来源：http://mva.0kj1m.cn

[D16] 求和与平均值
来源：http://ime.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rba.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ddi.nanxinkj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ucn.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zdp.ctjpmb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qzb.fengsongda.top

Go:   // 手写循环累加
来源：http://zlz.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://owk.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://kao.yueranfly.top

[D17] 最大值与最小值
来源：http://qae.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://yut.jlsjyb.cn

PHP:  max($arr);  min($arr);
来源：http://rbd.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://anj.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://rsl.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rhn.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ebk.yonumen.top

Ruby: arr.max;  arr.min
来源：http://bei.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://lhl.yj202588.top

[D18] 扁平化嵌套数组
来源：http://shh.tanke756.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ajo.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://rai.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ikm.pycfn.com

TS:   nested.flat();
来源：http://uso.yangfankeji.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dxa.tarul.cn

Go:   // 手写双层循环
来源：http://pmt.zhiwuduotai.top

Ruby: nested.flatten
来源：http://lfx.shzxlz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://skv.dianchejie.cn

[D19] 按字段分组
来源：http://nhx.cucudq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ikd.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://haa.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iei.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xhq.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fpn.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://xnp.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vsc.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ioh.shanyushiyangtech.top

[D20] 统计每个元素出现次数
来源：http://qil.bjfxy.top

Py:   Counter(arr)
来源：http://kcb.0kj1m.cn

PHP:  array_count_values($arr);
来源：http://oco.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wru.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bpe.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jmx.vehdjk.com

Go:   // 手写 map[T]int
来源：http://fnb.zhiwuduotai.top

Ruby: arr.tally
来源：http://yeq.xuetiantiany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ddk.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://amu.daxiang520.top

Py:   x in arr
来源：http://vxl.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://unq.yangfankeji.com

JS:   arr.includes(x)
来源：http://iku.ctjpmb.com

TS:   arr.includes(x)
来源：http://uvb.yuxming.cn

Java: list.contains(x)
来源：http://kml.cashguo.top

Go:   slices.Contains(arr, x)
来源：http://bsz.jyoumei.cn

Ruby: arr.include?(x)
来源：http://xyk.yfazqb.com

C#:   list.Contains(x)
来源：http://uho.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://lxu.ydzc1.top


<!-- 参考信息 -->