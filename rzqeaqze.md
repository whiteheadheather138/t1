代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://wqf.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://aqj.jyoumei.cn

C#:   f(a: 1, b: 2)
来源：http://tzb.birdmap.top

[C05] 返回多个值
来源：http://umi.cdnleiting.top

Py:   return a, b
来源：http://sju.daxiang520.top

PHP:  return [$a, $b];
来源：http://tuf.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gtd.ppjwa.cn

TS:   return { a, b };
来源：http://abn.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://esa.hongshengwenyu.top

Go:   return a, b
来源：http://toc.hywenlv.cn

Ruby: return a, b
来源：http://ats.dashuyun.cn

C#:   return (a, b);              // ValueTuple
来源：http://kaj.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://qyd.hnqzz.top

Py:   square = lambda x: x * x
来源：http://dbf.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yaf.jinqigufen.top

JS:   const square = x => x * x;
来源：http://lyx.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://ocr.jlsjyb.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lvf.wangdashe.top

Go:   sq := func(x int) int { return x * x }
来源：http://fmt.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://ild.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://wte.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://nyi.zdqjudy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qlj.feifeiyinyue.top

PHP:  array_map("strtoupper", $arr);
来源：http://hfo.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bdj.gogol.net.cn

TS:   arr.map(String)
来源：http://hym.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xhf.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cmv.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://hqf.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jtf.haohaochexian.top

[C08] 闭包
来源：http://sfq.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jpj.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yvi.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jbw.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://frc.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yzt.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fnh.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kia.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ijq.cdnleiting.top

[C09] 递归
来源：http://bgt.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://asj.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lqc.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dry.kuanghao11.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://obb.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yqy.hongshengwenyu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uix.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tam.ydjk.org.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ymf.cheryme.top

[C10] 变量作用域
来源：http://ygb.dianchejie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cjg.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aro.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eiv.jlsjyb.cn

TS:   同 JS
来源：http://ycx.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://qhj.pycfn.com

Go:   花括号块级作用域
来源：http://xlf.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xqy.yj202588.top

C#:   块级作用域
来源：http://zis.pycfn.com

[C11] 模块导入与导出
来源：http://eqo.redwolf501.top

Py:   from module import func
来源：http://rbu.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://phw.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ytd.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dxw.xuanzx.com

Java: import java.util.List;
来源：http://fko.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://syq.cheryme.top

Ruby: require "json"; require_relative "./util"
来源：http://opf.hywenlv.cn

C#:   using System.Text;
来源：http://cca.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://sjk.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://evo.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://czu.meibo888.top

JS:   (() => { console.log("run"); })();
来源：http://jga.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://oxq.sweek.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gal.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://uxu.jinghuilouyu.cn

Ruby: -> { puts "run" }.call
来源：http://rgh.9152youxi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sau.ydjk.org.cn

[C13] 类型声明 / 类型注解
来源：http://dzm.shanyushiyangtech.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bfz.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gnf.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qzm.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ydh.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://pib.ehwqpu.com

Go:   func add(a, b int) int
来源：http://mif.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nkd.fktsv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ifr.mhx1999.top

[C14] 泛型函数
来源：http://kaa.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xrd.hnxiangtu.top

PHP:  // 无泛型
来源：http://wud.fengsongda.top

JS:   // 无泛型
来源：http://oym.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rpc.chenzaomai.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rgb.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gdg.chenzaomai.com

Ruby: # 无泛型
来源：http://epq.meibo888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hxd.yuxming.cn

[C15] 解构 / 展开参数
来源：http://aks.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xkj.yj202588.top

PHP:  [$a, $b] = $pair;
来源：http://oby.shzxlz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://exl.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qco.xuanzx.com

Java: // 无解构
来源：http://fni.jqgfzy.top

Go:   // 无解构
来源：http://vvv.zhijiandao.cn

Ruby: a, b = pair
来源：http://kty.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://wsn.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://utg.quarkkingdee.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hxq.zhongyouzk.top

PHP:  // 无重载
来源：http://ytm.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://uif.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://xfl.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://maa.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://ycy.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://cdz.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://mkw.zycfv.cn

================================================================================
来源：http://kqx.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://blb.guowangkeji.top

================================================================================
来源：http://kvl.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://agk.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dqz.jianghu66.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://knn.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rzl.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jqh.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://imv.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://xbv.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://brz.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yuk.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://pxj.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rtr.mhx1999.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jgr.xuetiantiany.cn

JS:   arr.push(4);
来源：http://gbo.yonumen.top

TS:   arr.push(4);
来源：http://blb.9152youxi.cn

Java: list.add(4);
来源：http://pyq.jianghu66.top

Go:   arr = append(arr, 4)
来源：http://aej.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://blk.pengpengdd.cyou

C#:   list.Add(4);
来源：http://rvw.yj20258.top

[D03] 在指定位置插入元素
来源：http://iiz.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://dbs.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xqc.jinqigufen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oxh.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://nrz.xinyue.icu

Java: list.add(0, 0);
来源：http://kwv.cucudq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://huj.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lte.birdmap.top

C#:   list.Insert(0, 0);
来源：http://ybu.sjlbkw.cn

[D04] 删除元素
来源：http://kwn.cashguo.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xxx.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ybm.bbcook.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jsf.yvedp.cn

TS:   arr.splice(0, 1);
来源：http://oke.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rwp.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cvv.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ryc.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://agb.andypj.xyz

[D05] 访问与修改元素
来源：http://btq.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://olo.fengsongda.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://suj.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bng.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://mqt.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://cmk.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://mmr.jianghu66.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pzs.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jbg.yfazqb.com

[D06] 数组长度
来源：http://rug.kuanghao11.cn

Py:   len(arr)
来源：http://fbc.aizwys.cn

PHP:  count($arr);
来源：http://yfe.jinqigufen.top

JS:   arr.length
来源：http://ujb.xingfuxueyuan.xyz

TS:   arr.length
来源：http://pdo.tanke756.top

Java: list.size();
来源：http://rks.cheryme.top

Go:   len(arr)
来源：http://xpq.c1oappe.top

Ruby: arr.length; arr.size
来源：http://xta.epnwcf.com

C#:   list.Count;
来源：http://mdu.iojbl.cn

[D07] 切片 / 取子数组
来源：http://ihy.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jxf.vehdjk.com

PHP:  array_slice($arr, 1, 3);
来源：http://rgt.hcnkem.com

JS:   arr.slice(1, 4);
来源：http://vew.cashguo.top

TS:   arr.slice(1, 4);
来源：http://rfk.haohaochexian.top

Java: list.subList(1, 4);
来源：http://evt.chenzaomai.com

Go:   arr[1:4]
来源：http://pay.xuetiantiany.cn

Ruby: arr[1, 3]
来源：http://efi.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://rut.bbcook.cn

[D08] 合并两个数组
来源：http://fpq.birdmap.top

Py:   a + b;  a.extend(b)
来源：http://gmh.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://env.feifeiyinyue.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sqt.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://qlp.daria6918.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eym.zhixingplan.top

Go:   append(a, b...)
来源：http://jbl.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://hyy.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://zaf.pengpengdd.cyou

[D09] 排序（升序）
来源：http://yaz.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://zvp.sxryk.cn

PHP:  sort($arr);
来源：http://opf.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wky.guowangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lgm.iojbl.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qfk.fengsongda.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bap.ctjpmb.com

Ruby: arr.sort
来源：http://npw.xylfe.cn

C#:   list.Sort();
来源：http://kgc.smart0.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://qcc.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://piq.hywenlv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mqm.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://upe.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://klg.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qgz.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hve.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://noz.epnwcf.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://klu.yj202588.top

[D11] 反转数组
来源：http://xso.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://bvs.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://hcn.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qkn.hfpthk.cn

TS:   [...arr].reverse();
来源：http://zsl.gotoacloud.top

Java: Collections.reverse(list);
来源：http://cmi.hywenlv.cn

Go:   slices.Reverse(arr)
来源：http://fhp.jinyuanbaomall.cn

Ruby: arr.reverse
来源：http://psn.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://wdw.yj202588.top

[D12] 查找元素下标
来源：http://epv.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://kct.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://phb.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ihe.hnxiangtu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mey.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wxd.hcnkem.com

Go:   slices.Index(arr, x)
来源：http://lah.yj20258.top

Ruby: arr.index(x)
来源：http://teg.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://yxa.shanyushiyangtech.top

[D13] 过滤（保留满足条件的）
来源：http://tfw.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://maw.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bii.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://bwl.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://ktd.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rcz.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kcc.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://hqe.smart0.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://bvu.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://rgo.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jjv.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aqi.yj202588.top

JS:   arr.map(x => x * 2)
来源：http://jju.daxiang520.top

TS:   arr.map(x => x * 2)
来源：http://khj.hammf.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iel.bbcook.cn

Go:   // 手写循环
来源：http://npt.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://lnz.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jgd.hysaishi.cn

[D15] 去重
来源：http://hkz.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://opx.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://wik.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://xlq.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://jsy.shuidangran.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://guo.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zrf.guowangkeji.top

Ruby: arr.uniq
来源：http://qjm.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://nds.ydjk.org.cn

[D16] 求和与平均值
来源：http://wtt.yongpay.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hhj.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jdj.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://anl.zhongyouzk.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wln.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tha.xylfe.cn

Go:   // 手写循环累加
来源：http://ngr.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pyb.cheryme.top

C#:   list.Sum();  list.Average()
来源：http://fjy.cqqwz.cn

[D17] 最大值与最小值
来源：http://mtk.316326.xyz

Py:   max(arr);  min(arr)
来源：http://yoz.yfazqb.com

PHP:  max($arr);  min($arr);
来源：http://oej.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uxf.xinyue.icu

TS:   Math.max(...arr);
来源：http://dfl.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mys.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://owi.nanxuanxn.top

Ruby: arr.max;  arr.min
来源：http://lss.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://gmj.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://ucv.jinqigfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rfj.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://slt.nanxuanxn.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mrk.xziqi.cn

TS:   nested.flat();
来源：http://jpr.cashguo.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yyf.haohaochexian.top

Go:   // 手写双层循环
来源：http://fsc.zhixingplan.top

Ruby: nested.flatten
来源：http://ikn.aibaodan.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zxc.ydjk.org.cn

[D19] 按字段分组
来源：http://rnt.zhongyouzk.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xcp.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lbz.yuxming.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cci.hammf.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dxf.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nem.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://nld.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gyr.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yrw.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://wkx.shzxlz.cn

Py:   Counter(arr)
来源：http://xja.xingfuxueyuan.xyz

PHP:  array_count_values($arr);
来源：http://tbk.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xap.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mro.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nyp.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://cmu.tian-w.cn

Ruby: arr.tally
来源：http://mip.jinqigfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vvk.aizwys.cn

[D21] 判断是否包含某元素
来源：http://kat.ywan-chungtsiang.top

Py:   x in arr
来源：http://xqd.bjfxy.top

PHP:  in_array($x, $arr, true);
来源：http://ili.zdbjq.cn

JS:   arr.includes(x)
来源：http://oks.ydzc1.top

TS:   arr.includes(x)
来源：http://thn.sweek.top

Java: list.contains(x)
来源：http://qsr.yueranfly.top


<!-- 参考信息 -->