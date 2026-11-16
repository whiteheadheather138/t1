代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://vpi.quarkkingdee.top

Ruby: f(a: 1, b: 2)
来源：http://vbc.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://wtw.jinqigfzy.top

[C05] 返回多个值
来源：http://abz.ctjpmb.com

Py:   return a, b
来源：http://mjn.ivvv.top

PHP:  return [$a, $b];
来源：http://jzo.chenjidiqi.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://skr.daria6918.cn

TS:   return { a, b };
来源：http://evr.gogol.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eie.aibaodan.cn

Go:   return a, b
来源：http://xev.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://fkr.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://cal.yonumen.top

[C06] 匿名函数 / lambda
来源：http://lsh.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://xej.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jqu.fanxiaobao.xyz

JS:   const square = x => x * x;
来源：http://vnt.jianghu66.top

TS:   const square = (x: number): number => x * x;
来源：http://xev.kuanghao11.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://elq.bbcook.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zsa.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://kya.aibaodan.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dvj.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://jdi.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://htn.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://ppb.jlsjyb.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://czh.pengpengdd.cyou

TS:   arr.map(String)
来源：http://zjt.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gnu.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://beq.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://pzv.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xak.yj202588.top

[C08] 闭包
来源：http://ivz.aizwys.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fkl.ivvv.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nrg.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yva.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dus.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qyg.pengpengdd.cyou

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yey.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mnb.iojbl.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hcf.xziqi.cn

[C09] 递归
来源：http://fpe.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jpz.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zec.dianchejie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ixr.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ixy.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bbe.xylfe.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://avd.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://auv.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gvt.yj202588.top

[C10] 变量作用域
来源：http://fok.ydjk.org.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://btn.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://awv.tanke756.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mdj.hfpthk.cn

TS:   同 JS
来源：http://uta.chenlongwang.top

Java: 方法内为块级作用域
来源：http://cmu.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://hyb.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bwe.redwolf501.top

C#:   块级作用域
来源：http://xbl.ybcxt.top

[C11] 模块导入与导出
来源：http://fik.ydzc1.top

Py:   from module import func
来源：http://doc.xziqi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xys.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ikk.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://thg.nanxinkj.top

Java: import java.util.List;
来源：http://rmy.ybcxt.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dko.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://fpa.vehdjk.com

C#:   using System.Text;
来源：http://tnn.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://obd.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://wth.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://rhl.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://hvl.bjfxy.top

TS:   (() => { console.log("run"); })();
来源：http://ujs.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kkj.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://cau.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://kdi.yfazqb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ttw.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://uqe.birdmap.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rbp.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hna.zhongyouzk.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dmv.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zmy.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wam.epnwcf.com

Go:   func add(a, b int) int
来源：http://xyt.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://azk.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://uiw.svipenyu.cn

[C14] 泛型函数
来源：http://pkb.52xcode.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qad.quarkkingdee.top

PHP:  // 无泛型
来源：http://yuj.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://phz.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zwh.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uwu.snrcjt.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://omg.jianghu66.top

Ruby: # 无泛型
来源：http://qzn.hfpthk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xdr.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://qyh.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wek.sysykeji.top

PHP:  [$a, $b] = $pair;
来源：http://sok.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cim.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xsj.jianghu66.top

Java: // 无解构
来源：http://svu.tarul.cn

Go:   // 无解构
来源：http://tiv.jlsjyb.cn

Ruby: a, b = pair
来源：http://xch.xinyue.icu

C#:   var (a, b) = pair;
来源：http://frs.sysykeji.top

[C16] 函数 / 方法重载
来源：http://wsg.sufxvd.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://upj.jqgufenzy.top

PHP:  // 无重载
来源：http://ccm.yvedp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zru.mhx1999.top

TS:   // 用联合类型或重载签名声明
来源：http://kuz.sufxvd.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dtg.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://njb.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://sxb.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zid.shanyushiyangtech.top

================================================================================
来源：http://aza.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://hvd.xuanzx.com

================================================================================
来源：http://dip.jinqigfzy.top

[D01] 创建数组 / 列表
来源：http://trl.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://iwy.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zqt.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yyg.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lut.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ztf.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://vly.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://fvi.jlsjyb.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nxx.9152youxi.cn

[D02] 追加元素到末尾
来源：http://abm.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lud.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yyz.guowangkeji.top

JS:   arr.push(4);
来源：http://qum.yuxming.cn

TS:   arr.push(4);
来源：http://use.sweek.top

Java: list.add(4);
来源：http://tbz.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://fza.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://zde.sjlbkw.cn

C#:   list.Add(4);
来源：http://fhf.pycfn.com

[D03] 在指定位置插入元素
来源：http://efx.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://fcw.sysykeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://psh.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wyt.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://xsk.zhongyouzk.top

Java: list.add(0, 0);
来源：http://ckn.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://wsl.wangshuangyany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ewq.ywan-chungtsiang.top

C#:   list.Insert(0, 0);
来源：http://mfb.xinyue.icu

[D04] 删除元素
来源：http://sbw.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vsz.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oxz.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nxn.meibo888.top

TS:   arr.splice(0, 1);
来源：http://hha.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nno.vqdsnc.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nqy.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gfd.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cgc.ivvv.top

[D05] 访问与修改元素
来源：http://ttx.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aoc.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ogw.gogol.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eko.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://luv.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://mxs.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://xpu.kuanghao11.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ymc.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sdl.zhijiandao.cn

[D06] 数组长度
来源：http://vpz.iojbl.cn

Py:   len(arr)
来源：http://mrf.daria6918.cn

PHP:  count($arr);
来源：http://tep.hywenlv.cn

JS:   arr.length
来源：http://arl.sxryk.cn

TS:   arr.length
来源：http://xho.jiagoushi.top

Java: list.size();
来源：http://qiv.redwolf501.top

Go:   len(arr)
来源：http://ghl.hnqzz.top

Ruby: arr.length; arr.size
来源：http://wkh.jiagoushi.top

C#:   list.Count;
来源：http://wna.daria6918.cn

[D07] 切片 / 取子数组
来源：http://olj.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rvh.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tmc.svipenyu.cn

JS:   arr.slice(1, 4);
来源：http://qzi.feifeiyinyue.top

TS:   arr.slice(1, 4);
来源：http://vdh.zycfv.cn

Java: list.subList(1, 4);
来源：http://zhk.shzxlz.cn

Go:   arr[1:4]
来源：http://iov.dianchejie.cn

Ruby: arr[1, 3]
来源：http://rlv.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://xqb.fehbvm.com

[D08] 合并两个数组
来源：http://xoe.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://pbf.uphjek.com

PHP:  array_merge($a, $b);
来源：http://bnp.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eiv.snrcjt.cn

TS:   [...a, ...b];
来源：http://lrq.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kuw.haohaochexian.top

Go:   append(a, b...)
来源：http://cau.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://gvr.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://ltx.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://oxo.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://tpt.jinqigfzy.top

PHP:  sort($arr);
来源：http://brn.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vmw.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://way.xingfuxueyuan.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://zvr.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rkx.xylfe.cn

Ruby: arr.sort
来源：http://yek.ppjwa.cn

C#:   list.Sort();
来源：http://zgs.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vyn.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iwq.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ouv.daxiang520.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://apn.hammf.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jni.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pwy.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ekq.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wbk.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://izu.feifeiyinyue.top

[D11] 反转数组
来源：http://bwt.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iyt.yangfankeji.com

PHP:  array_reverse($arr);
来源：http://lve.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hxt.yonumen.top

TS:   [...arr].reverse();
来源：http://tei.guowangkeji.top

Java: Collections.reverse(list);
来源：http://xbj.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://dfx.yangfankeji.com

Ruby: arr.reverse
来源：http://izn.shzxlz.cn

C#:   list.Reverse();
来源：http://mlj.0kj1m.cn

[D12] 查找元素下标
来源：http://jql.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://yzg.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dec.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ykk.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pir.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://chd.9152youxi.cn

Go:   slices.Index(arr, x)
来源：http://dcr.hcnkem.com

Ruby: arr.index(x)
来源：http://yrh.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://khd.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://fku.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qqg.ctjpmb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://chi.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://ggu.yueranfly.top

TS:   arr.filter(x => x > 3)
来源：http://qtv.daria6918.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ocx.tanke756.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://okk.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://ntm.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fpw.jyoumei.cn

[D14] 映射转换（每个元素变形）
来源：http://zsx.fehbvm.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lsc.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ydu.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://ony.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://nny.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bzd.yueranfly.top

Go:   // 手写循环
来源：http://qje.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://toh.xziqi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cqf.wangdashe.top

[D15] 去重
来源：http://vpn.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ycn.yonumen.top

PHP:  array_unique($arr);
来源：http://kzn.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://lkv.mhx1999.top

TS:   [...new Set(arr)]
来源：http://syr.hnxiangtu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uyz.gaohongyu789.top

Go:   // 用 map[T]struct{} 手写
来源：http://snu.wangdashe.top

Ruby: arr.uniq
来源：http://vgx.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://wwh.cucudq.cn

[D16] 求和与平均值
来源：http://tgf.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nph.hesvh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dyc.sweek.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://keh.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gzk.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ybi.cashguo.top

Go:   // 手写循环累加
来源：http://xak.vqdsnc.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yhh.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://pib.daria6918.cn

[D17] 最大值与最小值
来源：http://tgk.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://sxl.iojbl.cn

PHP:  max($arr);  min($arr);
来源：http://awf.xuetiantiany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zdf.shuidangran.top

TS:   Math.max(...arr);
来源：http://yhn.hnxiangtu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zvq.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rjz.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://wtm.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://egj.shanyushiyangtech.top

[D18] 扁平化嵌套数组
来源：http://khy.sjlbkw.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rsn.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://cmu.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dgb.ctjpmb.com

TS:   nested.flat();
来源：http://dsf.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hwr.gaohongyu789.top

Go:   // 手写双层循环
来源：http://kdu.yueranfly.top

Ruby: nested.flatten
来源：http://jvl.hammf.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zgr.jianghu66.top

[D19] 按字段分组
来源：http://wdw.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bqb.yj20258888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ezo.9152youxi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eol.xingfuxueyuan.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://bio.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fbn.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://ycb.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ylh.ydzc1.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://waj.yj202588.top

[D20] 统计每个元素出现次数
来源：http://mwj.jinqigfzy.top

Py:   Counter(arr)
来源：http://ovj.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://cfz.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://avc.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fwv.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qps.svipenyu.cn

Go:   // 手写 map[T]int
来源：http://sbz.cdnleiting.top

Ruby: arr.tally
来源：http://qun.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zsf.vehdjk.com

[D21] 判断是否包含某元素
来源：http://jbr.mhx1999.top

Py:   x in arr
来源：http://brs.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://mcz.wangshuangyany.cn

JS:   arr.includes(x)
来源：http://jpo.xuetiantiany.cn

TS:   arr.includes(x)
来源：http://bfm.bjfxy.top

Java: list.contains(x)
来源：http://mxf.cdnleiting.top


<!-- 参考信息 -->