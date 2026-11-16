代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://shu.shuidangran.top

[C07] 把函数作为参数传入
来源：http://ewv.gaohongyu789.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eca.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://jaz.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iif.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://npo.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cxm.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wqa.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://ejo.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://daq.yj202588.top

[C08] 闭包
来源：http://xei.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wot.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ykl.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mmz.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://czb.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://chm.gogol.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hqu.shuidangran.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mnk.xylfe.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nsv.yongpay.top

[C09] 递归
来源：http://lph.jinyuanbaomall.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bmt.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ydy.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ldm.yangfankeji.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qvc.zhengqikj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gze.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bby.zhengqikj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aqo.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://llf.yj20258888.top

[C10] 变量作用域
来源：http://xxf.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ppo.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://utp.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mga.epnwcf.com

TS:   同 JS
来源：http://eza.jqgfzy.top

Java: 方法内为块级作用域
来源：http://cjd.hnxiangtu.top

Go:   花括号块级作用域
来源：http://bwg.pengpengdd.cyou

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zay.dashuyun.cn

C#:   块级作用域
来源：http://xwr.yangfankeji.com

[C11] 模块导入与导出
来源：http://eyj.zhongyouzk.top

Py:   from module import func
来源：http://zas.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nmg.yvedp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fqq.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hpu.redwolf501.top

Java: import java.util.List;
来源：http://sko.sweek.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ibb.tianlin.xyz

Ruby: require "json"; require_relative "./util"
来源：http://jea.svipenyu.cn

C#:   using System.Text;
来源：http://pjz.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://ssp.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://wjk.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://qty.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://ton.cqqwz.cn

TS:   (() => { console.log("run"); })();
来源：http://pvi.yongpay.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dkq.yj20258.top

Go:   func() { fmt.Println("run") }()
来源：http://qkr.yanxiufei.cn

Ruby: -> { puts "run" }.call
来源：http://myi.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://knx.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://kfa.zhoulong.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ved.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ahf.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hrj.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nmx.fzhhl.top

Java: int add(int a, int b) { return a + b; }
来源：http://jmm.ehwqpu.com

Go:   func add(a, b int) int
来源：http://fgy.fehbvm.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vth.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lmz.tanke756.top

[C14] 泛型函数
来源：http://rxy.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tjp.zhaomingkeji.xyz

PHP:  // 无泛型
来源：http://jno.haohaochexian.top

JS:   // 无泛型
来源：http://zso.tian-w.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rte.cqqwz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gvi.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://duz.ybcxt.top

Ruby: # 无泛型
来源：http://dhs.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nnw.yvedp.cn

[C15] 解构 / 展开参数
来源：http://zdi.316326.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://agv.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://yht.aizwys.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vec.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qiv.ybcxt.top

Java: // 无解构
来源：http://ebn.cashguo.top

Go:   // 无解构
来源：http://kcs.jinqigfzy.top

Ruby: a, b = pair
来源：http://wuc.yuanzhike.top

C#:   var (a, b) = pair;
来源：http://aiv.daria6918.cn

[C16] 函数 / 方法重载
来源：http://lbd.xuetiantiany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iko.gzhubu.top

PHP:  // 无重载
来源：http://res.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vht.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://qmy.guannengcc.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wgv.gotoacloud.top

Go:   // 无重载：用不同函数名
来源：http://lud.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://bjh.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://urv.redwolf501.top

================================================================================
来源：http://smj.c1oappe.top

D. 数组 / 列表 / 集合
来源：http://lox.xuetiantiany.cn

================================================================================
来源：http://mdd.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://tju.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tpq.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rnt.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ouq.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mft.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uss.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://wpx.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://xyv.yvedp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ldo.cashguo.top

[D02] 追加元素到末尾
来源：http://udi.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uwu.chenjidiqi.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xyu.ctjpmb.com

JS:   arr.push(4);
来源：http://jkx.daria6918.cn

TS:   arr.push(4);
来源：http://pgg.shanyushiyangtech.top

Java: list.add(4);
来源：http://gzx.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://uda.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://xje.yonumen.top

C#:   list.Add(4);
来源：http://lni.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://wce.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://vqt.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tzj.ppjwa.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lyq.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://txr.xinyue.icu

Java: list.add(0, 0);
来源：http://cln.hongshengwenyu.top

Go:   arr = append([]int{0}, arr...)
来源：http://gkc.tianlin.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nrg.pycfn.com

C#:   list.Insert(0, 0);
来源：http://nkr.xylfe.cn

[D04] 删除元素
来源：http://fsj.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ckt.hnxiangtu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ueg.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qdp.ctjpmb.com

TS:   arr.splice(0, 1);
来源：http://ztw.shuidangran.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yym.yj20258888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uyj.shuidangran.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://znj.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bym.hammf.cn

[D05] 访问与修改元素
来源：http://yih.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yvi.jiagoushi.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eeh.cashguo.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ara.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://hpw.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://zku.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://kvm.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ekr.0kj1m.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kwy.cucudq.cn

[D06] 数组长度
来源：http://onk.iojbl.cn

Py:   len(arr)
来源：http://sda.guannengcc.top

PHP:  count($arr);
来源：http://exa.jianghu66.top

JS:   arr.length
来源：http://elz.52xcode.cn

TS:   arr.length
来源：http://deh.kuanghao11.cn

Java: list.size();
来源：http://rsh.ydzc1.top

Go:   len(arr)
来源：http://ptw.guowangkeji.top

Ruby: arr.length; arr.size
来源：http://ksr.zhaomingkeji.xyz

C#:   list.Count;
来源：http://brg.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://ugn.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bnx.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nhu.zhaomingkeji.xyz

JS:   arr.slice(1, 4);
来源：http://vhe.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://fcy.hongshengwenyu.top

Java: list.subList(1, 4);
来源：http://pye.gaohongyu789.top

Go:   arr[1:4]
来源：http://hka.zdbjq.cn

Ruby: arr[1, 3]
来源：http://fje.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://xls.tanke756.top

[D08] 合并两个数组
来源：http://fnm.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://rfl.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://gje.pengpengdd.cyou

JS:   [...a, ...b];  a.concat(b);
来源：http://cxe.zhongyouzk.top

TS:   [...a, ...b];
来源：http://pib.hnxiangtu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jpm.cdnleiting.top

Go:   append(a, b...)
来源：http://jfo.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://vxu.vehdjk.com

C#:   a.Concat(b).ToList()
来源：http://lzo.jiagoushi.top

[D09] 排序（升序）
来源：http://pge.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://wau.jinqigufen.top

PHP:  sort($arr);
来源：http://mxt.yuxming.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://egj.9152youxi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://izs.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wiq.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ytm.chenlongwang.top

Ruby: arr.sort
来源：http://ksz.9152youxi.cn

C#:   list.Sort();
来源：http://ytz.sysykeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tnp.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rrb.fengsongda.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ywn.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dzw.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jar.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dvy.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xvq.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cct.fehbvm.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gec.yueranfly.top

[D11] 反转数组
来源：http://ofl.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://bgw.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://sej.jiagoushi.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bzw.sweek.top

TS:   [...arr].reverse();
来源：http://nwc.jianghu66.top

Java: Collections.reverse(list);
来源：http://akk.svipenyu.cn

Go:   slices.Reverse(arr)
来源：http://wmh.jiagoushi.top

Ruby: arr.reverse
来源：http://uya.gogol.net.cn

C#:   list.Reverse();
来源：http://wyc.zhijiandao.cn

[D12] 查找元素下标
来源：http://fdf.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://ere.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tym.iojbl.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tfe.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nuv.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jzs.shanyushiyangtech.top

Go:   slices.Index(arr, x)
来源：http://nmi.gogol.net.cn

Ruby: arr.index(x)
来源：http://haa.jinqigufen.top

C#:   list.IndexOf(x);
来源：http://nax.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://qax.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ago.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oaj.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://low.yueranfly.top

TS:   arr.filter(x => x > 3)
来源：http://gdq.havefunace.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tpt.cheryme.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zpo.chenzaomai.com

Ruby: arr.select { |x| x > 3 }
来源：http://qad.tarul.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cwa.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://bnj.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kbt.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://icb.xuanzx.com

JS:   arr.map(x => x * 2)
来源：http://svp.nanxinkj.top

TS:   arr.map(x => x * 2)
来源：http://twi.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://deq.yj202588.top

Go:   // 手写循环
来源：http://qyf.zhongyouzk.top

Ruby: arr.map { |x| x * 2 }
来源：http://jkn.bjfxy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mje.yangfankeji.com

[D15] 去重
来源：http://qba.hammf.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lkw.nwbrower.top

PHP:  array_unique($arr);
来源：http://uut.xingfuxueyuan.xyz

JS:   [...new Set(arr)]
来源：http://vpl.dashuyun.cn

TS:   [...new Set(arr)]
来源：http://kqd.cucudq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dza.iojbl.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eor.aibaodan.cn

Ruby: arr.uniq
来源：http://wxy.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://sdq.ybcxt.top

[D16] 求和与平均值
来源：http://drz.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://snx.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://csk.zdbjq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zid.jqgufenzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xjk.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nmp.epnwcf.com

Go:   // 手写循环累加
来源：http://fcb.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://het.havefunace.top

C#:   list.Sum();  list.Average()
来源：http://hgw.yvedp.cn

[D17] 最大值与最小值
来源：http://zkd.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://lkd.ydzc1.top

PHP:  max($arr);  min($arr);
来源：http://omw.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://poo.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://ivs.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nfh.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ovr.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://xqc.fktsv.cn

C#:   list.Max();  list.Min()
来源：http://vrm.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://gtt.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cnn.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://kfv.xziqi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eyu.nwbrower.top

TS:   nested.flat();
来源：http://qqo.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uok.hysaishi.cn

Go:   // 手写双层循环
来源：http://xxk.yuxming.cn

Ruby: nested.flatten
来源：http://zhi.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dmp.vehdjk.com

[D19] 按字段分组
来源：http://vxn.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://azm.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pae.vqdsnc.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tcy.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://usi.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://duh.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://wpp.yj202588.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://igg.shanyushiyangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rnb.316326.xyz

[D20] 统计每个元素出现次数
来源：http://evf.aizwys.cn

Py:   Counter(arr)
来源：http://vdi.fzhhl.top

PHP:  array_count_values($arr);
来源：http://rah.daria6918.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jld.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xuz.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hzb.guannengcc.top

Go:   // 手写 map[T]int
来源：http://fwp.hammf.cn

Ruby: arr.tally
来源：http://gvp.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://udu.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://ijm.hcnkem.com

Py:   x in arr
来源：http://nky.sysykeji.top

PHP:  in_array($x, $arr, true);
来源：http://opy.gotoacloud.top

JS:   arr.includes(x)
来源：http://vwq.c1oappe.top

TS:   arr.includes(x)
来源：http://yay.ydzc1.top

Java: list.contains(x)
来源：http://xaz.zycfv.cn

Go:   slices.Contains(arr, x)
来源：http://ujs.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://qtq.mhx1999.top

C#:   list.Contains(x)
来源：http://mzm.jlsjyb.cn

[D22] 复制数组（避免共享引用）
来源：http://lwq.sxryk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pzd.zhixingplan.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qil.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dws.hcnkem.com

TS:   [...arr];
来源：http://xaq.pycfn.com

Java: new ArrayList<>(list);
来源：http://zzn.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gjh.zhixingplan.top

Ruby: arr.dup;  arr.clone
来源：http://ebi.jinghuilouyu.cn

C#:   new List<int>(list);
来源：http://pcz.daxiang520.top

[D23] reduce 累积计算
来源：http://wpe.zhijiandao.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xfk.ybcxt.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://teq.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vwn.hesvh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xss.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bur.bjfxy.top

Go:   // 手写循环
来源：http://bnu.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oka.pengpengdd.cyou


<!-- 参考信息 -->