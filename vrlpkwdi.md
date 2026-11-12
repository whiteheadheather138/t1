代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bgf.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xcu.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vot.redwolf501.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hms.andypj.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hxu.nanxinkj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qyt.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://syn.jlsjyb.cn

[C09] 递归
来源：http://yka.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://feh.ybcxt.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hbl.daxiang520.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ilm.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tjz.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hox.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sdf.jinqigfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cyt.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lxh.haohaochexian.top

[C10] 变量作用域
来源：http://kow.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lyq.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://inp.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wlb.hcnkem.com

TS:   同 JS
来源：http://pyc.chenzaomai.com

Java: 方法内为块级作用域
来源：http://ujx.yonumen.top

Go:   花括号块级作用域
来源：http://dlc.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://azs.sxryk.cn

C#:   块级作用域
来源：http://bun.tanke756.top

[C11] 模块导入与导出
来源：http://ubh.zdbjq.cn

Py:   from module import func
来源：http://ybr.hnxiangtu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zom.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://tds.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gup.yonumen.top

Java: import java.util.List;
来源：http://eni.jinqigufen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uwy.jqgfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://jkh.jinghuilouyu.cn

C#:   using System.Text;
来源：http://soo.vqdsnc.cn

[C12] 立即执行函数 IIFE
来源：http://tpz.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://iby.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://kru.yonumen.top

JS:   (() => { console.log("run"); })();
来源：http://jtf.guannengcc.top

TS:   (() => { console.log("run"); })();
来源：http://nea.zhijiandao.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ehw.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://yyg.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://hqi.yongpay.top

C#:   // 无 IIFE：用静态构造函数
来源：http://szj.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://kpv.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qjk.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://flh.hesvh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eok.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lat.chenzaomai.com

Java: int add(int a, int b) { return a + b; }
来源：http://fbt.ppjwa.cn

Go:   func add(a, b int) int
来源：http://nil.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://drp.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mfn.havefunace.top

[C14] 泛型函数
来源：http://gwf.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hjf.vqdsnc.cn

PHP:  // 无泛型
来源：http://kiu.jlsjyb.cn

JS:   // 无泛型
来源：http://opc.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wnc.meibo888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://unp.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xvs.aizwys.cn

Ruby: # 无泛型
来源：http://bsh.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://elo.shuidangran.top

[C15] 解构 / 展开参数
来源：http://qia.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fpq.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://zpj.shanyushiyangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ecn.jinghuilouyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://amn.kuanghao11.cn

Java: // 无解构
来源：http://tmq.chenzaomai.com

Go:   // 无解构
来源：http://xfs.gzhubu.top

Ruby: a, b = pair
来源：http://ily.ydzc1.top

C#:   var (a, b) = pair;
来源：http://zdg.ybcxt.top

[C16] 函数 / 方法重载
来源：http://cvr.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xgv.havefunace.top

PHP:  // 无重载
来源：http://uak.zycfv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oyi.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://ttc.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nml.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://gky.shzxlz.cn

Ruby: # 无重载：靠动态参数
来源：http://yln.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rot.zycfv.cn

================================================================================
来源：http://eka.smart0.xyz

D. 数组 / 列表 / 集合
来源：http://qrj.zycfv.cn

================================================================================
来源：http://vwm.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://hds.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://spw.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dcv.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sea.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pom.sweek.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dno.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://exb.ehwqpu.com

Ruby: arr = [1, 2, 3]
来源：http://jhm.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bgf.9152youxi.cn

[D02] 追加元素到末尾
来源：http://oay.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wnw.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ozl.dashuyun.cn

JS:   arr.push(4);
来源：http://jru.yj20258.top

TS:   arr.push(4);
来源：http://ssc.jlsjyb.cn

Java: list.add(4);
来源：http://qrb.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://lou.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://hww.dashuyun.cn

C#:   list.Add(4);
来源：http://pxi.sysykeji.top

[D03] 在指定位置插入元素
来源：http://ddy.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://xeu.jiagoushi.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nnz.cqqwz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mna.zdbjq.cn

TS:   arr.splice(0, 0, 0);
来源：http://wxj.birdmap.top

Java: list.add(0, 0);
来源：http://ojl.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://dwc.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bhe.shanyushiyangkeji.top

C#:   list.Insert(0, 0);
来源：http://dmx.guannengcc.top

[D04] 删除元素
来源：http://llv.quarkkingdee.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://use.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dqr.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ktm.svipenyu.cn

TS:   arr.splice(0, 1);
来源：http://dvg.yj20258.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bvs.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nru.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jfe.gzhubu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kfy.hesvh.cn

[D05] 访问与修改元素
来源：http://icz.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zqc.fktsv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hnh.jianghu66.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jxn.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://vms.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://oco.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://pvw.jqgfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rfg.zhongyouzk.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dfd.yangfankeji.com

[D06] 数组长度
来源：http://jdy.sxryk.cn

Py:   len(arr)
来源：http://whb.bbcook.cn

PHP:  count($arr);
来源：http://flr.fktsv.cn

JS:   arr.length
来源：http://vlh.hywenlv.cn

TS:   arr.length
来源：http://qjq.yfazqb.com

Java: list.size();
来源：http://yku.zhixingplan.top

Go:   len(arr)
来源：http://cys.bjfxy.top

Ruby: arr.length; arr.size
来源：http://vtg.shzxlz.cn

C#:   list.Count;
来源：http://alc.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://txs.andypj.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://myv.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://fdh.hysaishi.cn

JS:   arr.slice(1, 4);
来源：http://uis.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://dry.jqgfzy.top

Java: list.subList(1, 4);
来源：http://sgg.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://pej.cdnleiting.top

Ruby: arr[1, 3]
来源：http://kcc.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://goh.fktsv.cn

[D08] 合并两个数组
来源：http://zwu.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://rye.andypj.xyz

PHP:  array_merge($a, $b);
来源：http://rjn.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pjl.bbcook.cn

TS:   [...a, ...b];
来源：http://ukz.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yed.zhiwuduotai.top

Go:   append(a, b...)
来源：http://snm.zycfv.cn

Ruby: a + b;  a.concat(b)
来源：http://msl.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://foa.jianghu66.top

[D09] 排序（升序）
来源：http://che.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://ewp.nwbrower.top

PHP:  sort($arr);
来源：http://hnd.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://twj.jlsjyb.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bno.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bov.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://arr.havefunace.top

Ruby: arr.sort
来源：http://ifc.ppjwa.cn

C#:   list.Sort();
来源：http://ynx.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zpq.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rox.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kwc.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nfn.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oge.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ycw.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xot.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ugq.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vkv.jinqigfzy.top

[D11] 反转数组
来源：http://ebv.xziqi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zge.meibo888.top

PHP:  array_reverse($arr);
来源：http://ayi.sjlbkw.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ary.xinyue.icu

TS:   [...arr].reverse();
来源：http://kic.zycfv.cn

Java: Collections.reverse(list);
来源：http://fks.wangshuangyany.cn

Go:   slices.Reverse(arr)
来源：http://pne.wangshuangyany.cn

Ruby: arr.reverse
来源：http://ttq.hysaishi.cn

C#:   list.Reverse();
来源：http://upf.chenjidiqi.icu

[D12] 查找元素下标
来源：http://par.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://hyr.dianchejie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lkr.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sqo.fehbvm.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vwd.jinqigufen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fxp.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://jly.uphjek.com

Ruby: arr.index(x)
来源：http://tlq.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://dvs.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://vwr.hywenlv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wdq.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dpk.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://ohq.0kj1m.cn

TS:   arr.filter(x => x > 3)
来源：http://uwm.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gml.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vyk.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://epb.hywenlv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dtz.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://nmj.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cnp.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gqh.xinyue.icu

JS:   arr.map(x => x * 2)
来源：http://kej.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://wws.ywan-chungtsiang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tgp.zhijiandao.cn

Go:   // 手写循环
来源：http://gdm.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://vvf.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nrv.shangyingyoupin.top

[D15] 去重
来源：http://ifp.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://opq.xingfuxueyuan.xyz

PHP:  array_unique($arr);
来源：http://bkb.iojbl.cn

JS:   [...new Set(arr)]
来源：http://dlg.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://ook.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://geg.yongpay.top

Go:   // 用 map[T]struct{} 手写
来源：http://utc.daria6918.cn

Ruby: arr.uniq
来源：http://asc.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://hxk.xuanzx.com

[D16] 求和与平均值
来源：http://dxg.cqqwz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ewk.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bxe.gotoacloud.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fvk.c1oappe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jff.jyoumei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ohe.jinqigufen.top

Go:   // 手写循环累加
来源：http://vof.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://auy.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://kkf.jyoumei.cn

[D17] 最大值与最小值
来源：http://xrc.hesvh.cn

Py:   max(arr);  min(arr)
来源：http://qgb.zdbjq.cn

PHP:  max($arr);  min($arr);
来源：http://byk.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ugj.pycfn.com

TS:   Math.max(...arr);
来源：http://utb.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://sgf.dianchejie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nkd.ppjwa.cn

Ruby: arr.max;  arr.min
来源：http://anb.sysykeji.top

C#:   list.Max();  list.Min()
来源：http://ain.meibo888.top

[D18] 扁平化嵌套数组
来源：http://xja.vqdsnc.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ocn.yj202588.top

PHP:  array_merge(...$nested);
来源：http://mnz.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pny.sysykeji.top

TS:   nested.flat();
来源：http://afq.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pgq.xinyue.icu

Go:   // 手写双层循环
来源：http://ujh.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://cdr.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ltz.nwbrower.top

[D19] 按字段分组
来源：http://tvm.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://snf.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jjq.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zex.jqgfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vfj.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://izb.52xcode.cn

Go:   // 手写 map[string][]T
来源：http://rci.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tql.cashguo.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uhg.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://dto.xinyue.icu

Py:   Counter(arr)
来源：http://mhu.yj202588.top

PHP:  array_count_values($arr);
来源：http://afg.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eas.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dcl.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uob.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://klf.ydzc1.top

Ruby: arr.tally
来源：http://hyr.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iaz.wangdashe.top

[D21] 判断是否包含某元素
来源：http://bnd.jinyuanbaomall.cn

Py:   x in arr
来源：http://efm.epnwcf.com

PHP:  in_array($x, $arr, true);
来源：http://ywj.fzhhl.top

JS:   arr.includes(x)
来源：http://fkp.zhoulong.xyz

TS:   arr.includes(x)
来源：http://gfk.jinqigufen.top

Java: list.contains(x)
来源：http://rdr.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://lwf.gogol.net.cn

Ruby: arr.include?(x)
来源：http://sex.cqqwz.cn

C#:   list.Contains(x)
来源：http://agg.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://vsr.svipenyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://awr.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wsi.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tsz.zycfv.cn

TS:   [...arr];
来源：http://aah.vehdjk.com

Java: new ArrayList<>(list);
来源：http://lhv.yanxiufei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bnj.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://npx.zhiwuduotai.top

C#:   new List<int>(list);
来源：http://qha.bbcook.cn

[D23] reduce 累积计算
来源：http://gxw.shanyushiyangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gjy.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ptc.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ncs.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fgl.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bfa.aibaodan.cn

Go:   // 手写循环
来源：http://bnn.pycfn.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qcx.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vhv.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://yle.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dpq.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nrs.smart0.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mts.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mwj.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oly.hnxiangtu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ewh.fktsv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aaq.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cpx.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://pmc.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vsk.yangfankeji.com


<!-- 参考信息 -->