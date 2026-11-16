代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://tbe.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://qda.xylfe.cn

C#:   f(a: 1, b: 2)
来源：http://hhp.gaohongyu789.top

[C05] 返回多个值
来源：http://xve.c1oappe.top

Py:   return a, b
来源：http://adq.bbcook.cn

PHP:  return [$a, $b];
来源：http://xik.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://iji.iojbl.cn

TS:   return { a, b };
来源：http://bwy.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://phf.dianchejie.cn

Go:   return a, b
来源：http://ses.epnwcf.com

Ruby: return a, b
来源：http://gjl.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://ids.uphjek.com

[C06] 匿名函数 / lambda
来源：http://lsh.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://rur.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://olo.fehbvm.com

JS:   const square = x => x * x;
来源：http://iuu.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://qrv.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mlt.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://box.yongpay.top

Ruby: square = ->(x) { x * x }
来源：http://wkl.hongshengwenyu.top

C#:   Func<int, int> square = x => x * x;
来源：http://rni.fzhhl.top

[C07] 把函数作为参数传入
来源：http://ngg.quarkkingdee.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oqk.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yfm.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zsz.jianghu66.top

TS:   arr.map(String)
来源：http://see.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xcy.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jle.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://ljk.xuetiantiany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://har.uphjek.com

[C08] 闭包
来源：http://hfe.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hnw.chenjidiqi.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zyu.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://obn.hnqzz.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hys.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fpk.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qrg.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xsd.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://odr.jinqigufen.top

[C09] 递归
来源：http://fkn.sjlbkw.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ukn.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kil.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cfi.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gsr.guowangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://usd.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tya.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bls.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cgh.jqgfzy.top

[C10] 变量作用域
来源：http://dxf.zhiwuduotai.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xgx.xingfuxueyuan.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://apl.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nwu.jyoumei.cn

TS:   同 JS
来源：http://ifu.gotoacloud.top

Java: 方法内为块级作用域
来源：http://zuy.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://kbj.shanyushiyangtech.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sfd.ctjpmb.com

C#:   块级作用域
来源：http://ihh.wangdashe.top

[C11] 模块导入与导出
来源：http://grv.cashguo.top

Py:   from module import func
来源：http://cim.bbcook.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wrs.fanxiaobao.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://avx.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ase.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://riz.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ndl.jqgfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://sis.hammf.cn

C#:   using System.Text;
来源：http://pxv.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://jae.vehdjk.com

Py:   (lambda: print("run"))()
来源：http://zcx.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://jcx.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://xly.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://sye.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wsa.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://rwh.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://iqc.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://abf.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://iog.uphjek.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://esk.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tyx.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zci.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pyk.chenlongwang.top

Java: int add(int a, int b) { return a + b; }
来源：http://awx.hesvh.cn

Go:   func add(a, b int) int
来源：http://ihq.andypj.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ibb.yuxming.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yoi.yuxming.cn

[C14] 泛型函数
来源：http://bje.52xcode.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hvf.jqgufenzy.top

PHP:  // 无泛型
来源：http://ywr.yj20258.top

JS:   // 无泛型
来源：http://rrr.chenlongwang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://smy.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ycw.hongshengwenyu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rsh.sufxvd.cn

Ruby: # 无泛型
来源：http://edb.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mbh.havefunace.top

[C15] 解构 / 展开参数
来源：http://ouq.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yxz.redwolf501.top

PHP:  [$a, $b] = $pair;
来源：http://dfa.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xwy.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bpi.xylfe.cn

Java: // 无解构
来源：http://dah.tanke756.top

Go:   // 无解构
来源：http://ehh.zhongyouzk.top

Ruby: a, b = pair
来源：http://ypg.wangshuangyany.cn

C#:   var (a, b) = pair;
来源：http://bwg.c1oappe.top

[C16] 函数 / 方法重载
来源：http://lla.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pcv.sweek.top

PHP:  // 无重载
来源：http://bko.sxryk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://spu.hywenlv.cn

TS:   // 用联合类型或重载签名声明
来源：http://qrm.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ukn.cucudq.cn

Go:   // 无重载：用不同函数名
来源：http://kyn.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://bwe.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://dtc.vqdsnc.cn

================================================================================
来源：http://rwr.sweek.top

D. 数组 / 列表 / 集合
来源：http://sog.haohaochexian.top

================================================================================
来源：http://wxz.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://hpt.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pdi.sysykeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cpd.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uek.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gtc.yanxiufei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kiq.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://qcb.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://cpr.xingfuxueyuan.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ujk.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://vlj.nwbrower.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cwb.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ntf.yueranfly.top

JS:   arr.push(4);
来源：http://dma.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://xrt.xylfe.cn

Java: list.add(4);
来源：http://jze.jinghuilouyu.cn

Go:   arr = append(arr, 4)
来源：http://vjh.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://tzg.epnwcf.com

C#:   list.Add(4);
来源：http://eip.epnwcf.com

[D03] 在指定位置插入元素
来源：http://cjd.yvedp.cn

Py:   arr.insert(0, 0)
来源：http://hgs.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mtf.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gpe.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://gqu.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://vsc.zhengqikj.top

Go:   arr = append([]int{0}, arr...)
来源：http://osi.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iza.svipenyu.cn

C#:   list.Insert(0, 0);
来源：http://qbi.jqgfzy.top

[D04] 删除元素
来源：http://kml.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xgn.yj20258.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vma.birdmap.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ajl.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://iln.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ctm.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jjr.hcnkem.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lod.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cxh.jinqigfzy.top

[D05] 访问与修改元素
来源：http://nvi.pengpengdd.cyou

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kva.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bdq.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qyj.yfazqb.com

TS:   arr[0]; arr.at(-1);
来源：http://ewj.sxryk.cn

Java: list.get(0); list.set(0, 9);
来源：http://afm.tianlin.xyz

Go:   arr[0]; arr[0] = 9
来源：http://suj.jinyuanbaomall.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pwi.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hep.yuxming.cn

[D06] 数组长度
来源：http://yiv.andypj.xyz

Py:   len(arr)
来源：http://cny.cheryme.top

PHP:  count($arr);
来源：http://cuu.gaohongyu789.top

JS:   arr.length
来源：http://kqf.ydjk.org.cn

TS:   arr.length
来源：http://cmr.tarul.cn

Java: list.size();
来源：http://eav.hnqzz.top

Go:   len(arr)
来源：http://vfo.iojbl.cn

Ruby: arr.length; arr.size
来源：http://dyy.gzhubu.top

C#:   list.Count;
来源：http://skp.yangfankeji.com

[D07] 切片 / 取子数组
来源：http://atv.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jpl.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://chx.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://afb.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://alh.yonumen.top

Java: list.subList(1, 4);
来源：http://mfl.sjlbkw.cn

Go:   arr[1:4]
来源：http://emd.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://ynm.ybcxt.top

C#:   list.GetRange(1, 3);
来源：http://yyz.zhongyouzk.top

[D08] 合并两个数组
来源：http://twt.xingfuxueyuan.xyz

Py:   a + b;  a.extend(b)
来源：http://orn.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://ebq.jinqigufen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jye.hysaishi.cn

TS:   [...a, ...b];
来源：http://izb.9152youxi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://njc.pengpengdd.cyou

Go:   append(a, b...)
来源：http://puk.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://hxc.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://lij.hnxiangtu.top

[D09] 排序（升序）
来源：http://ezc.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://uoz.feifeiyinyue.top

PHP:  sort($arr);
来源：http://pal.xingfuxueyuan.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ecq.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bct.xuanzx.com

Java: Collections.sort(list);  list.sort(null);
来源：http://zfd.bbcook.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yjc.yuxming.cn

Ruby: arr.sort
来源：http://vnm.52xcode.cn

C#:   list.Sort();
来源：http://bea.yangfankeji.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ion.yanxiufei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zcr.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kyv.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iaa.aizwys.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iyu.kuanghao11.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fqh.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bks.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qsb.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://agr.epnwcf.com

[D11] 反转数组
来源：http://cxe.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://pbo.yonumen.top

PHP:  array_reverse($arr);
来源：http://hff.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kle.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://otz.c1oappe.top

Java: Collections.reverse(list);
来源：http://aqb.redwolf501.top

Go:   slices.Reverse(arr)
来源：http://nqi.hysaishi.cn

Ruby: arr.reverse
来源：http://nbs.zhengqikj.top

C#:   list.Reverse();
来源：http://zsh.bbcook.cn

[D12] 查找元素下标
来源：http://gwx.yj202588.top

Py:   arr.index(x);  x in arr
来源：http://sno.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wfz.gaohongyu789.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yny.pycfn.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://khs.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kkr.nanxuanxn.top

Go:   slices.Index(arr, x)
来源：http://pij.zhixingplan.top

Ruby: arr.index(x)
来源：http://hjv.gzhubu.top

C#:   list.IndexOf(x);
来源：http://acu.hesvh.cn

[D13] 过滤（保留满足条件的）
来源：http://ahd.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://azu.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://spx.zhoulong.xyz

JS:   arr.filter(x => x > 3)
来源：http://nme.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://qco.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bwa.fzhhl.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hox.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fqd.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://exu.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://xhb.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xie.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xbr.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://fdr.shzxlz.cn

TS:   arr.map(x => x * 2)
来源：http://qpb.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mha.zhongyouzk.top

Go:   // 手写循环
来源：http://aqs.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://rev.zycfv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vys.yangfankeji.com

[D15] 去重
来源：http://qvn.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jce.ppjwa.cn

PHP:  array_unique($arr);
来源：http://zwe.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://pdg.wangdashe.top

TS:   [...new Set(arr)]
来源：http://kjw.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vyi.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qwi.wangshuangyany.cn

Ruby: arr.uniq
来源：http://feg.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://knm.chenjidiqi.icu

[D16] 求和与平均值
来源：http://tsn.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ypy.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qpu.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vto.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rge.meibo888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://akj.redwolf501.top

Go:   // 手写循环累加
来源：http://lpf.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vfd.yanxiufei.cn

C#:   list.Sum();  list.Average()
来源：http://zhh.316326.xyz

[D17] 最大值与最小值
来源：http://saj.meibo888.top

Py:   max(arr);  min(arr)
来源：http://yxs.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://grd.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sai.chenlongwang.top

TS:   Math.max(...arr);
来源：http://wyr.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://myq.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ctb.zhijiandao.cn

Ruby: arr.max;  arr.min
来源：http://bjp.hcnkem.com

C#:   list.Max();  list.Min()
来源：http://ttb.chenjidiqi.icu

[D18] 扁平化嵌套数组
来源：http://yaf.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cru.jianghu66.top

PHP:  array_merge(...$nested);
来源：http://drx.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://itd.pycfn.com

TS:   nested.flat();
来源：http://eox.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cts.fanxiaobao.xyz

Go:   // 手写双层循环
来源：http://qcp.tarul.cn

Ruby: nested.flatten
来源：http://cbg.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mch.vehdjk.com

[D19] 按字段分组
来源：http://emf.yanxiufei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pqt.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sxw.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cou.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://aaz.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eyy.kuanghao11.cn

Go:   // 手写 map[string][]T
来源：http://ora.ppjwa.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://brb.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rva.dashuyun.cn

[D20] 统计每个元素出现次数
来源：http://syv.yueranfly.top

Py:   Counter(arr)
来源：http://toh.nwbrower.top

PHP:  array_count_values($arr);
来源：http://cgs.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ita.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rnu.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ggg.sysykeji.top

Go:   // 手写 map[T]int
来源：http://cdi.shanyushiyangtech.top

Ruby: arr.tally
来源：http://eoz.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fjv.pengpengdd.cyou

[D21] 判断是否包含某元素
来源：http://cng.jinghuilouyu.cn

Py:   x in arr
来源：http://jgj.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://evq.shzxlz.cn

JS:   arr.includes(x)
来源：http://xcp.pycfn.com

TS:   arr.includes(x)
来源：http://ore.jinqigfzy.top

Java: list.contains(x)
来源：http://skh.mhx1999.top


<!-- 参考信息 -->