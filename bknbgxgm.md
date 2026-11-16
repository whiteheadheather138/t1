代发 wailian999

Py:   return a, b
来源：http://mpb.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://byq.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qla.yanxiufei.cn

TS:   return { a, b };
来源：http://mhn.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fpv.jqgfzy.top

Go:   return a, b
来源：http://jgv.fanxiaobao.xyz

Ruby: return a, b
来源：http://jmt.xinyue.icu

C#:   return (a, b);              // ValueTuple
来源：http://kqz.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://rmk.yj20258.top

Py:   square = lambda x: x * x
来源：http://uxs.andypj.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://cma.gzhubu.top

JS:   const square = x => x * x;
来源：http://wih.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://yhu.shanyushiyangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sls.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://upa.jqgfzy.top

Ruby: square = ->(x) { x * x }
来源：http://ifb.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nrc.yfazqb.com

[C07] 把函数作为参数传入
来源：http://esm.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lnr.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://imm.snrcjt.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gax.xuetiantiany.cn

TS:   arr.map(String)
来源：http://pfo.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cgz.jinghuilouyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mwj.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://haq.shzxlz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fmm.chenlongwang.top

[C08] 闭包
来源：http://bpr.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://abb.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ttp.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sot.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mcm.yuanzhike.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pek.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ojj.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://saa.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ypb.sysykeji.top

[C09] 递归
来源：http://yft.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zql.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zbz.316326.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wpm.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sov.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hyc.jlsjyb.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xwm.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://krk.chenjidiqi.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lyb.daxiang520.top

[C10] 变量作用域
来源：http://ciy.yj20258.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hmz.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ifq.wangdashe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gin.feifeiyinyue.top

TS:   同 JS
来源：http://pfp.ybcxt.top

Java: 方法内为块级作用域
来源：http://xnz.chenjidiqi.icu

Go:   花括号块级作用域
来源：http://awl.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lpz.guannengcc.top

C#:   块级作用域
来源：http://ujb.hcnkem.com

[C11] 模块导入与导出
来源：http://gvw.sufxvd.cn

Py:   from module import func
来源：http://fyv.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wuc.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ajl.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ylr.cashguo.top

Java: import java.util.List;
来源：http://rfd.0kj1m.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vdk.yueranfly.top

Ruby: require "json"; require_relative "./util"
来源：http://vbm.ydjk.org.cn

C#:   using System.Text;
来源：http://ifl.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://jyr.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://int.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://qio.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://itk.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://fzq.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nxs.sjlbkw.cn

Go:   func() { fmt.Println("run") }()
来源：http://kcm.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://hzn.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://drx.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://hrd.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://azf.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ktk.jqgufenzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wof.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bug.guowangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://pzj.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://vce.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nyg.ehwqpu.com

C#:   int Add(int a, int b) => a + b;
来源：http://ggl.hnxiangtu.top

[C14] 泛型函数
来源：http://mrc.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nku.fengsongda.top

PHP:  // 无泛型
来源：http://rre.epnwcf.com

JS:   // 无泛型
来源：http://kms.haohaochexian.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://loe.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vej.yuxming.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gim.redwolf501.top

Ruby: # 无泛型
来源：http://ues.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dsi.meibo888.top

[C15] 解构 / 展开参数
来源：http://xhj.yuanzhike.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mva.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://vch.316326.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zxn.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dou.gaohongyu789.top

Java: // 无解构
来源：http://zjn.gogol.net.cn

Go:   // 无解构
来源：http://vwb.birdmap.top

Ruby: a, b = pair
来源：http://rse.ppjwa.cn

C#:   var (a, b) = pair;
来源：http://zha.daria6918.cn

[C16] 函数 / 方法重载
来源：http://lny.xuetiantiany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jsh.jyoumei.cn

PHP:  // 无重载
来源：http://wzi.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wnc.jinqigufen.top

TS:   // 用联合类型或重载签名声明
来源：http://ucv.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://pru.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://gug.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://bds.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://byn.birdmap.top

================================================================================
来源：http://obu.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://rnn.shanyushiyangkeji.top

================================================================================
来源：http://izv.zdbjq.cn

[D01] 创建数组 / 列表
来源：http://nmk.yonumen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://due.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pyv.chenzaomai.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://aqj.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rkh.shangyingyoupin.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sog.xuanzx.com

Go:   arr := []int{1, 2, 3}
来源：http://egx.nanxuanxn.top

Ruby: arr = [1, 2, 3]
来源：http://tzu.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hvh.wangshuangyany.cn

[D02] 追加元素到末尾
来源：http://gkd.zycfv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zlg.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vzz.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://oyv.birdmap.top

TS:   arr.push(4);
来源：http://qmk.cashguo.top

Java: list.add(4);
来源：http://vxa.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://oid.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://qip.feifeiyinyue.top

C#:   list.Add(4);
来源：http://wwb.hnqzz.top

[D03] 在指定位置插入元素
来源：http://erl.sysykeji.top

Py:   arr.insert(0, 0)
来源：http://yfz.xuanzx.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qzv.jqgufenzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qkj.wangdashe.top

TS:   arr.splice(0, 0, 0);
来源：http://anv.zhongyouzk.top

Java: list.add(0, 0);
来源：http://mnc.hfpthk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xje.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rre.tanke756.top

C#:   list.Insert(0, 0);
来源：http://vnp.jinghuilouyu.cn

[D04] 删除元素
来源：http://vyy.wangshuangyany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sug.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iex.andypj.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mri.yonumen.top

TS:   arr.splice(0, 1);
来源：http://wdj.tanke756.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nof.xuanzx.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sil.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pci.cashguo.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jkl.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://kii.jiagoushi.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xjg.chenlongwang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rcl.c1oappe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hlh.iojbl.cn

TS:   arr[0]; arr.at(-1);
来源：http://lsi.52xcode.cn

Java: list.get(0); list.set(0, 9);
来源：http://evn.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://owb.andypj.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lap.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://npz.smart0.xyz

[D06] 数组长度
来源：http://xpg.iojbl.cn

Py:   len(arr)
来源：http://mwe.shanyushiyangkeji.top

PHP:  count($arr);
来源：http://tly.ivvv.top

JS:   arr.length
来源：http://esn.hysaishi.cn

TS:   arr.length
来源：http://uvv.cucudq.cn

Java: list.size();
来源：http://ugz.daria6918.cn

Go:   len(arr)
来源：http://sdr.smart0.xyz

Ruby: arr.length; arr.size
来源：http://mrj.cashguo.top

C#:   list.Count;
来源：http://ybf.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://hcz.xylfe.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ynm.gzhubu.top

PHP:  array_slice($arr, 1, 3);
来源：http://kce.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://knl.pengpengdd.cyou

TS:   arr.slice(1, 4);
来源：http://vmy.chenzaomai.com

Java: list.subList(1, 4);
来源：http://wjl.zhoulong.xyz

Go:   arr[1:4]
来源：http://mpv.0kj1m.cn

Ruby: arr[1, 3]
来源：http://xsd.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://ksu.vehdjk.com

[D08] 合并两个数组
来源：http://wng.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://hbe.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://oga.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://syn.fengsongda.top

TS:   [...a, ...b];
来源：http://wqw.ydjk.org.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aqe.yj20258888.top

Go:   append(a, b...)
来源：http://mlj.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://rar.52xcode.cn

C#:   a.Concat(b).ToList()
来源：http://roe.nwbrower.top

[D09] 排序（升序）
来源：http://qhh.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://zce.tarul.cn

PHP:  sort($arr);
来源：http://qxo.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://syj.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rye.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xpu.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nyb.chenlongwang.top

Ruby: arr.sort
来源：http://idk.xinyue.icu

C#:   list.Sort();
来源：http://qwb.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ohq.yj202588.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oak.yfazqb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://smi.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://crc.zhongyouzk.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uej.daxiang520.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jsn.xinyue.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iye.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tyc.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eaf.yuanzhike.top

[D11] 反转数组
来源：http://dxp.hfpthk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://aik.pengpengdd.cyou

PHP:  array_reverse($arr);
来源：http://adz.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kow.jianghu66.top

TS:   [...arr].reverse();
来源：http://bjd.yj20258.top

Java: Collections.reverse(list);
来源：http://pax.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://zzb.jlsjyb.cn

Ruby: arr.reverse
来源：http://lon.snrcjt.cn

C#:   list.Reverse();
来源：http://jmq.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://bzg.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://zeg.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yad.jyoumei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pmi.hammf.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lgv.ywan-chungtsiang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oqw.guannengcc.top

Go:   slices.Index(arr, x)
来源：http://nse.nanxinkj.top

Ruby: arr.index(x)
来源：http://xyg.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://vrz.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://pxq.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wql.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://chp.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://ghj.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://dgh.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://giv.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hve.xuetiantiany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ofz.zhengqikj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lys.fktsv.cn

[D14] 映射转换（每个元素变形）
来源：http://ssg.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vzn.cucudq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://azu.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://wje.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://jtk.yongpay.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vbm.hongshengwenyu.top

Go:   // 手写循环
来源：http://jcz.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bwj.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wpe.0kj1m.cn

[D15] 去重
来源：http://efz.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://idj.9152youxi.cn

PHP:  array_unique($arr);
来源：http://bjh.fzhhl.top

JS:   [...new Set(arr)]
来源：http://dql.wangdashe.top

TS:   [...new Set(arr)]
来源：http://fnt.kuanghao11.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ckx.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://nbo.sysykeji.top

Ruby: arr.uniq
来源：http://itd.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://ymp.smart0.xyz

[D16] 求和与平均值
来源：http://zul.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kov.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wjx.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mvj.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vwl.mhx1999.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aox.sxryk.cn

Go:   // 手写循环累加
来源：http://pko.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mzy.9152youxi.cn

C#:   list.Sum();  list.Average()
来源：http://ifa.cashguo.top

[D17] 最大值与最小值
来源：http://dvy.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://sot.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://uiu.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://msg.zdbjq.cn

TS:   Math.max(...arr);
来源：http://gcd.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ydl.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fdd.redwolf501.top

Ruby: arr.max;  arr.min
来源：http://kpr.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://igm.hywenlv.cn

[D18] 扁平化嵌套数组
来源：http://fhk.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nno.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://ubn.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ram.fehbvm.com

TS:   nested.flat();
来源：http://lfa.c1oappe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ezt.hfpthk.cn

Go:   // 手写双层循环
来源：http://ngr.zhiwuduotai.top

Ruby: nested.flatten
来源：http://rvh.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bzq.hywenlv.cn

[D19] 按字段分组
来源：http://qtg.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gcy.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yqe.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vxp.cdnleiting.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pqr.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aez.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://zsq.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rfq.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kye.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://haa.shzxlz.cn

Py:   Counter(arr)
来源：http://bdt.meibo888.top

PHP:  array_count_values($arr);
来源：http://jsj.jyoumei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fru.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ytu.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rqu.tian-w.cn

Go:   // 手写 map[T]int
来源：http://hct.52xcode.cn

Ruby: arr.tally
来源：http://pgk.shanyushiyangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wcu.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://tep.xylfe.cn

Py:   x in arr
来源：http://yzm.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://vej.ehwqpu.com

JS:   arr.includes(x)
来源：http://rxb.cdnleiting.top

TS:   arr.includes(x)
来源：http://rwl.daxiang520.top

Java: list.contains(x)
来源：http://aes.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://tki.ppjwa.cn

Ruby: arr.include?(x)
来源：http://kyb.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://sjd.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://tbo.cdnleiting.top


<!-- 参考信息 -->