代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://nxm.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tdi.bjfxy.top

Go:   sq := func(x int) int { return x * x }
来源：http://dgf.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://qap.hcnkem.com

C#:   Func<int, int> square = x => x * x;
来源：http://vtq.hammf.cn

[C07] 把函数作为参数传入
来源：http://glo.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ntq.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://frg.xuanzx.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://joh.havefunace.top

TS:   arr.map(String)
来源：http://leb.sxryk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xtn.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jqa.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://hqr.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ahk.hywenlv.cn

[C08] 闭包
来源：http://egu.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bbs.fanxiaobao.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rob.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wef.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://udm.hfpthk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qnu.xuanzx.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yte.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bqn.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mto.sweek.top

[C09] 递归
来源：http://fsv.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://esv.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fkd.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ixk.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ujb.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mii.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://alw.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ltf.jinqigfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yvc.xuanzx.com

[C10] 变量作用域
来源：http://grd.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ziw.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vqu.yanxiufei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dbx.sxryk.cn

TS:   同 JS
来源：http://pyd.bbcook.cn

Java: 方法内为块级作用域
来源：http://pnf.sxryk.cn

Go:   花括号块级作用域
来源：http://wxu.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://avw.andypj.xyz

C#:   块级作用域
来源：http://wqo.yfazqb.com

[C11] 模块导入与导出
来源：http://irq.hesvh.cn

Py:   from module import func
来源：http://rfd.snrcjt.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://frd.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://tzf.xinyue.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iie.andypj.xyz

Java: import java.util.List;
来源：http://muq.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qrn.xziqi.cn

Ruby: require "json"; require_relative "./util"
来源：http://ilt.wangshuangyany.cn

C#:   using System.Text;
来源：http://sie.sxryk.cn

[C12] 立即执行函数 IIFE
来源：http://vui.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://nwk.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://uhc.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://kcg.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://rup.ybcxt.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://izg.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://rxe.chenzaomai.com

Ruby: -> { puts "run" }.call
来源：http://pce.havefunace.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zpw.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://xcb.zhijiandao.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qrc.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vhb.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wgl.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lto.ppjwa.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ppk.haohaochexian.top

Go:   func add(a, b int) int
来源：http://zzt.aibaodan.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qcu.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tvb.mhx1999.top

[C14] 泛型函数
来源：http://lpn.fengsongda.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uec.hfpthk.cn

PHP:  // 无泛型
来源：http://okl.hcnkem.com

JS:   // 无泛型
来源：http://gtz.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://chk.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dml.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xoj.xuanzx.com

Ruby: # 无泛型
来源：http://czf.andypj.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://klz.xinyue.icu

[C15] 解构 / 展开参数
来源：http://ner.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mof.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://kzy.aizwys.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ngo.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fuw.vqdsnc.cn

Java: // 无解构
来源：http://mxa.cashguo.top

Go:   // 无解构
来源：http://iax.xylfe.cn

Ruby: a, b = pair
来源：http://thh.zhengqikj.top

C#:   var (a, b) = pair;
来源：http://usc.316326.xyz

[C16] 函数 / 方法重载
来源：http://lns.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ilr.ctjpmb.com

PHP:  // 无重载
来源：http://hyn.jqgufenzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://omc.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://ecv.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zyr.guannengcc.top

Go:   // 无重载：用不同函数名
来源：http://ktm.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://bcd.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cpx.cheryme.top

================================================================================
来源：http://yts.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://rki.jinqigufen.top

================================================================================
来源：http://bsn.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://oct.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qfy.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aya.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fsa.bbcook.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lxb.xylfe.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bjm.nwbrower.top

Go:   arr := []int{1, 2, 3}
来源：http://gcc.zhixingplan.top

Ruby: arr = [1, 2, 3]
来源：http://ypq.daria6918.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nug.redwolf501.top

[D02] 追加元素到末尾
来源：http://uio.daxiang520.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fkx.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qgc.ybcxt.top

JS:   arr.push(4);
来源：http://jle.xuanzx.com

TS:   arr.push(4);
来源：http://kxk.zhoulong.xyz

Java: list.add(4);
来源：http://ppc.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://iny.yj202588.top

Ruby: arr << 4; arr.push(5)
来源：http://ohk.mhx1999.top

C#:   list.Add(4);
来源：http://cjm.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://ibn.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://unk.ivvv.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jzo.dianchejie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ktb.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://lgk.zhongyouzk.top

Java: list.add(0, 0);
来源：http://bvw.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://cqf.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fnc.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://qoi.zhengqikj.top

[D04] 删除元素
来源：http://pre.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gsx.sysykeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ljb.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qda.sufxvd.cn

TS:   arr.splice(0, 1);
来源：http://ixw.guannengcc.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ynu.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lkw.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bzq.jiagoushi.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nbu.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://wep.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dwp.ydzc1.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ujw.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cog.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://ame.shanyushiyangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://tyh.yj202588.top

Go:   arr[0]; arr[0] = 9
来源：http://glq.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iif.chenlongwang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rqk.guannengcc.top

[D06] 数组长度
来源：http://gst.chenjidiqi.icu

Py:   len(arr)
来源：http://xdv.dashuyun.cn

PHP:  count($arr);
来源：http://hhh.ivvv.top

JS:   arr.length
来源：http://uqs.shangyingyoupin.top

TS:   arr.length
来源：http://zms.jyoumei.cn

Java: list.size();
来源：http://tup.uphjek.com

Go:   len(arr)
来源：http://lyb.meibo888.top

Ruby: arr.length; arr.size
来源：http://ceu.ppjwa.cn

C#:   list.Count;
来源：http://nio.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://mml.9152youxi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tmv.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://cst.zycfv.cn

JS:   arr.slice(1, 4);
来源：http://isu.yueranfly.top

TS:   arr.slice(1, 4);
来源：http://rnd.52xcode.cn

Java: list.subList(1, 4);
来源：http://yiw.yanxiufei.cn

Go:   arr[1:4]
来源：http://jvj.yuanzhike.top

Ruby: arr[1, 3]
来源：http://lat.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://hdy.hcnkem.com

[D08] 合并两个数组
来源：http://ujn.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://gog.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://alu.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ber.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://ddq.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wwn.hywenlv.cn

Go:   append(a, b...)
来源：http://fqt.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://hyw.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://alu.zdqjudy.top

[D09] 排序（升序）
来源：http://aob.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://cja.ivvv.top

PHP:  sort($arr);
来源：http://iiu.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ord.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cln.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://irz.kuanghao11.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://njq.yuanzhike.top

Ruby: arr.sort
来源：http://tzh.fktsv.cn

C#:   list.Sort();
来源：http://gfh.feifeiyinyue.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xvl.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dil.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lwh.uphjek.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uyp.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lek.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ytx.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qhc.xylfe.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kqg.tian-w.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://npp.yanxiufei.cn

[D11] 反转数组
来源：http://lwu.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tif.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://hva.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lxw.316326.xyz

TS:   [...arr].reverse();
来源：http://wgx.wangshuangyany.cn

Java: Collections.reverse(list);
来源：http://sgh.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://hzo.hnxiangtu.top

Ruby: arr.reverse
来源：http://pxl.ydzc1.top

C#:   list.Reverse();
来源：http://pld.snrcjt.cn

[D12] 查找元素下标
来源：http://wyq.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://ftj.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vld.xylfe.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aql.nwbrower.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jft.birdmap.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://acv.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://gbc.xziqi.cn

Ruby: arr.index(x)
来源：http://ryy.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://mrd.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://nkf.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uwb.yangfankeji.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xvd.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://mmc.zhijiandao.cn

TS:   arr.filter(x => x > 3)
来源：http://vmc.dashuyun.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://erk.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://twk.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mex.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qqu.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://fur.sufxvd.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://opv.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oah.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://loz.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://hos.tanke756.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nis.dashuyun.cn

Go:   // 手写循环
来源：http://nam.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://ppp.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yvr.xuetiantiany.cn

[D15] 去重
来源：http://tqy.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zdt.vehdjk.com

PHP:  array_unique($arr);
来源：http://eel.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://els.cucudq.cn

TS:   [...new Set(arr)]
来源：http://tdh.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://utn.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ebw.jianghu66.top

Ruby: arr.uniq
来源：http://zgi.meibo888.top

C#:   list.Distinct().ToList()
来源：http://dxm.yueranfly.top

[D16] 求和与平均值
来源：http://oyq.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wue.ywan-chungtsiang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ems.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lym.zhijiandao.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://elb.ppjwa.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ksy.hcnkem.com

Go:   // 手写循环累加
来源：http://etr.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gis.fehbvm.com

C#:   list.Sum();  list.Average()
来源：http://emp.redwolf501.top

[D17] 最大值与最小值
来源：http://qal.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://xen.jinqigfzy.top

PHP:  max($arr);  min($arr);
来源：http://nlp.yongpay.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wam.0kj1m.cn

TS:   Math.max(...arr);
来源：http://wkn.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qtv.havefunace.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ynk.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://uhj.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://mri.mhx1999.top

[D18] 扁平化嵌套数组
来源：http://joi.smart0.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pdj.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://dct.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ryl.hcnkem.com

TS:   nested.flat();
来源：http://jif.yuxming.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zcr.hnqzz.top

Go:   // 手写双层循环
来源：http://orf.zhijiandao.cn

Ruby: nested.flatten
来源：http://dgz.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tjf.birdmap.top

[D19] 按字段分组
来源：http://key.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jhx.iojbl.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bnx.hysaishi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zab.c1oappe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://adc.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gbk.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://uxo.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://mgi.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xzg.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://itu.smart0.xyz

Py:   Counter(arr)
来源：http://owx.daxiang520.top

PHP:  array_count_values($arr);
来源：http://bee.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tun.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://epc.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gce.yanxiufei.cn

Go:   // 手写 map[T]int
来源：http://beg.jinqigufen.top

Ruby: arr.tally
来源：http://neu.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lbw.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://pjn.yueranfly.top

Py:   x in arr
来源：http://wfk.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://kdi.xingfuxueyuan.xyz

JS:   arr.includes(x)
来源：http://dki.pengpengdd.cyou

TS:   arr.includes(x)
来源：http://nou.bbcook.cn

Java: list.contains(x)
来源：http://fce.redwolf501.top

Go:   slices.Contains(arr, x)
来源：http://nqm.meibo888.top

Ruby: arr.include?(x)
来源：http://fjt.guowangkeji.top

C#:   list.Contains(x)
来源：http://els.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://vkl.chenlongwang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jkj.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://arc.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oho.gogol.net.cn

TS:   [...arr];
来源：http://fcj.jinqigfzy.top

Java: new ArrayList<>(list);
来源：http://omn.jiagoushi.top

Go:   copied := append([]int(nil), arr...)
来源：http://unm.xziqi.cn

Ruby: arr.dup;  arr.clone
来源：http://lmt.hywenlv.cn

C#:   new List<int>(list);
来源：http://ohj.vehdjk.com

[D23] reduce 累积计算
来源：http://kpy.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qcg.cqqwz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nvz.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gas.jinyuanbaomall.cn


<!-- 参考信息 -->