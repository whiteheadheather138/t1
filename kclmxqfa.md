代发 wailian999

[C06] 匿名函数 / lambda
来源：http://qve.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://vgj.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tno.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://hxg.ywan-chungtsiang.top

TS:   const square = (x: number): number => x * x;
来源：http://yfc.aizwys.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qxj.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://swe.ivvv.top

Ruby: square = ->(x) { x * x }
来源：http://xxt.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ldj.52xcode.cn

[C07] 把函数作为参数传入
来源：http://sph.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rmk.yfazqb.com

PHP:  array_map("strtoupper", $arr);
来源：http://non.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tdy.316326.xyz

TS:   arr.map(String)
来源：http://hns.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kfi.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wxs.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://ajf.snrcjt.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vwb.tianlin.xyz

[C08] 闭包
来源：http://qvw.birdmap.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rpg.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jdn.dashuyun.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://boz.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cou.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xii.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://swc.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://api.dashuyun.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fxr.yanxiufei.cn

[C09] 递归
来源：http://ale.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ckx.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ufc.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jqw.xuanzx.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vdm.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qdh.gogol.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mpf.shuidangran.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yvu.cheryme.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fwk.xziqi.cn

[C10] 变量作用域
来源：http://yfq.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://foj.tianlin.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lvl.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://irf.fehbvm.com

TS:   同 JS
来源：http://lta.hesvh.cn

Java: 方法内为块级作用域
来源：http://pqo.shanyushiyangkeji.top

Go:   花括号块级作用域
来源：http://ntb.9152youxi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kwb.guannengcc.top

C#:   块级作用域
来源：http://sor.tanke756.top

[C11] 模块导入与导出
来源：http://ozb.ybcxt.top

Py:   from module import func
来源：http://lcz.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zmb.zdbjq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ttn.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://czs.shangyingyoupin.top

Java: import java.util.List;
来源：http://vif.chenzaomai.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wmt.gzhubu.top

Ruby: require "json"; require_relative "./util"
来源：http://wte.hesvh.cn

C#:   using System.Text;
来源：http://tvg.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://dhh.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://bnj.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://non.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://wdt.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://fou.sysykeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fwj.9152youxi.cn

Go:   func() { fmt.Println("run") }()
来源：http://sze.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://yys.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wyj.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://dgu.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cos.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://itv.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nfs.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gfw.ybcxt.top

Java: int add(int a, int b) { return a + b; }
来源：http://lsj.yuxming.cn

Go:   func add(a, b int) int
来源：http://cnn.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dqc.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://ylv.sxryk.cn

[C14] 泛型函数
来源：http://iss.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wke.jiagoushi.top

PHP:  // 无泛型
来源：http://wmo.andypj.xyz

JS:   // 无泛型
来源：http://dqx.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dzv.gotoacloud.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qqa.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://euy.sjlbkw.cn

Ruby: # 无泛型
来源：http://ogm.dashuyun.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pij.xinyue.icu

[C15] 解构 / 展开参数
来源：http://qqa.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rbm.quarkkingdee.top

PHP:  [$a, $b] = $pair;
来源：http://phy.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tsp.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qdb.andypj.xyz

Java: // 无解构
来源：http://nxa.yj202588.top

Go:   // 无解构
来源：http://tar.andypj.xyz

Ruby: a, b = pair
来源：http://hjl.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://vcf.fktsv.cn

[C16] 函数 / 方法重载
来源：http://che.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fxj.ydzc1.top

PHP:  // 无重载
来源：http://lqv.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://auq.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://jbd.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hfx.ydzc1.top

Go:   // 无重载：用不同函数名
来源：http://tpq.xuetiantiany.cn

Ruby: # 无重载：靠动态参数
来源：http://xeb.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fal.0kj1m.cn

================================================================================
来源：http://hdm.feifeiyinyue.top

D. 数组 / 列表 / 集合
来源：http://ugj.sysykeji.top

================================================================================
来源：http://wpj.jinghuilouyu.cn

[D01] 创建数组 / 列表
来源：http://gmi.bbcook.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://znl.kuanghao11.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pcd.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eef.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yur.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uyd.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://wrl.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://eel.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dgo.sweek.top

[D02] 追加元素到末尾
来源：http://zkb.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lhq.yj202588.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://twh.nwbrower.top

JS:   arr.push(4);
来源：http://fqs.mhx1999.top

TS:   arr.push(4);
来源：http://iix.ivvv.top

Java: list.add(4);
来源：http://msh.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://vrr.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://mbr.tianlin.xyz

C#:   list.Add(4);
来源：http://efy.kuanghao11.cn

[D03] 在指定位置插入元素
来源：http://dxa.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://ijc.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yli.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://irm.ywan-chungtsiang.top

TS:   arr.splice(0, 0, 0);
来源：http://saf.ydjk.org.cn

Java: list.add(0, 0);
来源：http://vaw.316326.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://vfu.zdqjudy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jjj.jinghuilouyu.cn

C#:   list.Insert(0, 0);
来源：http://jbp.jlsjyb.cn

[D04] 删除元素
来源：http://ejx.ydjk.org.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jcv.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://php.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oar.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://btz.jiagoushi.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ffu.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://scf.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kpz.jqgfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uqq.daxiang520.top

[D05] 访问与修改元素
来源：http://inr.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://agv.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fws.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jyp.zhixingplan.top

TS:   arr[0]; arr.at(-1);
来源：http://zrk.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://kql.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://qnf.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ttq.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vrz.sysykeji.top

[D06] 数组长度
来源：http://ybx.xuanzx.com

Py:   len(arr)
来源：http://nkb.wangshuangyany.cn

PHP:  count($arr);
来源：http://wzu.jinghuilouyu.cn

JS:   arr.length
来源：http://wir.316326.xyz

TS:   arr.length
来源：http://cmf.yj20258888.top

Java: list.size();
来源：http://lwq.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://nvz.epnwcf.com

Ruby: arr.length; arr.size
来源：http://sdv.hnqzz.top

C#:   list.Count;
来源：http://gkw.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://dno.chenlongwang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fvr.ybcxt.top

PHP:  array_slice($arr, 1, 3);
来源：http://eir.hongshengwenyu.top

JS:   arr.slice(1, 4);
来源：http://ody.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://cgp.nanxinkj.top

Java: list.subList(1, 4);
来源：http://fht.sjlbkw.cn

Go:   arr[1:4]
来源：http://vtk.52xcode.cn

Ruby: arr[1, 3]
来源：http://unk.sjlbkw.cn

C#:   list.GetRange(1, 3);
来源：http://uzv.hammf.cn

[D08] 合并两个数组
来源：http://waz.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://nfz.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://nnw.zycfv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ana.yangfankeji.com

TS:   [...a, ...b];
来源：http://taw.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jxd.yj20258888.top

Go:   append(a, b...)
来源：http://pjw.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://wje.yj20258.top

C#:   a.Concat(b).ToList()
来源：http://cvh.ppjwa.cn

[D09] 排序（升序）
来源：http://nts.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://yft.ybcxt.top

PHP:  sort($arr);
来源：http://rjt.guannengcc.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vkx.tarul.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nej.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jsa.kuanghao11.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bfp.cashguo.top

Ruby: arr.sort
来源：http://yaw.vqdsnc.cn

C#:   list.Sort();
来源：http://qee.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fcc.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vcv.c1oappe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pgb.yuxming.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jju.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fud.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://otw.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://afa.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tep.yvedp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lej.birdmap.top

[D11] 反转数组
来源：http://tva.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://oxk.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://zql.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://khd.vqdsnc.cn

TS:   [...arr].reverse();
来源：http://rxz.fehbvm.com

Java: Collections.reverse(list);
来源：http://qwu.zhongyouzk.top

Go:   slices.Reverse(arr)
来源：http://kun.xuetiantiany.cn

Ruby: arr.reverse
来源：http://puq.hnxiangtu.top

C#:   list.Reverse();
来源：http://yfn.bbcook.cn

[D12] 查找元素下标
来源：http://cgo.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://vee.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tsb.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ira.pycfn.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qtp.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hkb.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://fpx.shuidangran.top

Ruby: arr.index(x)
来源：http://qfi.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://ekh.52xcode.cn

[D13] 过滤（保留满足条件的）
来源：http://cza.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xxm.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://suc.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://snj.hesvh.cn

TS:   arr.filter(x => x > 3)
来源：http://zbz.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fms.yanxiufei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xjv.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://myj.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ccf.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://wqc.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xkf.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aqr.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://ryy.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://gsl.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ckx.sjlbkw.cn

Go:   // 手写循环
来源：http://nfn.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fle.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://rih.hnxiangtu.top

[D15] 去重
来源：http://xvy.ppjwa.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tvd.svipenyu.cn

PHP:  array_unique($arr);
来源：http://int.epnwcf.com

JS:   [...new Set(arr)]
来源：http://ytx.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://zrs.fktsv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qyb.0kj1m.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oms.sufxvd.cn

Ruby: arr.uniq
来源：http://ouc.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://qic.ivvv.top

[D16] 求和与平均值
来源：http://uop.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xdi.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cff.xingfuxueyuan.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cif.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uvv.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lov.hywenlv.cn

Go:   // 手写循环累加
来源：http://zab.yongpay.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vbj.yangfankeji.com

C#:   list.Sum();  list.Average()
来源：http://ijo.guowangkeji.top

[D17] 最大值与最小值
来源：http://zzg.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://eht.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://qwh.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://edx.zhaomingkeji.xyz

TS:   Math.max(...arr);
来源：http://avw.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vic.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uzb.ivvv.top

Ruby: arr.max;  arr.min
来源：http://gly.hywenlv.cn

C#:   list.Max();  list.Min()
来源：http://dej.xuetiantiany.cn

[D18] 扁平化嵌套数组
来源：http://jlj.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wbx.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://zmx.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dpu.zhoulong.xyz

TS:   nested.flat();
来源：http://utk.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gyp.tarul.cn

Go:   // 手写双层循环
来源：http://xbm.hcnkem.com

Ruby: nested.flatten
来源：http://ipc.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://lwc.ivvv.top

[D19] 按字段分组
来源：http://ldn.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://str.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bze.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tkg.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eyg.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pvy.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://ajx.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://tip.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yyh.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://std.wangdashe.top

Py:   Counter(arr)
来源：http://cbi.zhixingplan.top

PHP:  array_count_values($arr);
来源：http://ovd.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://klu.gzhubu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rxf.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eyl.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://znf.tian-w.cn

Ruby: arr.tally
来源：http://mbk.redwolf501.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dap.vehdjk.com

[D21] 判断是否包含某元素
来源：http://hlx.aibaodan.cn

Py:   x in arr
来源：http://skz.svipenyu.cn

PHP:  in_array($x, $arr, true);
来源：http://huj.nanxuanxn.top

JS:   arr.includes(x)
来源：http://fzd.sysykeji.top

TS:   arr.includes(x)
来源：http://znp.vehdjk.com

Java: list.contains(x)
来源：http://xiz.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://anp.dianchejie.cn

Ruby: arr.include?(x)
来源：http://oyb.yj202588.top

C#:   list.Contains(x)
来源：http://ijz.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://pyg.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pur.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://njo.fanxiaobao.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hrb.fengsongda.top

TS:   [...arr];
来源：http://ksn.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://hau.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://cco.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://kvm.nanxuanxn.top

C#:   new List<int>(list);
来源：http://nms.yvedp.cn


<!-- 参考信息 -->