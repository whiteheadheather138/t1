代发 wailian999

[C06] 匿名函数 / lambda
来源：http://bem.jianghu66.top

Py:   square = lambda x: x * x
来源：http://gur.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fjs.hesvh.cn

JS:   const square = x => x * x;
来源：http://hxf.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://opt.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qij.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mvo.hesvh.cn

Ruby: square = ->(x) { x * x }
来源：http://ocd.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://ydz.jinyuanbaomall.cn

[C07] 把函数作为参数传入
来源：http://uhe.ywan-chungtsiang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://brj.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bus.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://svz.ydjk.org.cn

TS:   arr.map(String)
来源：http://rvj.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gti.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cxo.sufxvd.cn

Ruby: arr.map(&:upcase)
来源：http://ebc.yongpay.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vav.guowangkeji.top

[C08] 闭包
来源：http://gpb.tarul.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://clw.fanxiaobao.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://laa.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xuv.uphjek.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vvq.jinqigufen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://trc.fktsv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yzl.xylfe.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gvf.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uqw.hammf.cn

[C09] 递归
来源：http://xpg.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wxe.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ojw.fanxiaobao.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://llm.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://urd.fanxiaobao.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ouv.hesvh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jul.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yrh.hfpthk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uqe.cashguo.top

[C10] 变量作用域
来源：http://ozn.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mqi.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yhx.gotoacloud.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xac.zhiwuduotai.top

TS:   同 JS
来源：http://vhv.zhiwuduotai.top

Java: 方法内为块级作用域
来源：http://txi.nanxuanxn.top

Go:   花括号块级作用域
来源：http://enh.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jsi.yj202588.top

C#:   块级作用域
来源：http://zby.chenzaomai.com

[C11] 模块导入与导出
来源：http://hnm.xuanzx.com

Py:   from module import func
来源：http://pcu.jqgfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fvp.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://ftn.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ves.bjfxy.top

Java: import java.util.List;
来源：http://mrd.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qho.shanyushiyangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://vea.9152youxi.cn

C#:   using System.Text;
来源：http://jek.sjlbkw.cn

[C12] 立即执行函数 IIFE
来源：http://qce.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://rpa.yvedp.cn

PHP:  (function () { echo "run"; })();
来源：http://plz.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://ytx.sjlbkw.cn

TS:   (() => { console.log("run"); })();
来源：http://ltg.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gcq.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://czj.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://erk.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fcb.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://utq.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xqg.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jta.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gcd.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jej.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://fgq.xylfe.cn

Go:   func add(a, b int) int
来源：http://wrl.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nlk.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qht.xuanzx.com

[C14] 泛型函数
来源：http://hvx.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ynn.zdqjudy.top

PHP:  // 无泛型
来源：http://fxf.jianghu66.top

JS:   // 无泛型
来源：http://uxs.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://luy.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://feg.jiagoushi.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uve.zdbjq.cn

Ruby: # 无泛型
来源：http://kuk.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rse.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://msa.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sez.tian-w.cn

PHP:  [$a, $b] = $pair;
来源：http://jzr.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ajj.quarkkingdee.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wpp.shuidangran.top

Java: // 无解构
来源：http://kfu.ybcxt.top

Go:   // 无解构
来源：http://dxn.jiagoushi.top

Ruby: a, b = pair
来源：http://zfg.ybcxt.top

C#:   var (a, b) = pair;
来源：http://pbt.xinyue.icu

[C16] 函数 / 方法重载
来源：http://dsb.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kte.shangyingyoupin.top

PHP:  // 无重载
来源：http://qqq.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://snf.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://hlh.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xwe.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://eob.aizwys.cn

Ruby: # 无重载：靠动态参数
来源：http://spv.shzxlz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xkw.gzhubu.top

================================================================================
来源：http://szu.sweek.top

D. 数组 / 列表 / 集合
来源：http://iaa.dashuyun.cn

================================================================================
来源：http://nmt.smart0.xyz

[D01] 创建数组 / 列表
来源：http://wmj.kuanghao11.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iec.tarul.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eej.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ogv.9152youxi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fod.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ffp.52xcode.cn

Go:   arr := []int{1, 2, 3}
来源：http://wrr.yj20258888.top

Ruby: arr = [1, 2, 3]
来源：http://xpe.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eqe.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://nxu.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lsd.snrcjt.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vaq.yvedp.cn

JS:   arr.push(4);
来源：http://pom.haohaochexian.top

TS:   arr.push(4);
来源：http://sbr.wangdashe.top

Java: list.add(4);
来源：http://qim.dianchejie.cn

Go:   arr = append(arr, 4)
来源：http://fav.uphjek.com

Ruby: arr << 4; arr.push(5)
来源：http://zcm.xingfuxueyuan.xyz

C#:   list.Add(4);
来源：http://jps.yj20258.top

[D03] 在指定位置插入元素
来源：http://ixo.zhixingplan.top

Py:   arr.insert(0, 0)
来源：http://kvt.meibo888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xvp.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hey.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://wgp.havefunace.top

Java: list.add(0, 0);
来源：http://qgm.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://yqn.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nhk.andypj.xyz

C#:   list.Insert(0, 0);
来源：http://znu.birdmap.top

[D04] 删除元素
来源：http://fbo.zhaomingkeji.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vrl.dianchejie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ifb.jiagoushi.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://elb.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://jkg.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dup.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vwy.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xtp.gzhubu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://psz.havefunace.top

[D05] 访问与修改元素
来源：http://cll.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ayz.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rlf.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ypl.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://nxe.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://aie.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://rhk.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://moy.smart0.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yjz.sweek.top

[D06] 数组长度
来源：http://jjs.vehdjk.com

Py:   len(arr)
来源：http://vsd.jinghuilouyu.cn

PHP:  count($arr);
来源：http://vts.quarkkingdee.top

JS:   arr.length
来源：http://qek.yj202588.top

TS:   arr.length
来源：http://mmu.316326.xyz

Java: list.size();
来源：http://tbk.gotoacloud.top

Go:   len(arr)
来源：http://ghk.cashguo.top

Ruby: arr.length; arr.size
来源：http://che.jiagoushi.top

C#:   list.Count;
来源：http://lob.yangfankeji.com

[D07] 切片 / 取子数组
来源：http://flm.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://smo.tarul.cn

PHP:  array_slice($arr, 1, 3);
来源：http://apc.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://exm.nanxinkj.top

TS:   arr.slice(1, 4);
来源：http://ekb.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://lpg.feifeiyinyue.top

Go:   arr[1:4]
来源：http://ebb.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://lyg.birdmap.top

C#:   list.GetRange(1, 3);
来源：http://rlw.jlsjyb.cn

[D08] 合并两个数组
来源：http://osa.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://lqz.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://bro.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vmv.vqdsnc.cn

TS:   [...a, ...b];
来源：http://zpi.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zcu.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://kep.52xcode.cn

Ruby: a + b;  a.concat(b)
来源：http://hij.redwolf501.top

C#:   a.Concat(b).ToList()
来源：http://imc.andypj.xyz

[D09] 排序（升序）
来源：http://ria.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://mrz.iojbl.cn

PHP:  sort($arr);
来源：http://kwb.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ctv.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://pka.iojbl.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sds.hammf.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lcn.ppjwa.cn

Ruby: arr.sort
来源：http://ptf.vehdjk.com

C#:   list.Sort();
来源：http://stw.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cau.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qme.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bta.jinqigfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iji.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ewd.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ldh.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ggd.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fkt.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://naz.c1oappe.top

[D11] 反转数组
来源：http://ztq.hongshengwenyu.top

Py:   arr[::-1];  arr.reverse()
来源：http://nmf.cucudq.cn

PHP:  array_reverse($arr);
来源：http://jco.shuidangran.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pxr.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://dao.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://buo.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://dxa.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://jrk.ctjpmb.com

C#:   list.Reverse();
来源：http://tsn.sjlbkw.cn

[D12] 查找元素下标
来源：http://iyl.yj202588.top

Py:   arr.index(x);  x in arr
来源：http://qzt.yuanzhike.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tsu.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qcf.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jwl.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vlt.iojbl.cn

Go:   slices.Index(arr, x)
来源：http://eek.daxiang520.top

Ruby: arr.index(x)
来源：http://qta.smart0.xyz

C#:   list.IndexOf(x);
来源：http://hvh.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://dju.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kec.shzxlz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eqg.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://jyu.ivvv.top

TS:   arr.filter(x => x > 3)
来源：http://rbj.zhiwuduotai.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oux.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xus.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://hog.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bqp.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://rcj.jianghu66.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nbb.zdbjq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fwy.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://igx.birdmap.top

TS:   arr.map(x => x * 2)
来源：http://cog.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://occ.sweek.top

Go:   // 手写循环
来源：http://jcb.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://zwb.nwbrower.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gpy.hnxiangtu.top

[D15] 去重
来源：http://lfs.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mnd.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://zhf.meibo888.top

JS:   [...new Set(arr)]
来源：http://iyd.yj202588.top

TS:   [...new Set(arr)]
来源：http://uhf.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lwa.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rrw.feifeiyinyue.top

Ruby: arr.uniq
来源：http://ole.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://lia.tianlin.xyz

[D16] 求和与平均值
来源：http://dpi.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qmt.yueranfly.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ebv.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://odq.shanyushiyangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wam.hnxiangtu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vik.iojbl.cn

Go:   // 手写循环累加
来源：http://wig.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gno.haohaochexian.top

C#:   list.Sum();  list.Average()
来源：http://lcb.nwbrower.top

[D17] 最大值与最小值
来源：http://dlo.zhijiandao.cn

Py:   max(arr);  min(arr)
来源：http://zds.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://rfs.shanyushiyangtech.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cit.epnwcf.com

TS:   Math.max(...arr);
来源：http://ngv.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fxu.gzhubu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vcp.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://idp.snrcjt.cn

C#:   list.Max();  list.Min()
来源：http://dff.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://uee.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hfq.ppjwa.cn

PHP:  array_merge(...$nested);
来源：http://eav.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://icb.havefunace.top

TS:   nested.flat();
来源：http://yqt.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://igf.9152youxi.cn

Go:   // 手写双层循环
来源：http://sjj.svipenyu.cn

Ruby: nested.flatten
来源：http://rbq.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uvm.xylfe.cn

[D19] 按字段分组
来源：http://lck.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dtm.yueranfly.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qjn.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jyc.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://opm.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nrp.yj20258.top

Go:   // 手写 map[string][]T
来源：http://bju.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xwi.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qfg.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://guh.sweek.top

Py:   Counter(arr)
来源：http://hwl.xziqi.cn

PHP:  array_count_values($arr);
来源：http://wpj.sweek.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ojs.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cyp.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dkz.xylfe.cn

Go:   // 手写 map[T]int
来源：http://hkb.wangshuangyany.cn

Ruby: arr.tally
来源：http://zkr.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fos.cucudq.cn

[D21] 判断是否包含某元素
来源：http://dxh.smart0.xyz

Py:   x in arr
来源：http://jzp.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://jvo.9152youxi.cn

JS:   arr.includes(x)
来源：http://wff.316326.xyz

TS:   arr.includes(x)
来源：http://cnr.gzhubu.top

Java: list.contains(x)
来源：http://qdk.redwolf501.top

Go:   slices.Contains(arr, x)
来源：http://nfr.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://fvj.9152youxi.cn

C#:   list.Contains(x)
来源：http://lbs.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://zzb.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rxx.iojbl.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eal.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pyt.yanxiufei.cn

TS:   [...arr];
来源：http://jjr.fehbvm.com

Java: new ArrayList<>(list);
来源：http://vxc.yuanzhike.top

Go:   copied := append([]int(nil), arr...)
来源：http://jtp.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://diu.yueranfly.top

C#:   new List<int>(list);
来源：http://vnm.fanxiaobao.xyz


<!-- 参考信息 -->