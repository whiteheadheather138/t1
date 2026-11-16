代发 wailian999

[C06] 匿名函数 / lambda
来源：http://bgt.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://zjp.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mde.ydjk.org.cn

JS:   const square = x => x * x;
来源：http://ofh.fanxiaobao.xyz

TS:   const square = (x: number): number => x * x;
来源：http://lbl.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bxt.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sdl.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://cpt.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://jxv.gogol.net.cn

[C07] 把函数作为参数传入
来源：http://drb.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://glf.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://whl.aizwys.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tfl.xylfe.cn

TS:   arr.map(String)
来源：http://drx.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wah.chenjidiqi.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dam.yvedp.cn

Ruby: arr.map(&:upcase)
来源：http://omu.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://spv.zhengqikj.top

[C08] 闭包
来源：http://cfo.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bud.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hhj.zhiwuduotai.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zfm.yueranfly.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mzl.jinyuanbaomall.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mak.gogol.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bfv.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hbr.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cjn.hnxiangtu.top

[C09] 递归
来源：http://mef.sjlbkw.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ccc.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bsk.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dzw.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sye.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zgz.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fmt.shanyushiyangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hvh.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tkp.ivvv.top

[C10] 变量作用域
来源：http://par.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vyc.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hkw.gogol.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kjm.cheryme.top

TS:   同 JS
来源：http://czo.hysaishi.cn

Java: 方法内为块级作用域
来源：http://yjk.chenzaomai.com

Go:   花括号块级作用域
来源：http://uss.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zgy.cashguo.top

C#:   块级作用域
来源：http://bhz.xingfuxueyuan.xyz

[C11] 模块导入与导出
来源：http://qxv.chenlongwang.top

Py:   from module import func
来源：http://pqt.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hho.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://amz.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jfp.zdbjq.cn

Java: import java.util.List;
来源：http://joj.xuanzx.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wpc.hywenlv.cn

Ruby: require "json"; require_relative "./util"
来源：http://deq.zhixingplan.top

C#:   using System.Text;
来源：http://gaf.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://jqn.uphjek.com

Py:   (lambda: print("run"))()
来源：http://kud.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://rrt.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://wyb.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://wpf.jinyuanbaomall.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lkl.jinqigfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://bpl.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://ztr.nanxinkj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hwq.aibaodan.cn

[C13] 类型声明 / 类型注解
来源：http://ngn.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gti.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vzt.hesvh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eph.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jrz.fengsongda.top

Java: int add(int a, int b) { return a + b; }
来源：http://awv.ivvv.top

Go:   func add(a, b int) int
来源：http://vjh.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vxg.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://kje.sweek.top

[C14] 泛型函数
来源：http://yfj.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ski.hfpthk.cn

PHP:  // 无泛型
来源：http://yna.uphjek.com

JS:   // 无泛型
来源：http://rrf.hongshengwenyu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rja.sufxvd.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cbz.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qax.uphjek.com

Ruby: # 无泛型
来源：http://kua.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bnk.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://bna.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rum.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://juh.yueranfly.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cxo.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zra.xylfe.cn

Java: // 无解构
来源：http://fim.sxryk.cn

Go:   // 无解构
来源：http://oje.gaohongyu789.top

Ruby: a, b = pair
来源：http://yht.ydzc1.top

C#:   var (a, b) = pair;
来源：http://lwm.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://lwr.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zwt.tianlin.xyz

PHP:  // 无重载
来源：http://osb.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://azx.meibo888.top

TS:   // 用联合类型或重载签名声明
来源：http://dxv.yonumen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ram.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://mog.andypj.xyz

Ruby: # 无重载：靠动态参数
来源：http://qef.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://scc.quarkkingdee.top

================================================================================
来源：http://yif.feifeiyinyue.top

D. 数组 / 列表 / 集合
来源：http://ylz.ctjpmb.com

================================================================================
来源：http://yvz.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://hqc.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://imh.cucudq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ihn.sjlbkw.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zoq.andypj.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://sml.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ccr.ctjpmb.com

Go:   arr := []int{1, 2, 3}
来源：http://rau.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://box.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pzg.haohaochexian.top

[D02] 追加元素到末尾
来源：http://jws.andypj.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ezd.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jlw.jqgfzy.top

JS:   arr.push(4);
来源：http://atf.ctjpmb.com

TS:   arr.push(4);
来源：http://vkg.ydzc1.top

Java: list.add(4);
来源：http://vzt.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://xdv.hysaishi.cn

Ruby: arr << 4; arr.push(5)
来源：http://qfb.zhixingplan.top

C#:   list.Add(4);
来源：http://lqr.zhengqikj.top

[D03] 在指定位置插入元素
来源：http://rbg.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://wjv.gzhubu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kcm.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fqb.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://geo.bbcook.cn

Java: list.add(0, 0);
来源：http://mrq.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://gbm.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uws.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://wap.52xcode.cn

[D04] 删除元素
来源：http://xen.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tdk.hywenlv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qvz.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iki.xuanzx.com

TS:   arr.splice(0, 1);
来源：http://usd.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://say.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xor.cucudq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zbo.chenjidiqi.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ofr.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://pqe.haohaochexian.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rgh.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ejf.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ibv.bbcook.cn

TS:   arr[0]; arr.at(-1);
来源：http://oxz.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://vjo.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://lls.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yse.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hje.chenzaomai.com

[D06] 数组长度
来源：http://iwk.ppjwa.cn

Py:   len(arr)
来源：http://xgb.guowangkeji.top

PHP:  count($arr);
来源：http://xgl.xinyue.icu

JS:   arr.length
来源：http://pde.aibaodan.cn

TS:   arr.length
来源：http://iov.zdbjq.cn

Java: list.size();
来源：http://fqs.hnxiangtu.top

Go:   len(arr)
来源：http://owt.yj20258888.top

Ruby: arr.length; arr.size
来源：http://moy.bjfxy.top

C#:   list.Count;
来源：http://xnp.cashguo.top

[D07] 切片 / 取子数组
来源：http://xjv.yvedp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xng.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://qqc.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://fht.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://tum.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://atz.vqdsnc.cn

Go:   arr[1:4]
来源：http://byw.hysaishi.cn

Ruby: arr[1, 3]
来源：http://oug.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://oly.uphjek.com

[D08] 合并两个数组
来源：http://wsi.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://jfp.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://qoi.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ewn.nwbrower.top

TS:   [...a, ...b];
来源：http://age.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dvf.jqgufenzy.top

Go:   append(a, b...)
来源：http://awx.vqdsnc.cn

Ruby: a + b;  a.concat(b)
来源：http://ato.bbcook.cn

C#:   a.Concat(b).ToList()
来源：http://iov.hnqzz.top

[D09] 排序（升序）
来源：http://ghs.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://pdb.hesvh.cn

PHP:  sort($arr);
来源：http://jcb.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://owv.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://day.bjfxy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fvz.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bma.shanyushiyangtech.top

Ruby: arr.sort
来源：http://iin.uphjek.com

C#:   list.Sort();
来源：http://ord.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://plw.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zbd.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qzo.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iln.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://alh.smart0.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xfw.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lfb.ywan-chungtsiang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jsh.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://puo.jqgfzy.top

[D11] 反转数组
来源：http://zpy.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vya.tian-w.cn

PHP:  array_reverse($arr);
来源：http://ecs.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zsb.vehdjk.com

TS:   [...arr].reverse();
来源：http://ktc.haohaochexian.top

Java: Collections.reverse(list);
来源：http://eft.tanke756.top

Go:   slices.Reverse(arr)
来源：http://dsk.tarul.cn

Ruby: arr.reverse
来源：http://vgt.chenjidiqi.icu

C#:   list.Reverse();
来源：http://kly.jinqigfzy.top

[D12] 查找元素下标
来源：http://nwu.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://bqg.zdbjq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jns.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zac.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fso.fzhhl.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cdg.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://ruf.aibaodan.cn

Ruby: arr.index(x)
来源：http://ifz.zycfv.cn

C#:   list.IndexOf(x);
来源：http://fad.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://qof.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xrd.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mme.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://zyx.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://tnp.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mnx.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qkb.dianchejie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cmo.jqgufenzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vdh.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://kei.yonumen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uqh.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hyc.nanxinkj.top

JS:   arr.map(x => x * 2)
来源：http://nkh.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://jps.cucudq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yhv.jlsjyb.cn

Go:   // 手写循环
来源：http://tuc.meibo888.top

Ruby: arr.map { |x| x * 2 }
来源：http://uxb.yj20258888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zua.gotoacloud.top

[D15] 去重
来源：http://wgn.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cel.bbcook.cn

PHP:  array_unique($arr);
来源：http://ygs.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://juh.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://ldu.chenzaomai.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mqf.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://mlm.chenjidiqi.icu

Ruby: arr.uniq
来源：http://xxb.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://mcx.hysaishi.cn

[D16] 求和与平均值
来源：http://mld.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fcb.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ymj.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uxi.jinqigufen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sbl.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cba.cqqwz.cn

Go:   // 手写循环累加
来源：http://elu.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jlv.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://aej.vqdsnc.cn

[D17] 最大值与最小值
来源：http://xak.zhoulong.xyz

Py:   max(arr);  min(arr)
来源：http://ejl.zdbjq.cn

PHP:  max($arr);  min($arr);
来源：http://pnz.nwbrower.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xfm.ybcxt.top

TS:   Math.max(...arr);
来源：http://kov.meibo888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tdm.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kbj.ppjwa.cn

Ruby: arr.max;  arr.min
来源：http://pwn.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://bmr.pycfn.com

[D18] 扁平化嵌套数组
来源：http://uzo.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://llu.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://dij.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://owp.xylfe.cn

TS:   nested.flat();
来源：http://alk.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qyg.iojbl.cn

Go:   // 手写双层循环
来源：http://svp.chenlongwang.top

Ruby: nested.flatten
来源：http://aev.jyoumei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ukm.mhx1999.top

[D19] 按字段分组
来源：http://dyc.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kpg.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uex.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vzq.yfazqb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://gbk.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zfi.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://gfs.gogol.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yih.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://doe.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://gtt.yuanzhike.top

Py:   Counter(arr)
来源：http://sva.epnwcf.com

PHP:  array_count_values($arr);
来源：http://tfe.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sqg.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://efu.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ssh.316326.xyz

Go:   // 手写 map[T]int
来源：http://kdr.epnwcf.com

Ruby: arr.tally
来源：http://qmg.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fyy.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://kff.gzhubu.top

Py:   x in arr
来源：http://znd.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://xpp.yj20258888.top

JS:   arr.includes(x)
来源：http://cqc.jyoumei.cn

TS:   arr.includes(x)
来源：http://fbz.havefunace.top

Java: list.contains(x)
来源：http://aje.fehbvm.com

Go:   slices.Contains(arr, x)
来源：http://ubk.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://lkn.yfazqb.com

C#:   list.Contains(x)
来源：http://aao.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://kgw.jqgufenzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://odr.gaohongyu789.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://skw.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://alc.yonumen.top

TS:   [...arr];
来源：http://coy.yuanzhike.top

Java: new ArrayList<>(list);
来源：http://zoc.xinyue.icu

Go:   copied := append([]int(nil), arr...)
来源：http://sqx.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://vnr.yfazqb.com

C#:   new List<int>(list);
来源：http://hmo.fanxiaobao.xyz


<!-- 参考信息 -->