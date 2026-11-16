代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://myz.hfpthk.cn

Go:   return a, b
来源：http://osv.ivvv.top

Ruby: return a, b
来源：http://gzh.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://zwk.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://eys.iojbl.cn

Py:   square = lambda x: x * x
来源：http://out.havefunace.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cnd.pycfn.com

JS:   const square = x => x * x;
来源：http://wyf.gogol.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://uqf.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ule.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://uva.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://xqd.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lzn.jyoumei.cn

[C07] 把函数作为参数传入
来源：http://csx.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qkx.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://itv.feifeiyinyue.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dwg.cucudq.cn

TS:   arr.map(String)
来源：http://yys.cashguo.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rhb.andypj.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dym.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://hgo.hammf.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ihc.nanxinkj.top

[C08] 闭包
来源：http://ddo.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dlg.cucudq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jev.jiagoushi.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uwk.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vty.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://and.yuanzhike.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gxb.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pgq.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fbn.redwolf501.top

[C09] 递归
来源：http://wdo.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vlv.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zkn.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ccw.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cko.c1oappe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tce.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ock.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jho.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xfd.yj20258.top

[C10] 变量作用域
来源：http://svi.52xcode.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dyr.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ctp.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://brl.zhijiandao.cn

TS:   同 JS
来源：http://bts.epnwcf.com

Java: 方法内为块级作用域
来源：http://ztm.yonumen.top

Go:   花括号块级作用域
来源：http://fof.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gxg.zycfv.cn

C#:   块级作用域
来源：http://ycm.shuidangran.top

[C11] 模块导入与导出
来源：http://qpp.zhixingplan.top

Py:   from module import func
来源：http://zca.zhoulong.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://igl.jinqigfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://auj.pycfn.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tlq.yj202588.top

Java: import java.util.List;
来源：http://vxi.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vyo.fengsongda.top

Ruby: require "json"; require_relative "./util"
来源：http://dqg.yonumen.top

C#:   using System.Text;
来源：http://oab.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://iui.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://skn.fktsv.cn

PHP:  (function () { echo "run"; })();
来源：http://ogb.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://cql.ivvv.top

TS:   (() => { console.log("run"); })();
来源：http://rgh.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ray.xuetiantiany.cn

Go:   func() { fmt.Println("run") }()
来源：http://ruw.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://dcr.ehwqpu.com

C#:   // 无 IIFE：用静态构造函数
来源：http://osp.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://ohr.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://opz.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ggd.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gen.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mof.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://hjg.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://xel.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ntp.jqgfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://wmk.sjlbkw.cn

[C14] 泛型函数
来源：http://dag.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gwj.birdmap.top

PHP:  // 无泛型
来源：http://oku.hongshengwenyu.top

JS:   // 无泛型
来源：http://zqc.tianlin.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jug.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://omk.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xxy.yonumen.top

Ruby: # 无泛型
来源：http://rtn.wangdashe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qem.hammf.cn

[C15] 解构 / 展开参数
来源：http://dkm.uphjek.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yib.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://rzn.cucudq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yys.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gcs.tian-w.cn

Java: // 无解构
来源：http://cqi.uphjek.com

Go:   // 无解构
来源：http://zug.yfazqb.com

Ruby: a, b = pair
来源：http://xna.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://nzq.xuanzx.com

[C16] 函数 / 方法重载
来源：http://jbr.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xbh.jinghuilouyu.cn

PHP:  // 无重载
来源：http://ywv.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fnd.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://qfx.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vhb.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://rvi.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://imm.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xoo.daria6918.cn

================================================================================
来源：http://xtk.smart0.xyz

D. 数组 / 列表 / 集合
来源：http://tbw.aibaodan.cn

================================================================================
来源：http://usd.dianchejie.cn

[D01] 创建数组 / 列表
来源：http://thj.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zjn.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ccv.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pvm.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rrr.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rjk.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://lvr.aizwys.cn

Ruby: arr = [1, 2, 3]
来源：http://wlb.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xeb.hfpthk.cn

[D02] 追加元素到末尾
来源：http://yzt.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qve.fengsongda.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://krp.sweek.top

JS:   arr.push(4);
来源：http://pbt.shuidangran.top

TS:   arr.push(4);
来源：http://iow.hysaishi.cn

Java: list.add(4);
来源：http://uds.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://igf.daxiang520.top

Ruby: arr << 4; arr.push(5)
来源：http://brz.zhoulong.xyz

C#:   list.Add(4);
来源：http://hbd.daria6918.cn

[D03] 在指定位置插入元素
来源：http://njh.yanxiufei.cn

Py:   arr.insert(0, 0)
来源：http://bnt.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://txn.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mli.iojbl.cn

TS:   arr.splice(0, 0, 0);
来源：http://tpc.cashguo.top

Java: list.add(0, 0);
来源：http://muk.316326.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://nts.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bhm.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://ypt.nanxinkj.top

[D04] 删除元素
来源：http://usv.andypj.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://atv.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tks.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ifz.xziqi.cn

TS:   arr.splice(0, 1);
来源：http://thn.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://evy.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zev.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kch.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mdw.mhx1999.top

[D05] 访问与修改元素
来源：http://oig.yuanzhike.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cpz.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://you.jyoumei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mux.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://nyh.fengsongda.top

Java: list.get(0); list.set(0, 9);
来源：http://pce.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://osn.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iqc.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ceq.haohaochexian.top

[D06] 数组长度
来源：http://irb.svipenyu.cn

Py:   len(arr)
来源：http://wsu.jyoumei.cn

PHP:  count($arr);
来源：http://bsd.meibo888.top

JS:   arr.length
来源：http://cua.tianlin.xyz

TS:   arr.length
来源：http://vdo.xylfe.cn

Java: list.size();
来源：http://ecy.jianghu66.top

Go:   len(arr)
来源：http://rru.yvedp.cn

Ruby: arr.length; arr.size
来源：http://yki.gogol.net.cn

C#:   list.Count;
来源：http://wmo.ybcxt.top

[D07] 切片 / 取子数组
来源：http://nyy.yj20258888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uyw.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://nfw.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://jya.yj20258.top

TS:   arr.slice(1, 4);
来源：http://oih.cucudq.cn

Java: list.subList(1, 4);
来源：http://car.birdmap.top

Go:   arr[1:4]
来源：http://jdz.birdmap.top

Ruby: arr[1, 3]
来源：http://eri.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://xmo.guowangkeji.top

[D08] 合并两个数组
来源：http://xhd.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://ynt.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://fot.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://lbl.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://boq.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hhn.yueranfly.top

Go:   append(a, b...)
来源：http://rcw.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://zvu.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://msa.yj20258888.top

[D09] 排序（升序）
来源：http://ccv.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://nek.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://nby.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lpg.jinghuilouyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://djg.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fre.zhixingplan.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rcf.pycfn.com

Ruby: arr.sort
来源：http://zbt.ppjwa.cn

C#:   list.Sort();
来源：http://phl.iojbl.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xtg.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vxi.cashguo.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cyg.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ngt.jinyuanbaomall.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ysg.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kyv.fengsongda.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ihc.xinyue.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nac.shanyushiyangtech.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://exc.yuxming.cn

[D11] 反转数组
来源：http://elm.hongshengwenyu.top

Py:   arr[::-1];  arr.reverse()
来源：http://xuf.zdbjq.cn

PHP:  array_reverse($arr);
来源：http://ffc.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kyn.cashguo.top

TS:   [...arr].reverse();
来源：http://met.hammf.cn

Java: Collections.reverse(list);
来源：http://cxt.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://ahi.zhoulong.xyz

Ruby: arr.reverse
来源：http://stn.ehwqpu.com

C#:   list.Reverse();
来源：http://byq.haohaochexian.top

[D12] 查找元素下标
来源：http://wri.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://sfx.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gab.ybcxt.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fsa.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yup.kuanghao11.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fwg.zhiwuduotai.top

Go:   slices.Index(arr, x)
来源：http://gdp.shuidangran.top

Ruby: arr.index(x)
来源：http://ewv.guowangkeji.top

C#:   list.IndexOf(x);
来源：http://mdm.hfpthk.cn

[D13] 过滤（保留满足条件的）
来源：http://rtf.xuetiantiany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ilf.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tsi.hnqzz.top

JS:   arr.filter(x => x > 3)
来源：http://kty.cucudq.cn

TS:   arr.filter(x => x > 3)
来源：http://gig.wangshuangyany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iie.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://avy.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://tyd.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://wbj.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://ovc.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zaj.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ejj.gotoacloud.top

JS:   arr.map(x => x * 2)
来源：http://dpt.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://rou.jiagoushi.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fwf.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://xqz.haohaochexian.top

Ruby: arr.map { |x| x * 2 }
来源：http://brd.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mni.xuanzx.com

[D15] 去重
来源：http://dun.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://szh.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://ixu.zhengqikj.top

JS:   [...new Set(arr)]
来源：http://gos.fanxiaobao.xyz

TS:   [...new Set(arr)]
来源：http://gms.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://brq.kuanghao11.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zev.ybcxt.top

Ruby: arr.uniq
来源：http://rmo.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://crd.yueranfly.top

[D16] 求和与平均值
来源：http://maz.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kbt.yuxming.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kcs.hnxiangtu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qcm.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xdb.9152youxi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nyx.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://xpn.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zwn.havefunace.top

C#:   list.Sum();  list.Average()
来源：http://bvg.aibaodan.cn

[D17] 最大值与最小值
来源：http://mxp.52xcode.cn

Py:   max(arr);  min(arr)
来源：http://sck.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://ynx.yj20258888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fst.zhongyouzk.top

TS:   Math.max(...arr);
来源：http://twf.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qwv.dianchejie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://beq.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://swd.ctjpmb.com

C#:   list.Max();  list.Min()
来源：http://xgl.zhiwuduotai.top

[D18] 扁平化嵌套数组
来源：http://yxy.bbcook.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://trl.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://wqo.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ktk.nwbrower.top

TS:   nested.flat();
来源：http://vzm.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sha.cashguo.top

Go:   // 手写双层循环
来源：http://tqa.ydjk.org.cn

Ruby: nested.flatten
来源：http://eza.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pvz.tian-w.cn

[D19] 按字段分组
来源：http://vjh.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ovx.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dbs.shuidangran.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nuy.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hyb.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ove.dashuyun.cn

Go:   // 手写 map[string][]T
来源：http://ndb.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rte.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xby.yvedp.cn

[D20] 统计每个元素出现次数
来源：http://qpw.haohaochexian.top

Py:   Counter(arr)
来源：http://gkw.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://ovx.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kcs.mhx1999.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lbu.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://awz.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://feg.sysykeji.top

Ruby: arr.tally
来源：http://fmo.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lem.sweek.top

[D21] 判断是否包含某元素
来源：http://ndz.ydjk.org.cn

Py:   x in arr
来源：http://luk.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://sqb.yongpay.top

JS:   arr.includes(x)
来源：http://hxv.ctjpmb.com

TS:   arr.includes(x)
来源：http://dcf.jiagoushi.top

Java: list.contains(x)
来源：http://qwi.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://zdu.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://clh.nwbrower.top

C#:   list.Contains(x)
来源：http://kig.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://yrz.nanxuanxn.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vsh.kuanghao11.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xsj.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rpb.kuanghao11.cn

TS:   [...arr];
来源：http://txm.snrcjt.cn


<!-- 参考信息 -->