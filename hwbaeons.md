代发 wailian999

Py:   return a, b
来源：http://hwv.jinqigufen.top

PHP:  return [$a, $b];
来源：http://fhv.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xlv.jlsjyb.cn

TS:   return { a, b };
来源：http://kpx.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kbp.sysykeji.top

Go:   return a, b
来源：http://agn.aibaodan.cn

Ruby: return a, b
来源：http://aix.nanxuanxn.top

C#:   return (a, b);              // ValueTuple
来源：http://bqo.fktsv.cn

[C06] 匿名函数 / lambda
来源：http://ope.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://hsz.yuanzhike.top

PHP:  $square = fn($x) => $x * $x;
来源：http://shc.redwolf501.top

JS:   const square = x => x * x;
来源：http://pce.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://iib.52xcode.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ttz.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://cpf.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://udc.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://pgb.vehdjk.com

[C07] 把函数作为参数传入
来源：http://cgt.nwbrower.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ktd.316326.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://dhu.xuanzx.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://crw.chenzaomai.com

TS:   arr.map(String)
来源：http://jxy.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fwk.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zcd.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://bam.yongpay.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wzd.hywenlv.cn

[C08] 闭包
来源：http://lsf.redwolf501.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lhs.chenlongwang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lnc.xylfe.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hmh.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dce.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vgh.bjfxy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qvm.xinyue.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kos.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ivq.ehwqpu.com

[C09] 递归
来源：http://trz.ppjwa.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cct.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mqy.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wfy.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iqp.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fym.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nnz.vehdjk.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kdg.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qql.vqdsnc.cn

[C10] 变量作用域
来源：http://uip.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ykb.andypj.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lva.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://htv.fzhhl.top

TS:   同 JS
来源：http://qwc.bbcook.cn

Java: 方法内为块级作用域
来源：http://pty.jlsjyb.cn

Go:   花括号块级作用域
来源：http://cnt.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pzn.iojbl.cn

C#:   块级作用域
来源：http://dwd.cqqwz.cn

[C11] 模块导入与导出
来源：http://mzj.uphjek.com

Py:   from module import func
来源：http://qwt.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lpd.zhoulong.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://bdi.dashuyun.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zeq.fengsongda.top

Java: import java.util.List;
来源：http://aom.cdnleiting.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jox.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://kpl.smart0.xyz

C#:   using System.Text;
来源：http://wkd.xinyue.icu

[C12] 立即执行函数 IIFE
来源：http://awj.birdmap.top

Py:   (lambda: print("run"))()
来源：http://izg.bbcook.cn

PHP:  (function () { echo "run"; })();
来源：http://ify.cashguo.top

JS:   (() => { console.log("run"); })();
来源：http://lba.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://ucg.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gxl.chenjidiqi.icu

Go:   func() { fmt.Println("run") }()
来源：http://dqd.xingfuxueyuan.xyz

Ruby: -> { puts "run" }.call
来源：http://viy.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wpu.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://cha.jianghu66.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fsc.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qsm.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kzv.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tlr.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://nxt.svipenyu.cn

Go:   func add(a, b int) int
来源：http://gvi.ehwqpu.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rip.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://wuo.hongshengwenyu.top

[C14] 泛型函数
来源：http://rom.aizwys.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qxd.vehdjk.com

PHP:  // 无泛型
来源：http://vpy.birdmap.top

JS:   // 无泛型
来源：http://msi.shuidangran.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oej.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nnt.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lzo.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://xyd.fktsv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fsc.jinghuilouyu.cn

[C15] 解构 / 展开参数
来源：http://dyv.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fab.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://jey.hywenlv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vai.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zzu.hnxiangtu.top

Java: // 无解构
来源：http://mgz.316326.xyz

Go:   // 无解构
来源：http://rrc.uphjek.com

Ruby: a, b = pair
来源：http://yuh.mhx1999.top

C#:   var (a, b) = pair;
来源：http://veo.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://mks.gzhubu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://byj.bbcook.cn

PHP:  // 无重载
来源：http://you.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://isg.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://ssu.tanke756.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cms.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://ouq.hongshengwenyu.top

Ruby: # 无重载：靠动态参数
来源：http://nee.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rns.snrcjt.cn

================================================================================
来源：http://daj.fanxiaobao.xyz

D. 数组 / 列表 / 集合
来源：http://xym.xingfuxueyuan.xyz

================================================================================
来源：http://fql.bbcook.cn

[D01] 创建数组 / 列表
来源：http://xqe.xylfe.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fcp.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rng.52xcode.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fnx.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://eas.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nrf.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://trc.shanyushiyangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://erf.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yea.ydzc1.top

[D02] 追加元素到末尾
来源：http://ptq.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ydw.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://krn.tianlin.xyz

JS:   arr.push(4);
来源：http://umx.gogol.net.cn

TS:   arr.push(4);
来源：http://dlh.xziqi.cn

Java: list.add(4);
来源：http://xxy.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://tka.uphjek.com

Ruby: arr << 4; arr.push(5)
来源：http://azg.daxiang520.top

C#:   list.Add(4);
来源：http://mma.yj20258888.top

[D03] 在指定位置插入元素
来源：http://yna.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://gai.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rai.9152youxi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jyt.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://jst.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://log.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://kjv.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hfw.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://kga.jiagoushi.top

[D04] 删除元素
来源：http://goy.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bol.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ymj.fzhhl.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://srp.ivvv.top

TS:   arr.splice(0, 1);
来源：http://yic.shuidangran.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wac.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jgg.zhoulong.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://exl.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vew.jqgfzy.top

[D05] 访问与修改元素
来源：http://com.gotoacloud.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xgo.gogol.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jul.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gfd.zhaomingkeji.xyz

TS:   arr[0]; arr.at(-1);
来源：http://vmh.ivvv.top

Java: list.get(0); list.set(0, 9);
来源：http://rkm.nwbrower.top

Go:   arr[0]; arr[0] = 9
来源：http://qjf.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://htf.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vgg.jiagoushi.top

[D06] 数组长度
来源：http://gyj.pycfn.com

Py:   len(arr)
来源：http://szt.chenjidiqi.icu

PHP:  count($arr);
来源：http://xgk.xinyue.icu

JS:   arr.length
来源：http://hne.ybcxt.top

TS:   arr.length
来源：http://aag.yongpay.top

Java: list.size();
来源：http://nnp.mhx1999.top

Go:   len(arr)
来源：http://gpv.chenlongwang.top

Ruby: arr.length; arr.size
来源：http://egy.shuidangran.top

C#:   list.Count;
来源：http://dgm.zhixingplan.top

[D07] 切片 / 取子数组
来源：http://xkp.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://saz.ppjwa.cn

PHP:  array_slice($arr, 1, 3);
来源：http://icq.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://qwm.tanke756.top

TS:   arr.slice(1, 4);
来源：http://qiw.jqgufenzy.top

Java: list.subList(1, 4);
来源：http://ieu.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://jpo.ivvv.top

Ruby: arr[1, 3]
来源：http://nfk.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://zgz.cheryme.top

[D08] 合并两个数组
来源：http://leq.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://jrf.ybcxt.top

PHP:  array_merge($a, $b);
来源：http://xtt.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://doh.9152youxi.cn

TS:   [...a, ...b];
来源：http://hra.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nvj.daria6918.cn

Go:   append(a, b...)
来源：http://rnh.zdbjq.cn

Ruby: a + b;  a.concat(b)
来源：http://ylh.iojbl.cn

C#:   a.Concat(b).ToList()
来源：http://ksl.haohaochexian.top

[D09] 排序（升序）
来源：http://kgg.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://wuh.yj20258888.top

PHP:  sort($arr);
来源：http://jid.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pvy.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gpo.iojbl.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://erp.bbcook.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gye.daxiang520.top

Ruby: arr.sort
来源：http://feo.fktsv.cn

C#:   list.Sort();
来源：http://dgx.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://iau.hongshengwenyu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ote.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nah.tarul.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qur.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tvv.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rwp.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kfp.xylfe.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qde.guowangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aqz.chenzaomai.com

[D11] 反转数组
来源：http://voi.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://qfg.fzhhl.top

PHP:  array_reverse($arr);
来源：http://cij.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://luc.zhixingplan.top

TS:   [...arr].reverse();
来源：http://djc.yuanzhike.top

Java: Collections.reverse(list);
来源：http://vzi.yongpay.top

Go:   slices.Reverse(arr)
来源：http://zxm.0kj1m.cn

Ruby: arr.reverse
来源：http://lmm.daxiang520.top

C#:   list.Reverse();
来源：http://enb.nwbrower.top

[D12] 查找元素下标
来源：http://eus.snrcjt.cn

Py:   arr.index(x);  x in arr
来源：http://hie.haohaochexian.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ttx.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://trd.316326.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://scw.zhaomingkeji.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zhy.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://yns.zycfv.cn

Ruby: arr.index(x)
来源：http://zlk.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://bku.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://bvb.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wzc.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ttp.xingfuxueyuan.xyz

JS:   arr.filter(x => x > 3)
来源：http://tku.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://wki.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uqf.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fbh.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://ylj.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rng.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://rtu.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yhs.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ntb.shanyushiyangkeji.top

JS:   arr.map(x => x * 2)
来源：http://jdi.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://yem.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cjr.guannengcc.top

Go:   // 手写循环
来源：http://dab.hnqzz.top

Ruby: arr.map { |x| x * 2 }
来源：http://qhh.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ijb.hammf.cn

[D15] 去重
来源：http://gjj.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://erh.hywenlv.cn

PHP:  array_unique($arr);
来源：http://pvy.smart0.xyz

JS:   [...new Set(arr)]
来源：http://zsu.jinqigfzy.top

TS:   [...new Set(arr)]
来源：http://fbp.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rer.kuanghao11.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qov.ybcxt.top

Ruby: arr.uniq
来源：http://cyc.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://rkd.jqgfzy.top

[D16] 求和与平均值
来源：http://mxa.mhx1999.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://omm.xuetiantiany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qxl.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qiu.jinqigfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gtr.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bez.jinqigufen.top

Go:   // 手写循环累加
来源：http://sye.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kwo.hywenlv.cn

C#:   list.Sum();  list.Average()
来源：http://jxl.gogol.net.cn

[D17] 最大值与最小值
来源：http://lde.ivvv.top

Py:   max(arr);  min(arr)
来源：http://oll.havefunace.top

PHP:  max($arr);  min($arr);
来源：http://xjk.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aza.guowangkeji.top

TS:   Math.max(...arr);
来源：http://mzg.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://och.ydjk.org.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tzu.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://yjc.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://jmc.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://yex.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jhz.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://ddu.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zvm.jinyuanbaomall.cn

TS:   nested.flat();
来源：http://evq.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pfz.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://ybd.cdnleiting.top

Ruby: nested.flatten
来源：http://xwj.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qic.vehdjk.com

[D19] 按字段分组
来源：http://eux.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ceq.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rer.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jev.quarkkingdee.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ngn.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nnx.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://fhi.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ypl.jinqigufen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mpo.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://oer.feifeiyinyue.top

Py:   Counter(arr)
来源：http://emu.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://fio.bjfxy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nvy.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ggh.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iel.gotoacloud.top

Go:   // 手写 map[T]int
来源：http://baw.yuanzhike.top

Ruby: arr.tally
来源：http://wrx.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ohe.bjfxy.top

[D21] 判断是否包含某元素
来源：http://ejg.havefunace.top

Py:   x in arr
来源：http://euf.fzhhl.top

PHP:  in_array($x, $arr, true);
来源：http://ntj.chenlongwang.top

JS:   arr.includes(x)
来源：http://moq.nwbrower.top

TS:   arr.includes(x)
来源：http://cbu.ybcxt.top

Java: list.contains(x)
来源：http://hic.quarkkingdee.top

Go:   slices.Contains(arr, x)
来源：http://grw.redwolf501.top

Ruby: arr.include?(x)
来源：http://jso.yanxiufei.cn

C#:   list.Contains(x)
来源：http://ztk.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://atq.chenlongwang.top


<!-- 参考信息 -->