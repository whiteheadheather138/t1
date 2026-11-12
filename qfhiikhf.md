代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jfl.shzxlz.cn

Go:   return a, b
来源：http://dvi.daria6918.cn

Ruby: return a, b
来源：http://uwu.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://eaw.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://uui.yj20258888.top

Py:   square = lambda x: x * x
来源：http://ebu.wangshuangyany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xkd.yj202588.top

JS:   const square = x => x * x;
来源：http://mjz.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://ieg.xziqi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rnq.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://ogv.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://rjj.zhijiandao.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zqh.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://cmx.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ccy.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yme.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pcn.snrcjt.cn

TS:   arr.map(String)
来源：http://vbu.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ghh.nwbrower.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ofa.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://vkf.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ltw.yongpay.top

[C08] 闭包
来源：http://qbq.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://try.quarkkingdee.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sna.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tuh.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sfq.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://put.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jfb.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nhw.kuanghao11.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yxh.smart0.xyz

[C09] 递归
来源：http://jmi.epnwcf.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dau.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jdp.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ult.cqqwz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mpv.havefunace.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zbo.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://txl.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ula.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jlm.jinqigfzy.top

[C10] 变量作用域
来源：http://sst.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qym.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iml.0kj1m.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rov.tianlin.xyz

TS:   同 JS
来源：http://brz.sweek.top

Java: 方法内为块级作用域
来源：http://xrb.shanyushiyangkeji.top

Go:   花括号块级作用域
来源：http://sft.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nok.vehdjk.com

C#:   块级作用域
来源：http://ufb.hnxiangtu.top

[C11] 模块导入与导出
来源：http://uhu.havefunace.top

Py:   from module import func
来源：http://emy.316326.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://vov.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://eig.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://quk.haohaochexian.top

Java: import java.util.List;
来源：http://del.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ali.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://jgl.sxryk.cn

C#:   using System.Text;
来源：http://kfc.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://jtf.fanxiaobao.xyz

Py:   (lambda: print("run"))()
来源：http://abs.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://itb.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://rxj.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://hui.yangfankeji.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lna.jinghuilouyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://qjx.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://kfg.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hjh.sxryk.cn

[C13] 类型声明 / 类型注解
来源：http://znf.ywan-chungtsiang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baq.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mmn.xinyue.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ooq.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tqj.yj20258888.top

Java: int add(int a, int b) { return a + b; }
来源：http://qqx.hysaishi.cn

Go:   func add(a, b int) int
来源：http://sqr.zhengqikj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ozg.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://elh.tarul.cn

[C14] 泛型函数
来源：http://gjc.chenlongwang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qcg.cqqwz.cn

PHP:  // 无泛型
来源：http://drd.cashguo.top

JS:   // 无泛型
来源：http://zzv.9152youxi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dkp.havefunace.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://khr.ehwqpu.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qnz.guannengcc.top

Ruby: # 无泛型
来源：http://nog.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wtr.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://kwj.bjfxy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qgq.ybcxt.top

PHP:  [$a, $b] = $pair;
来源：http://qlh.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ppt.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uge.sweek.top

Java: // 无解构
来源：http://jxq.wangshuangyany.cn

Go:   // 无解构
来源：http://umk.fengsongda.top

Ruby: a, b = pair
来源：http://toc.hnqzz.top

C#:   var (a, b) = pair;
来源：http://yqu.fzhhl.top

[C16] 函数 / 方法重载
来源：http://fec.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vjb.nwbrower.top

PHP:  // 无重载
来源：http://hol.nwbrower.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dcy.shuidangran.top

TS:   // 用联合类型或重载签名声明
来源：http://hov.daxiang520.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ucd.epnwcf.com

Go:   // 无重载：用不同函数名
来源：http://zel.sysykeji.top

Ruby: # 无重载：靠动态参数
来源：http://zdy.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wwd.dianchejie.cn

================================================================================
来源：http://gzi.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://rgo.yuxming.cn

================================================================================
来源：http://xuy.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://fyt.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mak.wangshuangyany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://haj.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://man.zhixingplan.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://krx.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ggu.yueranfly.top

Go:   arr := []int{1, 2, 3}
来源：http://gbj.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://cxl.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dco.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://chh.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ohm.cucudq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bqd.chenjidiqi.icu

JS:   arr.push(4);
来源：http://aad.jiagoushi.top

TS:   arr.push(4);
来源：http://tju.fzhhl.top

Java: list.add(4);
来源：http://udu.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://mep.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://tzv.xinyue.icu

C#:   list.Add(4);
来源：http://gto.yuxming.cn

[D03] 在指定位置插入元素
来源：http://znj.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://kmo.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dhb.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dnn.andypj.xyz

TS:   arr.splice(0, 0, 0);
来源：http://guu.hysaishi.cn

Java: list.add(0, 0);
来源：http://snb.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://sot.cheryme.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iri.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://vgt.sxryk.cn

[D04] 删除元素
来源：http://kcf.xuetiantiany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pmg.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jek.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lsm.c1oappe.top

TS:   arr.splice(0, 1);
来源：http://iuf.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ipg.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://phl.chenjidiqi.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://avy.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://whj.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://ltp.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bel.tarul.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sml.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://skq.jianghu66.top

TS:   arr[0]; arr.at(-1);
来源：http://yoo.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://wyi.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://ero.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vgf.sufxvd.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wgx.hnxiangtu.top

[D06] 数组长度
来源：http://ugt.xuanzx.com

Py:   len(arr)
来源：http://yrk.shanyushiyangtech.top

PHP:  count($arr);
来源：http://mkb.shzxlz.cn

JS:   arr.length
来源：http://pad.bjfxy.top

TS:   arr.length
来源：http://kbo.gzhubu.top

Java: list.size();
来源：http://xwm.gzhubu.top

Go:   len(arr)
来源：http://nmt.iojbl.cn

Ruby: arr.length; arr.size
来源：http://dbh.xinyue.icu

C#:   list.Count;
来源：http://mvp.dianchejie.cn

[D07] 切片 / 取子数组
来源：http://efr.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wso.zhongyouzk.top

PHP:  array_slice($arr, 1, 3);
来源：http://uqy.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://diz.sufxvd.cn

TS:   arr.slice(1, 4);
来源：http://rlh.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://lyc.hongshengwenyu.top

Go:   arr[1:4]
来源：http://bcm.ctjpmb.com

Ruby: arr[1, 3]
来源：http://auj.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://tju.ppjwa.cn

[D08] 合并两个数组
来源：http://mia.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://mdq.havefunace.top

PHP:  array_merge($a, $b);
来源：http://loz.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mnx.yonumen.top

TS:   [...a, ...b];
来源：http://fgt.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zev.ywan-chungtsiang.top

Go:   append(a, b...)
来源：http://vkj.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://jth.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://nas.iojbl.cn

[D09] 排序（升序）
来源：http://hon.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://fde.shzxlz.cn

PHP:  sort($arr);
来源：http://wah.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mri.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nvi.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hwt.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://isc.zhijiandao.cn

Ruby: arr.sort
来源：http://yuy.zhijiandao.cn

C#:   list.Sort();
来源：http://idz.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://klj.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ncp.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fge.wangdashe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vow.hfpthk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://roc.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pef.birdmap.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rzl.tian-w.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pgv.gogol.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sdb.bjfxy.top

[D11] 反转数组
来源：http://wxf.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://del.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://plv.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cbn.bjfxy.top

TS:   [...arr].reverse();
来源：http://xpq.0kj1m.cn

Java: Collections.reverse(list);
来源：http://bnx.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://bes.xziqi.cn

Ruby: arr.reverse
来源：http://whp.ydzc1.top

C#:   list.Reverse();
来源：http://qnk.hongshengwenyu.top

[D12] 查找元素下标
来源：http://otp.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://mor.xinyue.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vrd.fengsongda.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zro.316326.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hbf.feifeiyinyue.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ayo.havefunace.top

Go:   slices.Index(arr, x)
来源：http://agv.ydzc1.top

Ruby: arr.index(x)
来源：http://kjd.yfazqb.com

C#:   list.IndexOf(x);
来源：http://iom.zhongyouzk.top

[D13] 过滤（保留满足条件的）
来源：http://spz.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wvv.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rng.zhiwuduotai.top

JS:   arr.filter(x => x > 3)
来源：http://utt.yvedp.cn

TS:   arr.filter(x => x > 3)
来源：http://pgt.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zlj.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nwz.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://srq.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qln.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://cvk.jinqigufen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dyr.0kj1m.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jmi.bbcook.cn

JS:   arr.map(x => x * 2)
来源：http://yij.shanyushiyangtech.top

TS:   arr.map(x => x * 2)
来源：http://ocq.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tsk.svipenyu.cn

Go:   // 手写循环
来源：http://nfc.uphjek.com

Ruby: arr.map { |x| x * 2 }
来源：http://gpv.zhiwuduotai.top

C#:   list.Select(x => x * 2).ToList()
来源：http://aaw.yangfankeji.com

[D15] 去重
来源：http://hiv.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vbw.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://nfy.zhoulong.xyz

JS:   [...new Set(arr)]
来源：http://flp.pengpengdd.cyou

TS:   [...new Set(arr)]
来源：http://fdq.xuanzx.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uyv.guannengcc.top

Go:   // 用 map[T]struct{} 手写
来源：http://tqk.xinyue.icu

Ruby: arr.uniq
来源：http://qmu.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://lfz.zhijiandao.cn

[D16] 求和与平均值
来源：http://qsh.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://exm.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uoi.daxiang520.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xeu.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vry.gaohongyu789.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dqe.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://oxf.daria6918.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ybt.daria6918.cn

C#:   list.Sum();  list.Average()
来源：http://knm.zhengqikj.top

[D17] 最大值与最小值
来源：http://njn.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://myb.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://zmu.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ltd.xuanzx.com

TS:   Math.max(...arr);
来源：http://etj.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vof.yangfankeji.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bqx.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://bta.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://ody.xylfe.cn

[D18] 扁平化嵌套数组
来源：http://jsj.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zje.yangfankeji.com

PHP:  array_merge(...$nested);
来源：http://mbi.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uzr.ivvv.top

TS:   nested.flat();
来源：http://wey.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yef.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://xtg.ehwqpu.com

Ruby: nested.flatten
来源：http://qmf.sufxvd.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hmq.andypj.xyz

[D19] 按字段分组
来源：http://hal.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hsy.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fqr.aibaodan.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ael.svipenyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mjf.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zut.yj20258888.top

Go:   // 手写 map[string][]T
来源：http://yua.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://rbg.cqqwz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qqv.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://apd.tarul.cn

Py:   Counter(arr)
来源：http://rzx.haohaochexian.top

PHP:  array_count_values($arr);
来源：http://miu.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://peb.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://exg.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kzk.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://lpb.snrcjt.cn

Ruby: arr.tally
来源：http://zqy.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uxe.0kj1m.cn

[D21] 判断是否包含某元素
来源：http://vrb.yuxming.cn

Py:   x in arr
来源：http://wew.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://qvv.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://uho.zhijiandao.cn

TS:   arr.includes(x)
来源：http://ooe.aibaodan.cn

Java: list.contains(x)
来源：http://faq.guowangkeji.top

Go:   slices.Contains(arr, x)
来源：http://sfi.guowangkeji.top

Ruby: arr.include?(x)
来源：http://etb.ppjwa.cn

C#:   list.Contains(x)
来源：http://whz.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://cck.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dzv.daxiang520.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dec.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lqx.52xcode.cn

TS:   [...arr];
来源：http://ggv.yangfankeji.com


<!-- 参考信息 -->