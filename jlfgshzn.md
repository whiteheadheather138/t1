代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://ukc.jlsjyb.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hfe.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dec.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://awv.wangshuangyany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zkl.yj202588.top

[C07] 把函数作为参数传入
来源：http://hdc.snrcjt.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yvm.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mrm.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ucb.jinqigfzy.top

TS:   arr.map(String)
来源：http://wzw.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gdc.jiagoushi.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dly.yueranfly.top

Ruby: arr.map(&:upcase)
来源：http://yxw.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://ehc.ehwqpu.com

[C08] 闭包
来源：http://vum.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eay.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://phg.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://utv.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lbi.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ogm.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sbk.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://azr.daxiang520.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://obx.52xcode.cn

[C09] 递归
来源：http://fho.jinyuanbaomall.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cnq.pycfn.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dbc.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eaz.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nvz.kuanghao11.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kly.gaohongyu789.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qbj.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ocv.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bhl.jinyuanbaomall.cn

[C10] 变量作用域
来源：http://qho.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fdl.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tnd.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://api.aibaodan.cn

TS:   同 JS
来源：http://ane.c1oappe.top

Java: 方法内为块级作用域
来源：http://hmx.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://jsh.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mky.havefunace.top

C#:   块级作用域
来源：http://fqw.tanke756.top

[C11] 模块导入与导出
来源：http://dyt.316326.xyz

Py:   from module import func
来源：http://hka.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://vkq.shuidangran.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://adv.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ssu.chenlongwang.top

Java: import java.util.List;
来源：http://jlx.ppjwa.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cum.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://jzl.nanxinkj.top

C#:   using System.Text;
来源：http://xqd.zhijiandao.cn

[C12] 立即执行函数 IIFE
来源：http://sdp.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://sww.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://ymo.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://gxy.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://bbb.iojbl.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vxz.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://qfi.ppjwa.cn

Ruby: -> { puts "run" }.call
来源：http://qak.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gls.cqqwz.cn

[C13] 类型声明 / 类型注解
来源：http://lpa.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://otb.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bno.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mbt.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ipb.sjlbkw.cn

Java: int add(int a, int b) { return a + b; }
来源：http://riy.bbcook.cn

Go:   func add(a, b int) int
来源：http://ytm.52xcode.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uey.0kj1m.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xkv.ydzc1.top

[C14] 泛型函数
来源：http://hfe.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nja.snrcjt.cn

PHP:  // 无泛型
来源：http://euw.cheryme.top

JS:   // 无泛型
来源：http://kao.redwolf501.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jmg.fzhhl.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uty.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vwk.gaohongyu789.top

Ruby: # 无泛型
来源：http://xbu.nanxuanxn.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wnl.sweek.top

[C15] 解构 / 展开参数
来源：http://niv.0kj1m.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://snw.cqqwz.cn

PHP:  [$a, $b] = $pair;
来源：http://csm.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qyx.dianchejie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xxh.snrcjt.cn

Java: // 无解构
来源：http://jpj.zdqjudy.top

Go:   // 无解构
来源：http://gkv.9152youxi.cn

Ruby: a, b = pair
来源：http://zki.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://bxv.316326.xyz

[C16] 函数 / 方法重载
来源：http://kpq.guowangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kqu.guowangkeji.top

PHP:  // 无重载
来源：http://iic.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://ojh.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://uri.yanxiufei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://snt.hnxiangtu.top

Go:   // 无重载：用不同函数名
来源：http://qdn.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://inf.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://fxd.chenjidiqi.icu

================================================================================
来源：http://wmj.uphjek.com

D. 数组 / 列表 / 集合
来源：http://xsi.ivvv.top

================================================================================
来源：http://bib.zycfv.cn

[D01] 创建数组 / 列表
来源：http://jgw.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://acb.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zef.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ukd.ctjpmb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://uft.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://acr.jiagoushi.top

Go:   arr := []int{1, 2, 3}
来源：http://quz.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://hvw.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fxa.hcnkem.com

[D02] 追加元素到末尾
来源：http://hfv.zhixingplan.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qii.hcnkem.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://slc.zycfv.cn

JS:   arr.push(4);
来源：http://cth.gogol.net.cn

TS:   arr.push(4);
来源：http://uyj.yvedp.cn

Java: list.add(4);
来源：http://dpu.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://hyr.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ery.jyoumei.cn

C#:   list.Add(4);
来源：http://tni.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://dhe.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://hmx.guowangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hug.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lvj.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://atx.yonumen.top

Java: list.add(0, 0);
来源：http://eok.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://efn.cashguo.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rwr.ivvv.top

C#:   list.Insert(0, 0);
来源：http://eoc.aibaodan.cn

[D04] 删除元素
来源：http://pik.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wqr.jiagoushi.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kxw.feifeiyinyue.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zes.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://utc.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://upi.snrcjt.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gmd.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aur.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://whs.yanxiufei.cn

[D05] 访问与修改元素
来源：http://tik.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uud.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nty.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dgy.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://jjg.52xcode.cn

Java: list.get(0); list.set(0, 9);
来源：http://arp.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://tfj.yuxming.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pwx.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kjm.jyoumei.cn

[D06] 数组长度
来源：http://ock.zhengqikj.top

Py:   len(arr)
来源：http://phn.shzxlz.cn

PHP:  count($arr);
来源：http://lkz.wangshuangyany.cn

JS:   arr.length
来源：http://tym.cheryme.top

TS:   arr.length
来源：http://rhc.hcnkem.com

Java: list.size();
来源：http://sdr.zhixingplan.top

Go:   len(arr)
来源：http://wsm.shuidangran.top

Ruby: arr.length; arr.size
来源：http://fzi.zdqjudy.top

C#:   list.Count;
来源：http://dft.uphjek.com

[D07] 切片 / 取子数组
来源：http://hye.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wne.hammf.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zsd.fktsv.cn

JS:   arr.slice(1, 4);
来源：http://gag.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://eps.gogol.net.cn

Java: list.subList(1, 4);
来源：http://zgt.shangyingyoupin.top

Go:   arr[1:4]
来源：http://cde.zhixingplan.top

Ruby: arr[1, 3]
来源：http://btw.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://cwn.chenzaomai.com

[D08] 合并两个数组
来源：http://jfl.xingfuxueyuan.xyz

Py:   a + b;  a.extend(b)
来源：http://dqb.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://buu.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ekq.bjfxy.top

TS:   [...a, ...b];
来源：http://nrj.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nrm.chenjidiqi.icu

Go:   append(a, b...)
来源：http://zrb.snrcjt.cn

Ruby: a + b;  a.concat(b)
来源：http://nnr.fengsongda.top

C#:   a.Concat(b).ToList()
来源：http://gee.ctjpmb.com

[D09] 排序（升序）
来源：http://kbw.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://bst.birdmap.top

PHP:  sort($arr);
来源：http://ybx.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jea.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ikk.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://iyc.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wyt.mhx1999.top

Ruby: arr.sort
来源：http://ygr.havefunace.top

C#:   list.Sort();
来源：http://hni.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hte.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lyj.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qxy.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xri.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vmn.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lgd.xuanzx.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uet.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ipm.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://flw.tarul.cn

[D11] 反转数组
来源：http://xzt.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://nxq.yj20258888.top

PHP:  array_reverse($arr);
来源：http://jpm.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ovw.hfpthk.cn

TS:   [...arr].reverse();
来源：http://zvz.aizwys.cn

Java: Collections.reverse(list);
来源：http://kug.xinyue.icu

Go:   slices.Reverse(arr)
来源：http://esl.andypj.xyz

Ruby: arr.reverse
来源：http://ilw.bjfxy.top

C#:   list.Reverse();
来源：http://dgk.yj20258888.top

[D12] 查找元素下标
来源：http://vre.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://nzv.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://saf.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bbg.dianchejie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://crb.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yhn.hammf.cn

Go:   slices.Index(arr, x)
来源：http://tkf.hongshengwenyu.top

Ruby: arr.index(x)
来源：http://jqz.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://csd.hnqzz.top

[D13] 过滤（保留满足条件的）
来源：http://ccc.snrcjt.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qpy.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ojf.shanyushiyangtech.top

JS:   arr.filter(x => x > 3)
来源：http://ovu.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://tps.52xcode.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wan.cqqwz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ytb.hongshengwenyu.top

Ruby: arr.select { |x| x > 3 }
来源：http://vgk.tarul.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lye.hywenlv.cn

[D14] 映射转换（每个元素变形）
来源：http://eez.hcnkem.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ztn.yuanzhike.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uhm.bbcook.cn

JS:   arr.map(x => x * 2)
来源：http://stn.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://pgh.jiagoushi.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xok.vqdsnc.cn

Go:   // 手写循环
来源：http://lij.hnqzz.top

Ruby: arr.map { |x| x * 2 }
来源：http://shy.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://igo.sxryk.cn

[D15] 去重
来源：http://vnn.sweek.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jth.hammf.cn

PHP:  array_unique($arr);
来源：http://lzx.xinyue.icu

JS:   [...new Set(arr)]
来源：http://hry.jinyuanbaomall.cn

TS:   [...new Set(arr)]
来源：http://kdt.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hic.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://idk.aibaodan.cn

Ruby: arr.uniq
来源：http://nin.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://rro.svipenyu.cn

[D16] 求和与平均值
来源：http://jrj.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kkd.xuetiantiany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://srn.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rgz.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xgm.ctjpmb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://adx.hysaishi.cn

Go:   // 手写循环累加
来源：http://kuy.cheryme.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://arv.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://usz.jiagoushi.top

[D17] 最大值与最小值
来源：http://fqj.yanxiufei.cn

Py:   max(arr);  min(arr)
来源：http://wgb.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://odk.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qxc.ivvv.top

TS:   Math.max(...arr);
来源：http://vrs.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fyb.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zxo.9152youxi.cn

Ruby: arr.max;  arr.min
来源：http://cis.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://cyd.vqdsnc.cn

[D18] 扁平化嵌套数组
来源：http://xol.fanxiaobao.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bmn.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://dwv.nanxuanxn.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://drv.cdnleiting.top

TS:   nested.flat();
来源：http://ojd.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://swf.snrcjt.cn

Go:   // 手写双层循环
来源：http://cym.zhongyouzk.top

Ruby: nested.flatten
来源：http://xxm.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ltd.zhixingplan.top

[D19] 按字段分组
来源：http://wtd.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pzy.tanke756.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tsp.hammf.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tpo.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gkw.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rap.xingfuxueyuan.xyz

Go:   // 手写 map[string][]T
来源：http://lxo.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jdr.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hbm.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://jbd.xylfe.cn

Py:   Counter(arr)
来源：http://owq.chenlongwang.top

PHP:  array_count_values($arr);
来源：http://vsp.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bqq.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zfu.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wnc.chenlongwang.top

Go:   // 手写 map[T]int
来源：http://ejo.c1oappe.top

Ruby: arr.tally
来源：http://zen.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qtb.cheryme.top

[D21] 判断是否包含某元素
来源：http://yjl.cqqwz.cn

Py:   x in arr
来源：http://fcx.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://ret.jinqigufen.top

JS:   arr.includes(x)
来源：http://bxw.meibo888.top

TS:   arr.includes(x)
来源：http://kih.daxiang520.top

Java: list.contains(x)
来源：http://caq.zdqjudy.top

Go:   slices.Contains(arr, x)
来源：http://uqr.dashuyun.cn

Ruby: arr.include?(x)
来源：http://qmt.birdmap.top

C#:   list.Contains(x)
来源：http://gle.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://rat.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eel.shuidangran.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fqn.yangfankeji.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tsb.quarkkingdee.top

TS:   [...arr];
来源：http://ajo.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://wry.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zcr.cucudq.cn

Ruby: arr.dup;  arr.clone
来源：http://onb.tarul.cn

C#:   new List<int>(list);
来源：http://wck.zhijiandao.cn

[D23] reduce 累积计算
来源：http://bco.shangyingyoupin.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qzc.316326.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hjf.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fjk.yonumen.top


<!-- 参考信息 -->