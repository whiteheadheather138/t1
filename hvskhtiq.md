代发 wailian999

[C06] 匿名函数 / lambda
来源：http://ywc.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://bze.xuanzx.com

PHP:  $square = fn($x) => $x * $x;
来源：http://gbd.iojbl.cn

JS:   const square = x => x * x;
来源：http://cfn.gogol.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://yjt.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xiu.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://lqe.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://vxu.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xlu.ybcxt.top

[C07] 把函数作为参数传入
来源：http://epn.guowangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gwf.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://chi.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sfd.hongshengwenyu.top

TS:   arr.map(String)
来源：http://ows.jyoumei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ygo.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jjt.jinqigfzy.top

Ruby: arr.map(&:upcase)
来源：http://qiz.redwolf501.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qrg.yuxming.cn

[C08] 闭包
来源：http://uva.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://era.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rhz.zhiwuduotai.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zrn.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fuh.andypj.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xpo.redwolf501.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qfv.jinqigfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mfi.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zag.smart0.xyz

[C09] 递归
来源：http://zzh.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iqm.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://scv.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aso.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iej.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://end.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ydr.yuxming.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lnw.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xvm.gogol.net.cn

[C10] 变量作用域
来源：http://vfe.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zxs.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dyz.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dhh.ctjpmb.com

TS:   同 JS
来源：http://lba.gzhubu.top

Java: 方法内为块级作用域
来源：http://plc.sysykeji.top

Go:   花括号块级作用域
来源：http://trq.pengpengdd.cyou

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wry.zhijiandao.cn

C#:   块级作用域
来源：http://sli.hfpthk.cn

[C11] 模块导入与导出
来源：http://klc.shuidangran.top

Py:   from module import func
来源：http://qzp.xylfe.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vgq.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zmd.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://unt.fanxiaobao.xyz

Java: import java.util.List;
来源：http://seg.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ulj.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://dwh.yvedp.cn

C#:   using System.Text;
来源：http://bwj.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://ogx.sweek.top

Py:   (lambda: print("run"))()
来源：http://bkp.xuanzx.com

PHP:  (function () { echo "run"; })();
来源：http://wzm.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://cqf.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://fmp.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lst.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://vps.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://sly.fktsv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pqu.jqgufenzy.top

[C13] 类型声明 / 类型注解
来源：http://bsd.ppjwa.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sfb.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pgd.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://thc.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oqh.xylfe.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ypt.ydjk.org.cn

Go:   func add(a, b int) int
来源：http://vhr.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cha.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://mrv.tarul.cn

[C14] 泛型函数
来源：http://ozj.xingfuxueyuan.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://boy.daxiang520.top

PHP:  // 无泛型
来源：http://pah.nanxinkj.top

JS:   // 无泛型
来源：http://arw.dianchejie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bak.tian-w.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yxg.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jlx.ydzc1.top

Ruby: # 无泛型
来源：http://ncy.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fzc.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://col.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wix.yvedp.cn

PHP:  [$a, $b] = $pair;
来源：http://fux.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fmd.xuanzx.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bzt.havefunace.top

Java: // 无解构
来源：http://ybp.nanxuanxn.top

Go:   // 无解构
来源：http://ppl.yongpay.top

Ruby: a, b = pair
来源：http://ete.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://xnw.yj20258.top

[C16] 函数 / 方法重载
来源：http://ffu.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ciu.dashuyun.cn

PHP:  // 无重载
来源：http://gwt.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://mkc.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://ddb.zhongyouzk.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mou.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://dyg.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://xlz.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bmy.wangshuangyany.cn

================================================================================
来源：http://bep.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://mmi.fktsv.cn

================================================================================
来源：http://loj.mhx1999.top

[D01] 创建数组 / 列表
来源：http://par.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sof.yangfankeji.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lmd.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bis.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ofv.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wkx.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://arf.yuanzhike.top

Ruby: arr = [1, 2, 3]
来源：http://ohc.zycfv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ool.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://cgy.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kev.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oiv.xylfe.cn

JS:   arr.push(4);
来源：http://dao.mhx1999.top

TS:   arr.push(4);
来源：http://quh.pycfn.com

Java: list.add(4);
来源：http://xuj.jinghuilouyu.cn

Go:   arr = append(arr, 4)
来源：http://iua.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://bxl.nwbrower.top

C#:   list.Add(4);
来源：http://jyb.meibo888.top

[D03] 在指定位置插入元素
来源：http://oiu.uphjek.com

Py:   arr.insert(0, 0)
来源：http://zcu.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kuh.snrcjt.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xry.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://nbp.0kj1m.cn

Java: list.add(0, 0);
来源：http://yja.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://fhs.shanyushiyangtech.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yyd.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://cds.nwbrower.top

[D04] 删除元素
来源：http://dwi.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qew.feifeiyinyue.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pgb.jianghu66.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nis.gogol.net.cn

TS:   arr.splice(0, 1);
来源：http://qsb.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wuu.xuanzx.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hkl.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://twt.316326.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://osv.hcnkem.com

[D05] 访问与修改元素
来源：http://yrs.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qjn.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wrf.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vsi.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://kxf.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://bfb.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://qzr.fengsongda.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://grh.redwolf501.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ngp.epnwcf.com

[D06] 数组长度
来源：http://uft.ydjk.org.cn

Py:   len(arr)
来源：http://gqo.iojbl.cn

PHP:  count($arr);
来源：http://jis.cucudq.cn

JS:   arr.length
来源：http://xah.yfazqb.com

TS:   arr.length
来源：http://rna.gotoacloud.top

Java: list.size();
来源：http://byc.sxryk.cn

Go:   len(arr)
来源：http://jfo.gzhubu.top

Ruby: arr.length; arr.size
来源：http://ybx.xinyue.icu

C#:   list.Count;
来源：http://oas.bjfxy.top

[D07] 切片 / 取子数组
来源：http://dzn.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bhn.havefunace.top

PHP:  array_slice($arr, 1, 3);
来源：http://ebi.yj202588.top

JS:   arr.slice(1, 4);
来源：http://ifr.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://yjn.hongshengwenyu.top

Java: list.subList(1, 4);
来源：http://ysq.wangshuangyany.cn

Go:   arr[1:4]
来源：http://cli.gogol.net.cn

Ruby: arr[1, 3]
来源：http://fnc.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://xcm.hcnkem.com

[D08] 合并两个数组
来源：http://vsb.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://vym.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://oxk.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qlv.gaohongyu789.top

TS:   [...a, ...b];
来源：http://qlv.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bsp.tarul.cn

Go:   append(a, b...)
来源：http://inf.xziqi.cn

Ruby: a + b;  a.concat(b)
来源：http://pag.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://lwm.zhaomingkeji.xyz

[D09] 排序（升序）
来源：http://ajc.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://slx.haohaochexian.top

PHP:  sort($arr);
来源：http://hkt.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xyt.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lfn.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wyf.chenjidiqi.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tvp.9152youxi.cn

Ruby: arr.sort
来源：http://zqe.nanxuanxn.top

C#:   list.Sort();
来源：http://kjz.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://sqo.zhengqikj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sla.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dcd.cheryme.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://edx.chenzaomai.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ygm.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://odc.meibo888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tvy.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ddj.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wpc.havefunace.top

[D11] 反转数组
来源：http://pte.birdmap.top

Py:   arr[::-1];  arr.reverse()
来源：http://zjh.shanyushiyangkeji.top

PHP:  array_reverse($arr);
来源：http://vuu.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vxg.gogol.net.cn

TS:   [...arr].reverse();
来源：http://ckm.quarkkingdee.top

Java: Collections.reverse(list);
来源：http://bxg.ybcxt.top

Go:   slices.Reverse(arr)
来源：http://rue.nanxuanxn.top

Ruby: arr.reverse
来源：http://lsa.yj20258.top

C#:   list.Reverse();
来源：http://vlr.sysykeji.top

[D12] 查找元素下标
来源：http://bnu.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://sxi.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://thw.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kng.guannengcc.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iof.yj20258.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://szg.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://ymj.sysykeji.top

Ruby: arr.index(x)
来源：http://fvj.fzhhl.top

C#:   list.IndexOf(x);
来源：http://npu.jinghuilouyu.cn

[D13] 过滤（保留满足条件的）
来源：http://pkc.tanke756.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mrm.aizwys.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tvn.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://tfi.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://zcb.redwolf501.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fec.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dkq.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://dsd.xylfe.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ujr.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://dpc.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zfx.zdqjudy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://grf.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://gha.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://ehw.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ejz.zhongyouzk.top

Go:   // 手写循环
来源：http://wwg.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://ifm.0kj1m.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sok.feifeiyinyue.top

[D15] 去重
来源：http://fbd.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rag.yuanzhike.top

PHP:  array_unique($arr);
来源：http://avg.aizwys.cn

JS:   [...new Set(arr)]
来源：http://jdk.guannengcc.top

TS:   [...new Set(arr)]
来源：http://ovz.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://opn.sysykeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://uur.jlsjyb.cn

Ruby: arr.uniq
来源：http://psq.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://meh.zhaomingkeji.xyz

[D16] 求和与平均值
来源：http://aic.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xbs.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nhv.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://isl.ydzc1.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nys.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lwm.zdbjq.cn

Go:   // 手写循环累加
来源：http://pht.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://azq.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://jfh.0kj1m.cn

[D17] 最大值与最小值
来源：http://afx.yvedp.cn

Py:   max(arr);  min(arr)
来源：http://mwf.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://ofg.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ubc.gotoacloud.top

TS:   Math.max(...arr);
来源：http://ugb.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://zsk.bbcook.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tdm.gaohongyu789.top

Ruby: arr.max;  arr.min
来源：http://ane.bjfxy.top

C#:   list.Max();  list.Min()
来源：http://hoh.bjfxy.top

[D18] 扁平化嵌套数组
来源：http://yvj.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wga.nwbrower.top

PHP:  array_merge(...$nested);
来源：http://hnx.fengsongda.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uwg.gotoacloud.top

TS:   nested.flat();
来源：http://nyd.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ymy.smart0.xyz

Go:   // 手写双层循环
来源：http://sdz.shangyingyoupin.top

Ruby: nested.flatten
来源：http://loh.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://iyb.yuxming.cn

[D19] 按字段分组
来源：http://ltk.birdmap.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://trt.yj20258888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eth.zhijiandao.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tvh.sufxvd.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nls.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://miq.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://pag.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kae.pycfn.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://adw.ivvv.top

[D20] 统计每个元素出现次数
来源：http://npd.cucudq.cn

Py:   Counter(arr)
来源：http://dap.shanyushiyangtech.top

PHP:  array_count_values($arr);
来源：http://tei.redwolf501.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vys.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hpi.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cdz.tarul.cn

Go:   // 手写 map[T]int
来源：http://plq.daxiang520.top

Ruby: arr.tally
来源：http://nnr.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jvu.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://eie.nanxuanxn.top

Py:   x in arr
来源：http://jug.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://kql.haohaochexian.top

JS:   arr.includes(x)
来源：http://ffv.uphjek.com

TS:   arr.includes(x)
来源：http://bxt.zhengqikj.top

Java: list.contains(x)
来源：http://ijj.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://smo.yuxming.cn

Ruby: arr.include?(x)
来源：http://hrb.fengsongda.top

C#:   list.Contains(x)
来源：http://euz.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://bqh.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zpn.xuetiantiany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://llx.hesvh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://srp.zycfv.cn

TS:   [...arr];
来源：http://zos.fehbvm.com

Java: new ArrayList<>(list);
来源：http://rdx.jqgufenzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://kom.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://mgt.bbcook.cn

C#:   new List<int>(list);
来源：http://bwq.andypj.xyz


<!-- 参考信息 -->