代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://tzd.yanxiufei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xso.hywenlv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gxq.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://pme.ybcxt.top

C#:   Func<int, int> square = x => x * x;
来源：http://pio.andypj.xyz

[C07] 把函数作为参数传入
来源：http://qwt.smart0.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lzx.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://hxx.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ohm.tian-w.cn

TS:   arr.map(String)
来源：http://chd.xingfuxueyuan.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ojk.bjfxy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jky.daria6918.cn

Ruby: arr.map(&:upcase)
来源：http://kqc.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uug.fehbvm.com

[C08] 闭包
来源：http://nds.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rku.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pxd.meibo888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ssa.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ark.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gse.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ljl.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xfe.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mzs.chenlongwang.top

[C09] 递归
来源：http://oog.epnwcf.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fps.sweek.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cdg.dashuyun.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://waj.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rbr.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fht.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rfq.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://esl.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://twh.tianlin.xyz

[C10] 变量作用域
来源：http://ach.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xlu.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tkb.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rxy.wangshuangyany.cn

TS:   同 JS
来源：http://nxs.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://vdf.sysykeji.top

Go:   花括号块级作用域
来源：http://uhx.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oas.jqgfzy.top

C#:   块级作用域
来源：http://myo.sysykeji.top

[C11] 模块导入与导出
来源：http://nvi.ybcxt.top

Py:   from module import func
来源：http://dpf.jinqigfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cdy.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bct.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://khj.jinghuilouyu.cn

Java: import java.util.List;
来源：http://zpq.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rgn.shuidangran.top

Ruby: require "json"; require_relative "./util"
来源：http://eoi.ehwqpu.com

C#:   using System.Text;
来源：http://fxi.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://uqd.zhijiandao.cn

Py:   (lambda: print("run"))()
来源：http://ogy.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://zmw.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://ijg.yanxiufei.cn

TS:   (() => { console.log("run"); })();
来源：http://zcf.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://joe.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://vtc.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://hpa.dianchejie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gev.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://dvd.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://akd.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ffc.zhongyouzk.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gze.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vso.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://ksv.hnqzz.top

Go:   func add(a, b int) int
来源：http://cyf.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gcr.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://grt.jinqigufen.top

[C14] 泛型函数
来源：http://nti.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vvn.mhx1999.top

PHP:  // 无泛型
来源：http://gtw.hywenlv.cn

JS:   // 无泛型
来源：http://aaa.birdmap.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sfl.smart0.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gun.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://otx.kuanghao11.cn

Ruby: # 无泛型
来源：http://izj.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iqt.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://oop.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hnk.cheryme.top

PHP:  [$a, $b] = $pair;
来源：http://hlq.9152youxi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wae.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qzl.hongshengwenyu.top

Java: // 无解构
来源：http://ues.havefunace.top

Go:   // 无解构
来源：http://blt.sweek.top

Ruby: a, b = pair
来源：http://lxa.yvedp.cn

C#:   var (a, b) = pair;
来源：http://yqw.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://ayl.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yhd.c1oappe.top

PHP:  // 无重载
来源：http://viw.jinghuilouyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sqi.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://dei.hnqzz.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vds.jinyuanbaomall.cn

Go:   // 无重载：用不同函数名
来源：http://wbh.9152youxi.cn

Ruby: # 无重载：靠动态参数
来源：http://hos.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vnv.redwolf501.top

================================================================================
来源：http://vmq.hammf.cn

D. 数组 / 列表 / 集合
来源：http://hzr.jyoumei.cn

================================================================================
来源：http://xvu.guannengcc.top

[D01] 创建数组 / 列表
来源：http://qta.shanyushiyangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xhz.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hbj.yonumen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hhn.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lqb.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zye.zhengqikj.top

Go:   arr := []int{1, 2, 3}
来源：http://nbd.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://gkn.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nwn.xylfe.cn

[D02] 追加元素到末尾
来源：http://wyl.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jcu.fzhhl.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vyr.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://ikz.hesvh.cn

TS:   arr.push(4);
来源：http://bbd.quarkkingdee.top

Java: list.add(4);
来源：http://atx.quarkkingdee.top

Go:   arr = append(arr, 4)
来源：http://zzi.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://kkg.yj20258.top

C#:   list.Add(4);
来源：http://xav.chenlongwang.top

[D03] 在指定位置插入元素
来源：http://nvs.ppjwa.cn

Py:   arr.insert(0, 0)
来源：http://snp.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zqc.birdmap.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vix.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://xfq.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://pkw.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lod.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gls.sysykeji.top

C#:   list.Insert(0, 0);
来源：http://agh.jianghu66.top

[D04] 删除元素
来源：http://vfo.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mul.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gnp.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qtt.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://pow.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qvf.ydjk.org.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pfj.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fsa.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mmk.zhijiandao.cn

[D05] 访问与修改元素
来源：http://nhr.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vzm.shanyushiyangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bhu.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rds.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://cvb.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://wbp.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://bio.snrcjt.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lkw.hnxiangtu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pkn.fktsv.cn

[D06] 数组长度
来源：http://mic.shanyushiyangkeji.top

Py:   len(arr)
来源：http://fvw.hcnkem.com

PHP:  count($arr);
来源：http://zau.epnwcf.com

JS:   arr.length
来源：http://yob.wangshuangyany.cn

TS:   arr.length
来源：http://nle.xuanzx.com

Java: list.size();
来源：http://bzq.haohaochexian.top

Go:   len(arr)
来源：http://vdv.snrcjt.cn

Ruby: arr.length; arr.size
来源：http://sqa.chenjidiqi.icu

C#:   list.Count;
来源：http://lat.yueranfly.top

[D07] 切片 / 取子数组
来源：http://qhx.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gif.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://nzx.nanxuanxn.top

JS:   arr.slice(1, 4);
来源：http://adj.aizwys.cn

TS:   arr.slice(1, 4);
来源：http://jot.hcnkem.com

Java: list.subList(1, 4);
来源：http://nzb.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://rna.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://qpe.ydjk.org.cn

C#:   list.GetRange(1, 3);
来源：http://inp.9152youxi.cn

[D08] 合并两个数组
来源：http://ftp.kuanghao11.cn

Py:   a + b;  a.extend(b)
来源：http://rvj.dianchejie.cn

PHP:  array_merge($a, $b);
来源：http://esm.andypj.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://jkk.zhixingplan.top

TS:   [...a, ...b];
来源：http://npa.wangshuangyany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rhk.ybcxt.top

Go:   append(a, b...)
来源：http://dxk.hcnkem.com

Ruby: a + b;  a.concat(b)
来源：http://ntc.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://pjo.wangdashe.top

[D09] 排序（升序）
来源：http://tcf.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://lrp.sufxvd.cn

PHP:  sort($arr);
来源：http://pda.nanxuanxn.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gme.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kfa.zdqjudy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zza.fzhhl.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yau.hnxiangtu.top

Ruby: arr.sort
来源：http://rcr.ivvv.top

C#:   list.Sort();
来源：http://qfn.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ksy.iojbl.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aoc.cucudq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dgm.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qqa.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cyu.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cvg.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fto.svipenyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dqb.zdqjudy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yif.cashguo.top

[D11] 反转数组
来源：http://cwu.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://kpm.hesvh.cn

PHP:  array_reverse($arr);
来源：http://ngh.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cbb.zdqjudy.top

TS:   [...arr].reverse();
来源：http://izj.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://cdq.vqdsnc.cn

Go:   slices.Reverse(arr)
来源：http://xxt.dianchejie.cn

Ruby: arr.reverse
来源：http://flm.yanxiufei.cn

C#:   list.Reverse();
来源：http://bmt.feifeiyinyue.top

[D12] 查找元素下标
来源：http://fbk.sufxvd.cn

Py:   arr.index(x);  x in arr
来源：http://tah.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tmb.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ymh.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ngb.uphjek.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://usy.nanxinkj.top

Go:   slices.Index(arr, x)
来源：http://qse.svipenyu.cn

Ruby: arr.index(x)
来源：http://urd.hammf.cn

C#:   list.IndexOf(x);
来源：http://tqa.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://ody.epnwcf.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ooc.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dqa.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://wfy.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://uuf.9152youxi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://skq.zdbjq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zwg.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://iob.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ysx.feifeiyinyue.top

[D14] 映射转换（每个元素变形）
来源：http://ofb.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nfo.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fbj.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://uyo.jinyuanbaomall.cn

TS:   arr.map(x => x * 2)
来源：http://tso.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://smm.c1oappe.top

Go:   // 手写循环
来源：http://ouc.ctjpmb.com

Ruby: arr.map { |x| x * 2 }
来源：http://vwz.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://djh.nanxuanxn.top

[D15] 去重
来源：http://add.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oze.fanxiaobao.xyz

PHP:  array_unique($arr);
来源：http://efv.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://ano.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://ypc.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dba.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://tlb.yj20258.top

Ruby: arr.uniq
来源：http://qid.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://jby.ydjk.org.cn

[D16] 求和与平均值
来源：http://bxi.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://isp.gaohongyu789.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vlx.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gxo.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ybr.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vyw.snrcjt.cn

Go:   // 手写循环累加
来源：http://klt.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vbb.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://gnn.zhixingplan.top

[D17] 最大值与最小值
来源：http://kam.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://pxv.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://uxc.zdbjq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vzb.pengpengdd.cyou

TS:   Math.max(...arr);
来源：http://ykw.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qom.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://osh.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://syc.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://jqz.nanxinkj.top

[D18] 扁平化嵌套数组
来源：http://xuv.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rpd.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://oey.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hvn.zhengqikj.top

TS:   nested.flat();
来源：http://phs.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://imm.xuanzx.com

Go:   // 手写双层循环
来源：http://mol.zdbjq.cn

Ruby: nested.flatten
来源：http://frw.fktsv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hom.zhijiandao.cn

[D19] 按字段分组
来源：http://zsl.ctjpmb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://edk.sysykeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tnq.zhijiandao.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wvc.nanxinkj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nmu.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sri.meibo888.top

Go:   // 手写 map[string][]T
来源：http://fkd.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wix.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hiy.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://lqd.yonumen.top

Py:   Counter(arr)
来源：http://gyn.pycfn.com

PHP:  array_count_values($arr);
来源：http://wpw.daria6918.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kka.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fvt.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iuw.yuxming.cn

Go:   // 手写 map[T]int
来源：http://ogk.hywenlv.cn

Ruby: arr.tally
来源：http://wsj.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kbd.nanxuanxn.top

[D21] 判断是否包含某元素
来源：http://txi.jinqigufen.top

Py:   x in arr
来源：http://sfx.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://nvx.xuanzx.com

JS:   arr.includes(x)
来源：http://urb.nanxinkj.top

TS:   arr.includes(x)
来源：http://hvr.hywenlv.cn

Java: list.contains(x)
来源：http://tti.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://qpp.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://pxv.9152youxi.cn

C#:   list.Contains(x)
来源：http://eos.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://wmq.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sds.daria6918.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vos.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aye.jinyuanbaomall.cn

TS:   [...arr];
来源：http://ecv.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://yts.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://lic.sxryk.cn

Ruby: arr.dup;  arr.clone
来源：http://qzf.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://tbp.fehbvm.com

[D23] reduce 累积计算
来源：http://edj.hysaishi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bev.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://owa.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dzj.guannengcc.top


<!-- 参考信息 -->