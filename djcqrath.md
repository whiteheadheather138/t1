代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wqo.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dhk.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yut.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xqa.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zkl.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tvw.yuanzhike.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://igc.hysaishi.cn

[C09] 递归
来源：http://ute.jlsjyb.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ksg.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uba.shuidangran.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://weh.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wzz.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mck.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rqt.feifeiyinyue.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qvq.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yys.zhoulong.xyz

[C10] 变量作用域
来源：http://oor.nwbrower.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vjl.yj202588.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://myc.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://udi.0kj1m.cn

TS:   同 JS
来源：http://thh.wangdashe.top

Java: 方法内为块级作用域
来源：http://qsq.jianghu66.top

Go:   花括号块级作用域
来源：http://fem.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yut.gzhubu.top

C#:   块级作用域
来源：http://aaa.pycfn.com

[C11] 模块导入与导出
来源：http://uov.yongpay.top

Py:   from module import func
来源：http://mja.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ien.ydzc1.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vkm.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wbq.hnxiangtu.top

Java: import java.util.List;
来源：http://rcm.jinghuilouyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aoa.sufxvd.cn

Ruby: require "json"; require_relative "./util"
来源：http://flx.uphjek.com

C#:   using System.Text;
来源：http://gqh.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://jzb.sxryk.cn

Py:   (lambda: print("run"))()
来源：http://gny.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://fjl.vqdsnc.cn

JS:   (() => { console.log("run"); })();
来源：http://lbp.yueranfly.top

TS:   (() => { console.log("run"); })();
来源：http://ntu.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ljl.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://cso.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://yen.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bmp.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://jtf.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gbo.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tqm.shanyushiyangtech.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gey.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sax.redwolf501.top

Java: int add(int a, int b) { return a + b; }
来源：http://mmd.fehbvm.com

Go:   func add(a, b int) int
来源：http://kxw.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kae.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://brm.nanxuanxn.top

[C14] 泛型函数
来源：http://ela.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zdq.cdnleiting.top

PHP:  // 无泛型
来源：http://nfe.zhongyouzk.top

JS:   // 无泛型
来源：http://omo.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uvd.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uqg.yuanzhike.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dsl.mhx1999.top

Ruby: # 无泛型
来源：http://htx.shanyushiyangtech.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ebi.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://rvp.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mcn.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://ubx.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lej.feifeiyinyue.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xcl.tanke756.top

Java: // 无解构
来源：http://xzz.xuanzx.com

Go:   // 无解构
来源：http://ixt.bbcook.cn

Ruby: a, b = pair
来源：http://tbe.jiagoushi.top

C#:   var (a, b) = pair;
来源：http://xca.fktsv.cn

[C16] 函数 / 方法重载
来源：http://okz.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ekr.sjlbkw.cn

PHP:  // 无重载
来源：http://uhq.tianlin.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://ydz.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://zlp.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lmg.ehwqpu.com

Go:   // 无重载：用不同函数名
来源：http://juk.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://yyd.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oyk.tianlin.xyz

================================================================================
来源：http://ujd.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://hfa.yfazqb.com

================================================================================
来源：http://xuo.fktsv.cn

[D01] 创建数组 / 列表
来源：http://jiz.shuidangran.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ede.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gfv.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uli.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://qgo.jianghu66.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tdm.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://hzs.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://tdl.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gzo.yongpay.top

[D02] 追加元素到末尾
来源：http://jgv.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xdk.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fhd.gotoacloud.top

JS:   arr.push(4);
来源：http://oyp.tarul.cn

TS:   arr.push(4);
来源：http://qoi.fanxiaobao.xyz

Java: list.add(4);
来源：http://evp.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://nuc.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://dsg.shanyushiyangtech.top

C#:   list.Add(4);
来源：http://jsb.ybcxt.top

[D03] 在指定位置插入元素
来源：http://rps.zhixingplan.top

Py:   arr.insert(0, 0)
来源：http://vft.gzhubu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://clr.zhaomingkeji.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wnq.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://dfc.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://tvf.tianlin.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ckx.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ohj.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://fdm.pengpengdd.cyou

[D04] 删除元素
来源：http://hil.yvedp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vdy.ybcxt.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hvm.tanke756.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vay.gotoacloud.top

TS:   arr.splice(0, 1);
来源：http://rmb.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fkq.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://imp.gotoacloud.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://amf.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qrf.cheryme.top

[D05] 访问与修改元素
来源：http://jke.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sez.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mbu.hywenlv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gpk.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://aof.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ija.nanxinkj.top

Go:   arr[0]; arr[0] = 9
来源：http://ufo.vqdsnc.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fhl.andypj.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xmi.52xcode.cn

[D06] 数组长度
来源：http://zme.xuanzx.com

Py:   len(arr)
来源：http://zew.yj20258.top

PHP:  count($arr);
来源：http://pqr.vehdjk.com

JS:   arr.length
来源：http://iss.aibaodan.cn

TS:   arr.length
来源：http://xwv.sjlbkw.cn

Java: list.size();
来源：http://iwc.yuanzhike.top

Go:   len(arr)
来源：http://bxn.ybcxt.top

Ruby: arr.length; arr.size
来源：http://cdh.0kj1m.cn

C#:   list.Count;
来源：http://wtr.jianghu66.top

[D07] 切片 / 取子数组
来源：http://yal.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zdn.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://voz.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://xtm.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://ljj.hfpthk.cn

Java: list.subList(1, 4);
来源：http://pxz.sysykeji.top

Go:   arr[1:4]
来源：http://iii.zhixingplan.top

Ruby: arr[1, 3]
来源：http://jqe.cashguo.top

C#:   list.GetRange(1, 3);
来源：http://gze.shangyingyoupin.top

[D08] 合并两个数组
来源：http://zpj.shuidangran.top

Py:   a + b;  a.extend(b)
来源：http://lqi.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://hla.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bba.redwolf501.top

TS:   [...a, ...b];
来源：http://irn.ybcxt.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uhr.yvedp.cn

Go:   append(a, b...)
来源：http://lew.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://wuy.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://mqx.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://jwx.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://bdk.c1oappe.top

PHP:  sort($arr);
来源：http://pke.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://crs.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qal.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://teo.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zuo.hcnkem.com

Ruby: arr.sort
来源：http://lyw.chenlongwang.top

C#:   list.Sort();
来源：http://ach.hongshengwenyu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://afh.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://izt.yfazqb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tmc.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nzk.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lvz.sweek.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://giw.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cvx.aibaodan.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gvc.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tkb.aizwys.cn

[D11] 反转数组
来源：http://ruf.cucudq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zcy.pengpengdd.cyou

PHP:  array_reverse($arr);
来源：http://xnj.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lpz.svipenyu.cn

TS:   [...arr].reverse();
来源：http://emq.shanyushiyangkeji.top

Java: Collections.reverse(list);
来源：http://sfl.smart0.xyz

Go:   slices.Reverse(arr)
来源：http://hsx.fehbvm.com

Ruby: arr.reverse
来源：http://aqy.zdbjq.cn

C#:   list.Reverse();
来源：http://ltg.xuanzx.com

[D12] 查找元素下标
来源：http://nyj.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://umh.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://szp.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qbi.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://izz.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jnj.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://krn.xuetiantiany.cn

Ruby: arr.index(x)
来源：http://ibh.fengsongda.top

C#:   list.IndexOf(x);
来源：http://vkh.316326.xyz

[D13] 过滤（保留满足条件的）
来源：http://xmg.tanke756.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iyh.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rdh.shanyushiyangtech.top

JS:   arr.filter(x => x > 3)
来源：http://pwk.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://vfy.zhoulong.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yzd.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tlb.gzhubu.top

Ruby: arr.select { |x| x > 3 }
来源：http://gvx.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vac.sjlbkw.cn

[D14] 映射转换（每个元素变形）
来源：http://rcr.fehbvm.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://upn.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bvi.snrcjt.cn

JS:   arr.map(x => x * 2)
来源：http://xnu.shzxlz.cn

TS:   arr.map(x => x * 2)
来源：http://ggb.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kcy.cdnleiting.top

Go:   // 手写循环
来源：http://ode.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://jpq.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jcs.daxiang520.top

[D15] 去重
来源：http://xgi.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ffu.zycfv.cn

PHP:  array_unique($arr);
来源：http://ljj.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://eua.cheryme.top

TS:   [...new Set(arr)]
来源：http://rjj.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://keq.ybcxt.top

Go:   // 用 map[T]struct{} 手写
来源：http://scg.pengpengdd.cyou

Ruby: arr.uniq
来源：http://yix.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://mfj.guowangkeji.top

[D16] 求和与平均值
来源：http://yfd.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://whz.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gmf.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eoy.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oop.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hnm.nwbrower.top

Go:   // 手写循环累加
来源：http://ats.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kbf.dashuyun.cn

C#:   list.Sum();  list.Average()
来源：http://lzc.wangdashe.top

[D17] 最大值与最小值
来源：http://uql.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://tpp.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://uqm.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tho.jianghu66.top

TS:   Math.max(...arr);
来源：http://wrm.ywan-chungtsiang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vlr.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://top.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://zqy.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://drz.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://nrv.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lvc.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://oqb.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dys.jlsjyb.cn

TS:   nested.flat();
来源：http://iqf.zhaomingkeji.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cpu.snrcjt.cn

Go:   // 手写双层循环
来源：http://drz.chenzaomai.com

Ruby: nested.flatten
来源：http://dxz.ppjwa.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://guo.birdmap.top

[D19] 按字段分组
来源：http://pzv.iojbl.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://utg.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nsh.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fke.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://euq.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lrq.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://xck.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tgw.mhx1999.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dcw.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://yld.sufxvd.cn

Py:   Counter(arr)
来源：http://scv.smart0.xyz

PHP:  array_count_values($arr);
来源：http://byp.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dxy.tarul.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nig.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jgd.yj20258888.top

Go:   // 手写 map[T]int
来源：http://oih.wangshuangyany.cn

Ruby: arr.tally
来源：http://vzq.52xcode.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ump.wangdashe.top

[D21] 判断是否包含某元素
来源：http://mvc.sysykeji.top

Py:   x in arr
来源：http://zkk.xingfuxueyuan.xyz

PHP:  in_array($x, $arr, true);
来源：http://xry.fktsv.cn

JS:   arr.includes(x)
来源：http://uyz.ivvv.top

TS:   arr.includes(x)
来源：http://afo.52xcode.cn

Java: list.contains(x)
来源：http://ggp.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://wzk.ctjpmb.com

Ruby: arr.include?(x)
来源：http://yst.yfazqb.com

C#:   list.Contains(x)
来源：http://wpn.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://hcz.sxryk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bzx.xingfuxueyuan.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tft.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hmt.316326.xyz

TS:   [...arr];
来源：http://vnb.meibo888.top

Java: new ArrayList<>(list);
来源：http://ygq.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://lmv.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://vvs.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://adh.0kj1m.cn

[D23] reduce 累积计算
来源：http://fxr.shzxlz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nam.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cic.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rmq.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gns.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mfh.jinghuilouyu.cn

Go:   // 手写循环
来源：http://duq.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://imh.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aww.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://nuy.tanke756.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pdp.yuanzhike.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baq.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jqn.jqgufenzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://loz.smart0.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nmp.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jgp.nanxinkj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dbr.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yjj.ehwqpu.com

[D25] Set 集合去重与交并差
来源：http://aot.shanyushiyangtech.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gvr.jianghu66.top


<!-- 参考信息 -->