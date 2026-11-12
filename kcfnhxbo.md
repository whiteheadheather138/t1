代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://zbt.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://vhr.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://euz.gzhubu.top

[C05] 返回多个值
来源：http://ges.jinqigufen.top

Py:   return a, b
来源：http://jjc.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://sgi.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://mzg.fzhhl.top

TS:   return { a, b };
来源：http://coy.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mzm.hammf.cn

Go:   return a, b
来源：http://rdt.dianchejie.cn

Ruby: return a, b
来源：http://aoo.shanyushiyangtech.top

C#:   return (a, b);              // ValueTuple
来源：http://wwj.bjfxy.top

[C06] 匿名函数 / lambda
来源：http://siu.smart0.xyz

Py:   square = lambda x: x * x
来源：http://jhv.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lrj.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://amm.yj20258888.top

TS:   const square = (x: number): number => x * x;
来源：http://kxc.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qrq.cqqwz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vqp.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://ehk.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://iuc.yfazqb.com

[C07] 把函数作为参数传入
来源：http://xgy.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iod.zhiwuduotai.top

PHP:  array_map("strtoupper", $arr);
来源：http://ike.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pdb.yongpay.top

TS:   arr.map(String)
来源：http://zlt.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xjl.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oqt.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://tsz.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kus.zhixingplan.top

[C08] 闭包
来源：http://gik.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hxr.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jyx.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uhb.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jeo.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pcu.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ore.yonumen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://frm.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yas.ivvv.top

[C09] 递归
来源：http://yjq.hnxiangtu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zby.zhongyouzk.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xcw.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mzk.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wqw.fanxiaobao.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pnc.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ifn.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://afj.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kow.epnwcf.com

[C10] 变量作用域
来源：http://qvg.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://udb.quarkkingdee.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yct.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://abi.yj202588.top

TS:   同 JS
来源：http://map.birdmap.top

Java: 方法内为块级作用域
来源：http://bmm.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://oyb.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ouk.quarkkingdee.top

C#:   块级作用域
来源：http://tqt.yj20258888.top

[C11] 模块导入与导出
来源：http://dgm.yueranfly.top

Py:   from module import func
来源：http://ipi.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eqe.ppjwa.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jfu.sxryk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jqg.yonumen.top

Java: import java.util.List;
来源：http://bio.aibaodan.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://was.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://gze.nanxinkj.top

C#:   using System.Text;
来源：http://wvb.chenlongwang.top

[C12] 立即执行函数 IIFE
来源：http://umx.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://jxc.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://pup.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://hzw.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://zfw.yongpay.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vnj.hammf.cn

Go:   func() { fmt.Println("run") }()
来源：http://qac.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://wgx.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wcz.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://tif.zhoulong.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sgi.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ole.dianchejie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xdq.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://utk.jlsjyb.cn

Java: int add(int a, int b) { return a + b; }
来源：http://use.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://waa.yj20258.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fng.cheryme.top

C#:   int Add(int a, int b) => a + b;
来源：http://wtj.yfazqb.com

[C14] 泛型函数
来源：http://tar.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ijy.bbcook.cn

PHP:  // 无泛型
来源：http://mas.hywenlv.cn

JS:   // 无泛型
来源：http://lit.kuanghao11.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://arf.nanxuanxn.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://stg.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fbh.meibo888.top

Ruby: # 无泛型
来源：http://utt.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xoh.ybcxt.top

[C15] 解构 / 展开参数
来源：http://ltr.jinyuanbaomall.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zvh.yj202588.top

PHP:  [$a, $b] = $pair;
来源：http://jsk.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jne.jqgfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fnq.epnwcf.com

Java: // 无解构
来源：http://vik.zhixingplan.top

Go:   // 无解构
来源：http://fto.sjlbkw.cn

Ruby: a, b = pair
来源：http://qbj.hesvh.cn

C#:   var (a, b) = pair;
来源：http://ftc.pengpengdd.cyou

[C16] 函数 / 方法重载
来源：http://ezl.zhixingplan.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://okv.jyoumei.cn

PHP:  // 无重载
来源：http://ins.aibaodan.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://evg.shanyushiyangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://mog.zdqjudy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wnf.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://lar.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://pba.uphjek.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://lgr.nwbrower.top

================================================================================
来源：http://oic.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://cof.vehdjk.com

================================================================================
来源：http://pkc.yuxming.cn

[D01] 创建数组 / 列表
来源：http://djh.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fzk.hongshengwenyu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tjx.tarul.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ohl.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://cmt.fktsv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kio.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://ukh.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://flr.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xjz.nwbrower.top

[D02] 追加元素到末尾
来源：http://lnc.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hvd.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zbx.andypj.xyz

JS:   arr.push(4);
来源：http://gic.hesvh.cn

TS:   arr.push(4);
来源：http://hkm.wangshuangyany.cn

Java: list.add(4);
来源：http://hjc.gzhubu.top

Go:   arr = append(arr, 4)
来源：http://lmr.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://awl.shzxlz.cn

C#:   list.Add(4);
来源：http://pdc.yueranfly.top

[D03] 在指定位置插入元素
来源：http://yjn.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://yam.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iqx.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sue.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://kai.yuxming.cn

Java: list.add(0, 0);
来源：http://anw.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://ays.cashguo.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eey.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://era.xuetiantiany.cn

[D04] 删除元素
来源：http://dic.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lfs.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qth.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vvx.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://obr.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wle.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cij.shangyingyoupin.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://orv.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fvi.yuxming.cn

[D05] 访问与修改元素
来源：http://bvo.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zag.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://imk.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bgm.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://qxo.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://xgi.c1oappe.top

Go:   arr[0]; arr[0] = 9
来源：http://xnl.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rha.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://npt.sxryk.cn

[D06] 数组长度
来源：http://enm.jinqigfzy.top

Py:   len(arr)
来源：http://fve.aibaodan.cn

PHP:  count($arr);
来源：http://dpa.chenlongwang.top

JS:   arr.length
来源：http://bml.jlsjyb.cn

TS:   arr.length
来源：http://gwr.yueranfly.top

Java: list.size();
来源：http://zkt.zhaomingkeji.xyz

Go:   len(arr)
来源：http://ueo.gotoacloud.top

Ruby: arr.length; arr.size
来源：http://cki.chenjidiqi.icu

C#:   list.Count;
来源：http://wul.gzhubu.top

[D07] 切片 / 取子数组
来源：http://voo.sxryk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tci.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://upf.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://qpz.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://yis.zhengqikj.top

Java: list.subList(1, 4);
来源：http://qpo.sufxvd.cn

Go:   arr[1:4]
来源：http://tgs.pycfn.com

Ruby: arr[1, 3]
来源：http://eyz.jinqigufen.top

C#:   list.GetRange(1, 3);
来源：http://nmx.xuetiantiany.cn

[D08] 合并两个数组
来源：http://caa.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://zee.cheryme.top

PHP:  array_merge($a, $b);
来源：http://hxq.mhx1999.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gld.xylfe.cn

TS:   [...a, ...b];
来源：http://gmn.yueranfly.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fiw.daria6918.cn

Go:   append(a, b...)
来源：http://umc.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://ahg.jinyuanbaomall.cn

C#:   a.Concat(b).ToList()
来源：http://dyf.dashuyun.cn

[D09] 排序（升序）
来源：http://ijb.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://iav.zhiwuduotai.top

PHP:  sort($arr);
来源：http://stu.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://stk.dianchejie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wtl.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://sdz.zdbjq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yci.xuanzx.com

Ruby: arr.sort
来源：http://jbr.dianchejie.cn

C#:   list.Sort();
来源：http://nag.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kdu.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://evu.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tkn.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lbt.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dll.birdmap.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uly.shuidangran.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fzo.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mit.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dpt.shanyushiyangkeji.top

[D11] 反转数组
来源：http://gfq.jinyuanbaomall.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xwf.birdmap.top

PHP:  array_reverse($arr);
来源：http://xbr.hongshengwenyu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jxq.tianlin.xyz

TS:   [...arr].reverse();
来源：http://ioc.yongpay.top

Java: Collections.reverse(list);
来源：http://edt.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://mbm.zhiwuduotai.top

Ruby: arr.reverse
来源：http://ukm.zhengqikj.top

C#:   list.Reverse();
来源：http://dlm.cqqwz.cn

[D12] 查找元素下标
来源：http://srf.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://vjl.cheryme.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://peb.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iom.316326.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ivq.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gxq.snrcjt.cn

Go:   slices.Index(arr, x)
来源：http://jyj.aibaodan.cn

Ruby: arr.index(x)
来源：http://xno.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://ipc.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://grk.ydzc1.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://upk.yj20258.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://njr.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://fnp.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://lqz.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://led.xylfe.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bsb.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://abx.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://noc.sjlbkw.cn

[D14] 映射转换（每个元素变形）
来源：http://yva.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://thg.hywenlv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kox.bbcook.cn

JS:   arr.map(x => x * 2)
来源：http://civ.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://wjc.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://frv.dashuyun.cn

Go:   // 手写循环
来源：http://boe.gotoacloud.top

Ruby: arr.map { |x| x * 2 }
来源：http://ztq.yvedp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qee.guowangkeji.top

[D15] 去重
来源：http://iro.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qro.yfazqb.com

PHP:  array_unique($arr);
来源：http://kre.pycfn.com

JS:   [...new Set(arr)]
来源：http://npv.mhx1999.top

TS:   [...new Set(arr)]
来源：http://mfr.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lru.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://hgn.sjlbkw.cn

Ruby: arr.uniq
来源：http://gfj.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://ufx.wangdashe.top

[D16] 求和与平均值
来源：http://uvj.cdnleiting.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cpw.daxiang520.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sdv.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wbm.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://skt.dashuyun.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mnv.birdmap.top

Go:   // 手写循环累加
来源：http://lum.daria6918.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xfh.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://kjm.zdqjudy.top

[D17] 最大值与最小值
来源：http://qee.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://aac.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://dnw.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jme.gogol.net.cn

TS:   Math.max(...arr);
来源：http://oty.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xcc.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cpf.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://mzo.kuanghao11.cn

C#:   list.Max();  list.Min()
来源：http://dyy.kuanghao11.cn

[D18] 扁平化嵌套数组
来源：http://dcq.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bao.aibaodan.cn

PHP:  array_merge(...$nested);
来源：http://srj.tianlin.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mcr.redwolf501.top

TS:   nested.flat();
来源：http://cvd.jinghuilouyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zmz.dianchejie.cn

Go:   // 手写双层循环
来源：http://ixd.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://ipd.andypj.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://xrg.shanyushiyangtech.top

[D19] 按字段分组
来源：http://wky.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gmt.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zna.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://shg.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xbp.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uvy.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://fum.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://hdv.jinghuilouyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ujj.vqdsnc.cn

[D20] 统计每个元素出现次数
来源：http://xwa.nwbrower.top

Py:   Counter(arr)
来源：http://ayy.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://ddo.ydjk.org.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pdc.epnwcf.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rxb.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kas.yj20258888.top

Go:   // 手写 map[T]int
来源：http://xuj.cashguo.top

Ruby: arr.tally
来源：http://dte.wangshuangyany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://imx.jqgfzy.top

[D21] 判断是否包含某元素
来源：http://tou.xylfe.cn

Py:   x in arr
来源：http://hjb.hnqzz.top

PHP:  in_array($x, $arr, true);
来源：http://pjz.hcnkem.com

JS:   arr.includes(x)
来源：http://wjw.havefunace.top

TS:   arr.includes(x)
来源：http://tyo.tian-w.cn

Java: list.contains(x)
来源：http://esk.cheryme.top


<!-- 参考信息 -->