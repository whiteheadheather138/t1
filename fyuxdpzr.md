代发 wailian999

[C06] 匿名函数 / lambda
来源：http://lbz.ctjpmb.com

Py:   square = lambda x: x * x
来源：http://nrk.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://prh.yongpay.top

JS:   const square = x => x * x;
来源：http://opc.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://wcj.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zmx.tanke756.top

Go:   sq := func(x int) int { return x * x }
来源：http://hkr.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://vum.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://ojd.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://gdm.bjfxy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tzi.yfazqb.com

PHP:  array_map("strtoupper", $arr);
来源：http://was.bjfxy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://drl.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://sgf.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://abz.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fsi.aibaodan.cn

Ruby: arr.map(&:upcase)
来源：http://abf.aizwys.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lor.sxryk.cn

[C08] 闭包
来源：http://hoz.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qjp.shangyingyoupin.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://buf.hnqzz.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pla.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ope.aizwys.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ygw.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ewh.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nez.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hkj.fanxiaobao.xyz

[C09] 递归
来源：http://gjy.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://igs.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tjm.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pla.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qcl.zdqjudy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vro.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jph.birdmap.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pqp.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nax.hnxiangtu.top

[C10] 变量作用域
来源：http://xwd.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wyk.fzhhl.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nmw.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xyu.guannengcc.top

TS:   同 JS
来源：http://mjt.hesvh.cn

Java: 方法内为块级作用域
来源：http://nou.jinqigufen.top

Go:   花括号块级作用域
来源：http://nem.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jzv.shuidangran.top

C#:   块级作用域
来源：http://duc.xinyue.icu

[C11] 模块导入与导出
来源：http://pgs.daxiang520.top

Py:   from module import func
来源：http://wyt.kuanghao11.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ckg.havefunace.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kyj.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://czm.kuanghao11.cn

Java: import java.util.List;
来源：http://mhj.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hmz.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://paz.smart0.xyz

C#:   using System.Text;
来源：http://wlf.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://fyv.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://fpx.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://lbs.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://pyr.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://hkz.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hqj.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://zzp.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://tbo.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xge.yongpay.top

[C13] 类型声明 / 类型注解
来源：http://fdj.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ojm.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://opq.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://koh.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mgf.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://ytg.sxryk.cn

Go:   func add(a, b int) int
来源：http://lnr.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://otv.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://buu.dashuyun.cn

[C14] 泛型函数
来源：http://tfg.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tnv.yfazqb.com

PHP:  // 无泛型
来源：http://bpl.nanxinkj.top

JS:   // 无泛型
来源：http://vqa.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sqh.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ojx.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://agz.sweek.top

Ruby: # 无泛型
来源：http://ied.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ylc.fzhhl.top

[C15] 解构 / 展开参数
来源：http://twt.yj20258.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ayo.shanyushiyangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://rzt.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wsb.ydjk.org.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qjj.zhengqikj.top

Java: // 无解构
来源：http://hzl.shangyingyoupin.top

Go:   // 无解构
来源：http://fvf.chenzaomai.com

Ruby: a, b = pair
来源：http://czk.fzhhl.top

C#:   var (a, b) = pair;
来源：http://mwq.aibaodan.cn

[C16] 函数 / 方法重载
来源：http://lra.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oag.zhongyouzk.top

PHP:  // 无重载
来源：http://vwq.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oyk.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://jhy.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://hky.sysykeji.top

Go:   // 无重载：用不同函数名
来源：http://tii.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://ojh.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://xxc.birdmap.top

================================================================================
来源：http://aen.smart0.xyz

D. 数组 / 列表 / 集合
来源：http://caj.feifeiyinyue.top

================================================================================
来源：http://gkf.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://cfb.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xvv.yj20258.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pja.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pki.ydjk.org.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oyi.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dbl.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://dyv.hnqzz.top

Ruby: arr = [1, 2, 3]
来源：http://yyl.fanxiaobao.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rvs.snrcjt.cn

[D02] 追加元素到末尾
来源：http://qde.vqdsnc.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://skz.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jfu.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://mdy.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://fxz.havefunace.top

Java: list.add(4);
来源：http://pjm.hongshengwenyu.top

Go:   arr = append(arr, 4)
来源：http://lkp.zdbjq.cn

Ruby: arr << 4; arr.push(5)
来源：http://vdj.9152youxi.cn

C#:   list.Add(4);
来源：http://zcu.zdqjudy.top

[D03] 在指定位置插入元素
来源：http://fll.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://zim.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bcd.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zzb.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://lnn.gotoacloud.top

Java: list.add(0, 0);
来源：http://wat.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://nxm.hfpthk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bpf.zhongyouzk.top

C#:   list.Insert(0, 0);
来源：http://xft.kuanghao11.cn

[D04] 删除元素
来源：http://jas.daxiang520.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wkw.zycfv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hdr.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eym.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://koh.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uyn.fktsv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xjd.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pgj.cashguo.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ain.zdqjudy.top

[D05] 访问与修改元素
来源：http://nmi.tarul.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://joz.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://soh.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cuh.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://tjk.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://aev.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://vml.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gaq.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nug.nanxinkj.top

[D06] 数组长度
来源：http://zrf.aibaodan.cn

Py:   len(arr)
来源：http://doa.chenlongwang.top

PHP:  count($arr);
来源：http://cmj.ehwqpu.com

JS:   arr.length
来源：http://xfa.jinqigfzy.top

TS:   arr.length
来源：http://fkl.iojbl.cn

Java: list.size();
来源：http://ezn.ppjwa.cn

Go:   len(arr)
来源：http://aec.cashguo.top

Ruby: arr.length; arr.size
来源：http://moh.birdmap.top

C#:   list.Count;
来源：http://uwe.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://dwc.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uxd.kuanghao11.cn

PHP:  array_slice($arr, 1, 3);
来源：http://idm.yongpay.top

JS:   arr.slice(1, 4);
来源：http://btn.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://pui.xinyue.icu

Java: list.subList(1, 4);
来源：http://mta.cdnleiting.top

Go:   arr[1:4]
来源：http://gom.zdbjq.cn

Ruby: arr[1, 3]
来源：http://ntr.sjlbkw.cn

C#:   list.GetRange(1, 3);
来源：http://mll.nanxuanxn.top

[D08] 合并两个数组
来源：http://ddg.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://udq.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://uor.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fgb.svipenyu.cn

TS:   [...a, ...b];
来源：http://cug.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wop.xylfe.cn

Go:   append(a, b...)
来源：http://rex.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://rnm.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://wxd.zhijiandao.cn

[D09] 排序（升序）
来源：http://ulv.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://ayb.fehbvm.com

PHP:  sort($arr);
来源：http://ydz.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kbp.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ltf.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://oos.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dlz.dianchejie.cn

Ruby: arr.sort
来源：http://jmi.andypj.xyz

C#:   list.Sort();
来源：http://wuq.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mdh.ehwqpu.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://trq.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mnn.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://skp.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kex.kuanghao11.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dwq.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wmq.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wov.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cmt.andypj.xyz

[D11] 反转数组
来源：http://lmq.pycfn.com

Py:   arr[::-1];  arr.reverse()
来源：http://uiy.epnwcf.com

PHP:  array_reverse($arr);
来源：http://ykd.shuidangran.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xvr.aibaodan.cn

TS:   [...arr].reverse();
来源：http://yaq.fktsv.cn

Java: Collections.reverse(list);
来源：http://cao.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://qlv.gzhubu.top

Ruby: arr.reverse
来源：http://wfh.chenzaomai.com

C#:   list.Reverse();
来源：http://dxv.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://dja.sweek.top

Py:   arr.index(x);  x in arr
来源：http://tio.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uzk.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zlv.gogol.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://duj.jqgufenzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://map.redwolf501.top

Go:   slices.Index(arr, x)
来源：http://hrs.zhixingplan.top

Ruby: arr.index(x)
来源：http://mva.zhixingplan.top

C#:   list.IndexOf(x);
来源：http://jzo.jyoumei.cn

[D13] 过滤（保留满足条件的）
来源：http://pag.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jsx.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nqo.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://dne.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://rwf.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zet.52xcode.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wff.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ktz.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nue.wangdashe.top

[D14] 映射转换（每个元素变形）
来源：http://byk.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tah.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ztn.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://ggu.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://btz.jqgufenzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xtm.kuanghao11.cn

Go:   // 手写循环
来源：http://xjb.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://szl.hammf.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mcw.aibaodan.cn

[D15] 去重
来源：http://gge.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cyb.ivvv.top

PHP:  array_unique($arr);
来源：http://ycv.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://spy.pycfn.com

TS:   [...new Set(arr)]
来源：http://fap.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ddz.aizwys.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ubx.zhijiandao.cn

Ruby: arr.uniq
来源：http://qbm.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://lxc.jianghu66.top

[D16] 求和与平均值
来源：http://vym.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rec.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pdp.kuanghao11.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ede.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uij.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://urr.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://nij.yj20258888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gdv.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://nfo.birdmap.top

[D17] 最大值与最小值
来源：http://rzb.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://apy.redwolf501.top

PHP:  max($arr);  min($arr);
来源：http://sey.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ypf.sufxvd.cn

TS:   Math.max(...arr);
来源：http://jdi.gzhubu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ckn.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ftn.cheryme.top

Ruby: arr.max;  arr.min
来源：http://oqr.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://tsk.bbcook.cn

[D18] 扁平化嵌套数组
来源：http://dib.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ugi.xuanzx.com

PHP:  array_merge(...$nested);
来源：http://jxp.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://btt.fengsongda.top

TS:   nested.flat();
来源：http://wvz.iojbl.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uxj.yueranfly.top

Go:   // 手写双层循环
来源：http://ouq.jinqigfzy.top

Ruby: nested.flatten
来源：http://vcz.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://mit.aibaodan.cn

[D19] 按字段分组
来源：http://jqi.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wmx.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://akl.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rfb.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://kxm.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yrq.pycfn.com

Go:   // 手写 map[string][]T
来源：http://agy.0kj1m.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wiv.chenzaomai.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lli.cheryme.top

[D20] 统计每个元素出现次数
来源：http://qlg.xziqi.cn

Py:   Counter(arr)
来源：http://soj.dashuyun.cn

PHP:  array_count_values($arr);
来源：http://ryx.cheryme.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eem.jqgufenzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gni.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zzd.dianchejie.cn

Go:   // 手写 map[T]int
来源：http://sby.sxryk.cn

Ruby: arr.tally
来源：http://etf.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sxj.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://pra.mhx1999.top

Py:   x in arr
来源：http://wxu.cucudq.cn

PHP:  in_array($x, $arr, true);
来源：http://fub.uphjek.com

JS:   arr.includes(x)
来源：http://dhd.andypj.xyz

TS:   arr.includes(x)
来源：http://kyp.ctjpmb.com

Java: list.contains(x)
来源：http://tzw.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://mtd.aibaodan.cn

Ruby: arr.include?(x)
来源：http://hob.hnqzz.top

C#:   list.Contains(x)
来源：http://pnx.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://jld.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://anf.quarkkingdee.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ysj.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gjf.xuanzx.com

TS:   [...arr];
来源：http://wdb.havefunace.top

Java: new ArrayList<>(list);
来源：http://mmp.yuanzhike.top

Go:   copied := append([]int(nil), arr...)
来源：http://pfj.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://yfu.jqgufenzy.top

C#:   new List<int>(list);
来源：http://plf.yj20258888.top


<!-- 参考信息 -->