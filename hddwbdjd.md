代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://rvs.quarkkingdee.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iaq.hnqzz.top

Go:   sq := func(x int) int { return x * x }
来源：http://oab.ivvv.top

Ruby: square = ->(x) { x * x }
来源：http://lvg.hesvh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oog.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://jjd.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kjm.tian-w.cn

PHP:  array_map("strtoupper", $arr);
来源：http://szy.hongshengwenyu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ifh.jinqigfzy.top

TS:   arr.map(String)
来源：http://lwe.ehwqpu.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lfy.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ism.aibaodan.cn

Ruby: arr.map(&:upcase)
来源：http://sqh.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://wsj.fanxiaobao.xyz

[C08] 闭包
来源：http://jyx.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yof.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://acl.xziqi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wsk.zycfv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bgu.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kbb.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hym.bjfxy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uar.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ghk.zycfv.cn

[C09] 递归
来源：http://iso.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ypk.quarkkingdee.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ozj.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://crp.shanyushiyangtech.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uvn.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dpv.ybcxt.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vbh.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ovh.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rqs.smart0.xyz

[C10] 变量作用域
来源：http://bmx.dianchejie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rwl.jinqigufen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iyq.cdnleiting.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kck.daxiang520.top

TS:   同 JS
来源：http://cwb.aibaodan.cn

Java: 方法内为块级作用域
来源：http://nba.aizwys.cn

Go:   花括号块级作用域
来源：http://ueg.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lrj.smart0.xyz

C#:   块级作用域
来源：http://bud.ctjpmb.com

[C11] 模块导入与导出
来源：http://qfp.jlsjyb.cn

Py:   from module import func
来源：http://xkn.hcnkem.com

PHP:  require "file.php";  或 use App\Service;
来源：http://dpo.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kmo.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rdg.birdmap.top

Java: import java.util.List;
来源：http://qiz.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://eqa.tanke756.top

C#:   using System.Text;
来源：http://lyk.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://bdr.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://vac.yanxiufei.cn

PHP:  (function () { echo "run"; })();
来源：http://piy.jinyuanbaomall.cn

JS:   (() => { console.log("run"); })();
来源：http://wcr.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://cpr.316326.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tiw.meibo888.top

Go:   func() { fmt.Println("run") }()
来源：http://lqf.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://yqw.sweek.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rxm.sxryk.cn

[C13] 类型声明 / 类型注解
来源：http://miz.tianlin.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dgl.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kjs.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://osm.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sci.zhaomingkeji.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://foq.sweek.top

Go:   func add(a, b int) int
来源：http://lev.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rmx.zdqjudy.top

C#:   int Add(int a, int b) => a + b;
来源：http://rej.andypj.xyz

[C14] 泛型函数
来源：http://psp.yj20258.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://smx.uphjek.com

PHP:  // 无泛型
来源：http://yiw.xinyue.icu

JS:   // 无泛型
来源：http://hwf.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://quf.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vpl.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gkv.feifeiyinyue.top

Ruby: # 无泛型
来源：http://wbq.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fcf.andypj.xyz

[C15] 解构 / 展开参数
来源：http://xxv.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cqz.sweek.top

PHP:  [$a, $b] = $pair;
来源：http://grs.guannengcc.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://svn.xinyue.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iiv.jinqigufen.top

Java: // 无解构
来源：http://zkx.yj202588.top

Go:   // 无解构
来源：http://vqk.yongpay.top

Ruby: a, b = pair
来源：http://prz.guannengcc.top

C#:   var (a, b) = pair;
来源：http://kxr.guannengcc.top

[C16] 函数 / 方法重载
来源：http://bwf.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qzc.gotoacloud.top

PHP:  // 无重载
来源：http://pem.bjfxy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pqk.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://can.zhoulong.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://eev.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://fry.yongpay.top

Ruby: # 无重载：靠动态参数
来源：http://zpd.fanxiaobao.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://dnc.ybcxt.top

================================================================================
来源：http://lre.smart0.xyz

D. 数组 / 列表 / 集合
来源：http://phk.wangshuangyany.cn

================================================================================
来源：http://tky.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://ash.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lng.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ovv.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qom.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://jeg.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dbn.cucudq.cn

Go:   arr := []int{1, 2, 3}
来源：http://wwe.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://rid.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dwk.yj20258888.top

[D02] 追加元素到末尾
来源：http://uwz.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://alx.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pnr.zhixingplan.top

JS:   arr.push(4);
来源：http://cbh.daria6918.cn

TS:   arr.push(4);
来源：http://msg.ctjpmb.com

Java: list.add(4);
来源：http://ufr.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://pwz.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://gdy.cqqwz.cn

C#:   list.Add(4);
来源：http://fsj.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://cmr.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://kbx.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yvo.xinyue.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kae.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://tur.jqgufenzy.top

Java: list.add(0, 0);
来源：http://bqc.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://eel.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://thf.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://hae.cqqwz.cn

[D04] 删除元素
来源：http://aii.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wrw.ybcxt.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lwb.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bdq.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://zis.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kbt.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ywi.mhx1999.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mkw.yj20258888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cbr.uphjek.com

[D05] 访问与修改元素
来源：http://pms.zhongyouzk.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ype.chenlongwang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mcs.zdqjudy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nvn.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://hkl.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://uop.yongpay.top

Go:   arr[0]; arr[0] = 9
来源：http://pbk.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uwz.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ler.meibo888.top

[D06] 数组长度
来源：http://dmj.xuanzx.com

Py:   len(arr)
来源：http://chy.quarkkingdee.top

PHP:  count($arr);
来源：http://ccu.xingfuxueyuan.xyz

JS:   arr.length
来源：http://zdg.cqqwz.cn

TS:   arr.length
来源：http://slm.hfpthk.cn

Java: list.size();
来源：http://jpc.fzhhl.top

Go:   len(arr)
来源：http://nrf.smart0.xyz

Ruby: arr.length; arr.size
来源：http://qjs.shuidangran.top

C#:   list.Count;
来源：http://hrr.daxiang520.top

[D07] 切片 / 取子数组
来源：http://exs.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qqo.chenjidiqi.icu

PHP:  array_slice($arr, 1, 3);
来源：http://wwk.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://ulk.cheryme.top

TS:   arr.slice(1, 4);
来源：http://rkd.hnqzz.top

Java: list.subList(1, 4);
来源：http://emx.316326.xyz

Go:   arr[1:4]
来源：http://bhb.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://tps.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://xvw.hcnkem.com

[D08] 合并两个数组
来源：http://osp.shuidangran.top

Py:   a + b;  a.extend(b)
来源：http://zvq.tanke756.top

PHP:  array_merge($a, $b);
来源：http://odb.uphjek.com

JS:   [...a, ...b];  a.concat(b);
来源：http://mpl.meibo888.top

TS:   [...a, ...b];
来源：http://cnl.hcnkem.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dxt.fengsongda.top

Go:   append(a, b...)
来源：http://gie.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://kel.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://okw.jiagoushi.top

[D09] 排序（升序）
来源：http://lvs.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://omc.sxryk.cn

PHP:  sort($arr);
来源：http://tkz.fehbvm.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dgt.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oah.ydzc1.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qeg.zhaomingkeji.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://djm.hcnkem.com

Ruby: arr.sort
来源：http://boc.dianchejie.cn

C#:   list.Sort();
来源：http://jzk.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hec.fzhhl.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lfz.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wut.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hej.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tog.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nsa.daxiang520.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://agp.yj202588.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aoi.smart0.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gct.tianlin.xyz

[D11] 反转数组
来源：http://gds.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://zlr.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://bvb.meibo888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://axr.vehdjk.com

TS:   [...arr].reverse();
来源：http://ija.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://tzd.andypj.xyz

Go:   slices.Reverse(arr)
来源：http://yji.xinyue.icu

Ruby: arr.reverse
来源：http://sjv.pengpengdd.cyou

C#:   list.Reverse();
来源：http://gdm.zhijiandao.cn

[D12] 查找元素下标
来源：http://faw.hammf.cn

Py:   arr.index(x);  x in arr
来源：http://chw.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://npj.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tkn.sysykeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jrq.tanke756.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cpc.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://ple.bjfxy.top

Ruby: arr.index(x)
来源：http://cnr.fzhhl.top

C#:   list.IndexOf(x);
来源：http://njp.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://ivz.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iom.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xey.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://rfb.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://glg.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fts.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cuh.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://rhu.tarul.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jho.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://qqq.yuanzhike.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://epk.snrcjt.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qbf.havefunace.top

JS:   arr.map(x => x * 2)
来源：http://gmj.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://lls.gaohongyu789.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mjb.shzxlz.cn

Go:   // 手写循环
来源：http://eul.yueranfly.top

Ruby: arr.map { |x| x * 2 }
来源：http://yuf.jqgufenzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://soh.sysykeji.top

[D15] 去重
来源：http://non.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qst.52xcode.cn

PHP:  array_unique($arr);
来源：http://qox.yanxiufei.cn

JS:   [...new Set(arr)]
来源：http://zuv.316326.xyz

TS:   [...new Set(arr)]
来源：http://ykf.meibo888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mha.shangyingyoupin.top

Go:   // 用 map[T]struct{} 手写
来源：http://qtr.nanxinkj.top

Ruby: arr.uniq
来源：http://jwx.sweek.top

C#:   list.Distinct().ToList()
来源：http://szk.mhx1999.top

[D16] 求和与平均值
来源：http://uux.fehbvm.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yni.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://njb.yonumen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://slg.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sjo.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://luf.nanxuanxn.top

Go:   // 手写循环累加
来源：http://blt.hysaishi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uti.hnxiangtu.top

C#:   list.Sum();  list.Average()
来源：http://qlb.cashguo.top

[D17] 最大值与最小值
来源：http://ztf.hysaishi.cn

Py:   max(arr);  min(arr)
来源：http://kce.wangdashe.top

PHP:  max($arr);  min($arr);
来源：http://aty.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hsp.hammf.cn

TS:   Math.max(...arr);
来源：http://ajn.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://zct.dashuyun.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jem.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://rtj.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://iwy.sweek.top

[D18] 扁平化嵌套数组
来源：http://fkb.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pia.nwbrower.top

PHP:  array_merge(...$nested);
来源：http://noi.nanxuanxn.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uae.zhijiandao.cn

TS:   nested.flat();
来源：http://tdv.hywenlv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jxo.yfazqb.com

Go:   // 手写双层循环
来源：http://ddd.xylfe.cn

Ruby: nested.flatten
来源：http://zlw.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://vuq.xinyue.icu

[D19] 按字段分组
来源：http://nhs.ivvv.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tni.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://afn.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qms.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mpb.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cxx.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://opf.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jck.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kbe.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://mnr.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://ehi.sweek.top

PHP:  array_count_values($arr);
来源：http://mzn.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cme.andypj.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zuv.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vii.jinqigfzy.top

Go:   // 手写 map[T]int
来源：http://tlv.zhoulong.xyz

Ruby: arr.tally
来源：http://nrt.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cta.epnwcf.com

[D21] 判断是否包含某元素
来源：http://tpy.feifeiyinyue.top

Py:   x in arr
来源：http://mjm.zdqjudy.top

PHP:  in_array($x, $arr, true);
来源：http://yom.ctjpmb.com

JS:   arr.includes(x)
来源：http://bik.jianghu66.top

TS:   arr.includes(x)
来源：http://qya.yj202588.top

Java: list.contains(x)
来源：http://hgp.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://fik.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://eiy.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://etq.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://rwf.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://noa.shzxlz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iiy.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zax.sufxvd.cn

TS:   [...arr];
来源：http://pyv.cucudq.cn

Java: new ArrayList<>(list);
来源：http://ult.shangyingyoupin.top

Go:   copied := append([]int(nil), arr...)
来源：http://lxj.epnwcf.com

Ruby: arr.dup;  arr.clone
来源：http://ttv.jlsjyb.cn

C#:   new List<int>(list);
来源：http://eab.cdnleiting.top

[D23] reduce 累积计算
来源：http://ajc.feifeiyinyue.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jym.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mef.sjlbkw.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iqz.yvedp.cn


<!-- 参考信息 -->