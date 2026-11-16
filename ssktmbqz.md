代发 wailian999

[C06] 匿名函数 / lambda
来源：http://zus.hcnkem.com

Py:   square = lambda x: x * x
来源：http://ich.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://toe.hongshengwenyu.top

JS:   const square = x => x * x;
来源：http://aww.feifeiyinyue.top

TS:   const square = (x: number): number => x * x;
来源：http://irq.hnqzz.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kyh.yuanzhike.top

Go:   sq := func(x int) int { return x * x }
来源：http://ahw.birdmap.top

Ruby: square = ->(x) { x * x }
来源：http://lxc.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jxu.kuanghao11.cn

[C07] 把函数作为参数传入
来源：http://kuc.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xqg.jqgfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://rxe.iojbl.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://htg.zdqjudy.top

TS:   arr.map(String)
来源：http://kvy.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://flj.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qod.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://wef.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fph.ehwqpu.com

[C08] 闭包
来源：http://wsw.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fsg.fktsv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cma.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bly.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cgn.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nyf.pengpengdd.cyou

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tmt.snrcjt.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vhp.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gbl.gotoacloud.top

[C09] 递归
来源：http://ygj.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dpn.vqdsnc.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://azh.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vpy.smart0.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://btp.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lcy.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xba.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jpc.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vel.iojbl.cn

[C10] 变量作用域
来源：http://zvn.gotoacloud.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://buj.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yns.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cai.0kj1m.cn

TS:   同 JS
来源：http://pwr.birdmap.top

Java: 方法内为块级作用域
来源：http://uis.cheryme.top

Go:   花括号块级作用域
来源：http://pgg.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ayx.cashguo.top

C#:   块级作用域
来源：http://yay.jqgufenzy.top

[C11] 模块导入与导出
来源：http://edv.yongpay.top

Py:   from module import func
来源：http://moj.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://crc.feifeiyinyue.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zwu.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zzq.nanxinkj.top

Java: import java.util.List;
来源：http://mcd.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ajm.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://aec.hywenlv.cn

C#:   using System.Text;
来源：http://phk.yanxiufei.cn

[C12] 立即执行函数 IIFE
来源：http://lke.svipenyu.cn

Py:   (lambda: print("run"))()
来源：http://ssi.chenzaomai.com

PHP:  (function () { echo "run"; })();
来源：http://elh.zhijiandao.cn

JS:   (() => { console.log("run"); })();
来源：http://ves.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://vay.cdnleiting.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mod.cucudq.cn

Go:   func() { fmt.Println("run") }()
来源：http://sev.wangshuangyany.cn

Ruby: -> { puts "run" }.call
来源：http://cpx.ctjpmb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://hmb.ydjk.org.cn

[C13] 类型声明 / 类型注解
来源：http://adp.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hbq.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ngx.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gnk.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rxc.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://uvr.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://tgp.chenzaomai.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nca.zdqjudy.top

C#:   int Add(int a, int b) => a + b;
来源：http://jbq.yj202588.top

[C14] 泛型函数
来源：http://pwo.ywan-chungtsiang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mxs.yuanzhike.top

PHP:  // 无泛型
来源：http://gzg.chenjidiqi.icu

JS:   // 无泛型
来源：http://hqs.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wke.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jro.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ovp.zdqjudy.top

Ruby: # 无泛型
来源：http://elf.ydjk.org.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mgu.havefunace.top

[C15] 解构 / 展开参数
来源：http://qdn.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cre.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://lrh.xylfe.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ias.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ofl.smart0.xyz

Java: // 无解构
来源：http://jrs.hcnkem.com

Go:   // 无解构
来源：http://srj.shangyingyoupin.top

Ruby: a, b = pair
来源：http://fvn.hcnkem.com

C#:   var (a, b) = pair;
来源：http://mki.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://ibt.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rmd.jqgufenzy.top

PHP:  // 无重载
来源：http://rdq.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://vwm.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://sjo.bjfxy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ikz.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://ffa.hysaishi.cn

Ruby: # 无重载：靠动态参数
来源：http://nwr.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://aqk.hcnkem.com

================================================================================
来源：http://uwc.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://cwu.hysaishi.cn

================================================================================
来源：http://ubg.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://ksw.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ibg.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wjm.sxryk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://egv.guannengcc.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ral.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pau.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://lnc.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://jpr.yvedp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dbn.gogol.net.cn

[D02] 追加元素到末尾
来源：http://ezu.zycfv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ebr.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nkg.zhoulong.xyz

JS:   arr.push(4);
来源：http://ifp.ivvv.top

TS:   arr.push(4);
来源：http://khf.zhixingplan.top

Java: list.add(4);
来源：http://tpt.cheryme.top

Go:   arr = append(arr, 4)
来源：http://lqo.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://pxi.feifeiyinyue.top

C#:   list.Add(4);
来源：http://vkl.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://kly.pycfn.com

Py:   arr.insert(0, 0)
来源：http://peb.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dvp.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rhm.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://weq.zhijiandao.cn

Java: list.add(0, 0);
来源：http://bfy.316326.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://uui.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ets.hfpthk.cn

C#:   list.Insert(0, 0);
来源：http://mzi.jlsjyb.cn

[D04] 删除元素
来源：http://gas.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cxo.yj20258888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zgk.shangyingyoupin.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lis.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://qtk.jinqigufen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gsm.jiagoushi.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wgk.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dmo.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oyz.jqgufenzy.top

[D05] 访问与修改元素
来源：http://csh.jiagoushi.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aol.nwbrower.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gla.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://msy.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://ufm.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://jnr.uphjek.com

Go:   arr[0]; arr[0] = 9
来源：http://pmx.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lul.shangyingyoupin.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aod.vehdjk.com

[D06] 数组长度
来源：http://vqe.hysaishi.cn

Py:   len(arr)
来源：http://pxa.xuanzx.com

PHP:  count($arr);
来源：http://vcr.jlsjyb.cn

JS:   arr.length
来源：http://ukk.wangdashe.top

TS:   arr.length
来源：http://dlt.chenjidiqi.icu

Java: list.size();
来源：http://ltg.haohaochexian.top

Go:   len(arr)
来源：http://zuv.fengsongda.top

Ruby: arr.length; arr.size
来源：http://bvq.ctjpmb.com

C#:   list.Count;
来源：http://jnz.cashguo.top

[D07] 切片 / 取子数组
来源：http://qnr.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rcp.chenjidiqi.icu

PHP:  array_slice($arr, 1, 3);
来源：http://irh.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://twf.xylfe.cn

TS:   arr.slice(1, 4);
来源：http://ocl.yuxming.cn

Java: list.subList(1, 4);
来源：http://tyu.ctjpmb.com

Go:   arr[1:4]
来源：http://igb.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://csj.jlsjyb.cn

C#:   list.GetRange(1, 3);
来源：http://gcn.fktsv.cn

[D08] 合并两个数组
来源：http://hnw.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://nnj.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://jxn.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bwt.cashguo.top

TS:   [...a, ...b];
来源：http://qys.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fca.0kj1m.cn

Go:   append(a, b...)
来源：http://kco.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://goz.ydzc1.top

C#:   a.Concat(b).ToList()
来源：http://rpo.uphjek.com

[D09] 排序（升序）
来源：http://umw.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://avi.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://iav.fengsongda.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kci.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xbw.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://ewx.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ifo.fanxiaobao.xyz

Ruby: arr.sort
来源：http://mjg.yvedp.cn

C#:   list.Sort();
来源：http://eiq.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lut.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ykh.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://arj.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wmw.jinqigfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xal.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rla.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://scu.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ugw.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dyd.iojbl.cn

[D11] 反转数组
来源：http://irp.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sdp.daria6918.cn

PHP:  array_reverse($arr);
来源：http://ypw.ehwqpu.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eov.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://bcd.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://oza.jianghu66.top

Go:   slices.Reverse(arr)
来源：http://qrv.yuxming.cn

Ruby: arr.reverse
来源：http://tmj.yfazqb.com

C#:   list.Reverse();
来源：http://kqw.tian-w.cn

[D12] 查找元素下标
来源：http://yqn.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://gej.316326.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pbk.316326.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dws.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vhl.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://syc.redwolf501.top

Go:   slices.Index(arr, x)
来源：http://kve.gaohongyu789.top

Ruby: arr.index(x)
来源：http://uez.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://edl.yfazqb.com

[D13] 过滤（保留满足条件的）
来源：http://ijp.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mqj.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eef.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://gjj.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://aah.shanyushiyangtech.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lxp.shzxlz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vxj.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://jdw.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bbq.guannengcc.top

[D14] 映射转换（每个元素变形）
来源：http://zgr.redwolf501.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://toq.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zcz.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://row.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://drs.0kj1m.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ual.hnxiangtu.top

Go:   // 手写循环
来源：http://xqr.jinqigfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://smq.cdnleiting.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ooa.yuxming.cn

[D15] 去重
来源：http://bpb.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dpg.wangshuangyany.cn

PHP:  array_unique($arr);
来源：http://gmd.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://kju.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://pdv.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gje.gotoacloud.top

Go:   // 用 map[T]struct{} 手写
来源：http://xqg.ivvv.top

Ruby: arr.uniq
来源：http://kwb.fehbvm.com

C#:   list.Distinct().ToList()
来源：http://xaq.yonumen.top

[D16] 求和与平均值
来源：http://mhx.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://szk.yj202588.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qtl.sysykeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://war.fanxiaobao.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cvi.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qar.yvedp.cn

Go:   // 手写循环累加
来源：http://bko.daria6918.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bll.xingfuxueyuan.xyz

C#:   list.Sum();  list.Average()
来源：http://hdf.havefunace.top

[D17] 最大值与最小值
来源：http://pxu.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://wjz.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://jxt.52xcode.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gja.zhiwuduotai.top

TS:   Math.max(...arr);
来源：http://nye.shanyushiyangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://efb.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://him.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://oum.wangdashe.top

C#:   list.Max();  list.Min()
来源：http://grf.zhongyouzk.top

[D18] 扁平化嵌套数组
来源：http://hvq.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gza.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://vmm.xingfuxueyuan.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xmo.cdnleiting.top

TS:   nested.flat();
来源：http://ear.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eha.andypj.xyz

Go:   // 手写双层循环
来源：http://iha.jiagoushi.top

Ruby: nested.flatten
来源：http://pgp.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kds.shanyushiyangtech.top

[D19] 按字段分组
来源：http://tlm.fktsv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://raa.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pzp.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xhu.cdnleiting.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uwl.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mkx.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://xhg.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mqo.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kyy.ctjpmb.com

[D20] 统计每个元素出现次数
来源：http://qmd.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://sic.daria6918.cn

PHP:  array_count_values($arr);
来源：http://bwr.yvedp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ltk.hammf.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jza.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://idq.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://klz.0kj1m.cn

Ruby: arr.tally
来源：http://haz.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://juo.cheryme.top

[D21] 判断是否包含某元素
来源：http://ain.smart0.xyz

Py:   x in arr
来源：http://vio.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://qkk.9152youxi.cn

JS:   arr.includes(x)
来源：http://hly.fktsv.cn

TS:   arr.includes(x)
来源：http://jve.shzxlz.cn

Java: list.contains(x)
来源：http://lii.fktsv.cn

Go:   slices.Contains(arr, x)
来源：http://bgt.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://alw.cheryme.top

C#:   list.Contains(x)
来源：http://iwe.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://dcd.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uqy.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rfo.zhoulong.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aje.yangfankeji.com

TS:   [...arr];
来源：http://htd.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://soo.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://ynz.dashuyun.cn

Ruby: arr.dup;  arr.clone
来源：http://tmy.cucudq.cn

C#:   new List<int>(list);
来源：http://frv.nanxuanxn.top


<!-- 参考信息 -->