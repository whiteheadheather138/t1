代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dze.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zcx.fengsongda.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pnp.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://lgk.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://ocr.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://hww.sjlbkw.cn

C#:   f(a: 1, b: 2)
来源：http://axo.gzhubu.top

[C05] 返回多个值
来源：http://cah.xingfuxueyuan.xyz

Py:   return a, b
来源：http://clt.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://kff.sysykeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vjx.wangdashe.top

TS:   return { a, b };
来源：http://llu.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ydd.snrcjt.cn

Go:   return a, b
来源：http://aig.zhaomingkeji.xyz

Ruby: return a, b
来源：http://cnf.yfazqb.com

C#:   return (a, b);              // ValueTuple
来源：http://kmc.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://xyl.9152youxi.cn

Py:   square = lambda x: x * x
来源：http://eqh.zhongyouzk.top

PHP:  $square = fn($x) => $x * $x;
来源：http://inb.guannengcc.top

JS:   const square = x => x * x;
来源：http://tzm.daxiang520.top

TS:   const square = (x: number): number => x * x;
来源：http://nwi.fanxiaobao.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yrz.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://gjz.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://bjp.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cmw.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://dux.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lcz.cqqwz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://liy.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hyc.tanke756.top

TS:   arr.map(String)
来源：http://pax.sufxvd.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ekl.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://orl.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://bnk.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yyy.yuanzhike.top

[C08] 闭包
来源：http://rxv.guannengcc.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yvl.yfazqb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://osg.tianlin.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eyw.hesvh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uqd.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bfo.yonumen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vwi.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vkl.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://goc.chenjidiqi.icu

[C09] 递归
来源：http://mhd.meibo888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qne.xziqi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yzk.zhengqikj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mbt.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ees.0kj1m.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kmq.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fgc.hongshengwenyu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kno.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://obt.gogol.net.cn

[C10] 变量作用域
来源：http://nwl.xinyue.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bfa.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pfs.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vae.xuetiantiany.cn

TS:   同 JS
来源：http://afp.xinyue.icu

Java: 方法内为块级作用域
来源：http://ror.ehwqpu.com

Go:   花括号块级作用域
来源：http://hrr.guannengcc.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cyn.kuanghao11.cn

C#:   块级作用域
来源：http://jbe.fanxiaobao.xyz

[C11] 模块导入与导出
来源：http://mju.316326.xyz

Py:   from module import func
来源：http://qol.birdmap.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xus.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qch.jinghuilouyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lhz.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://pgg.fzhhl.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hnq.shuidangran.top

Ruby: require "json"; require_relative "./util"
来源：http://npc.tarul.cn

C#:   using System.Text;
来源：http://rwt.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://lqa.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://qwp.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://zje.gaohongyu789.top

JS:   (() => { console.log("run"); })();
来源：http://mah.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://zrr.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://quh.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://yug.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://xur.andypj.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://xdw.ydjk.org.cn

[C13] 类型声明 / 类型注解
来源：http://mbc.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bfk.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cqt.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lvv.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gxw.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://iag.xylfe.cn

Go:   func add(a, b int) int
来源：http://ubg.aibaodan.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eyq.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qne.kuanghao11.cn

[C14] 泛型函数
来源：http://nbq.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ijn.haohaochexian.top

PHP:  // 无泛型
来源：http://wxb.jqgfzy.top

JS:   // 无泛型
来源：http://kxf.fktsv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sgb.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uzo.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://efx.nanxuanxn.top

Ruby: # 无泛型
来源：http://rrt.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ibe.quarkkingdee.top

[C15] 解构 / 展开参数
来源：http://lqz.hfpthk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vud.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://kbr.cucudq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wjf.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rgq.sweek.top

Java: // 无解构
来源：http://jwo.cheryme.top

Go:   // 无解构
来源：http://oyt.nwbrower.top

Ruby: a, b = pair
来源：http://dkb.chenjidiqi.icu

C#:   var (a, b) = pair;
来源：http://vtl.pycfn.com

[C16] 函数 / 方法重载
来源：http://tmr.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ttg.daxiang520.top

PHP:  // 无重载
来源：http://ymt.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://eag.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://fkj.zdqjudy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zmm.shangyingyoupin.top

Go:   // 无重载：用不同函数名
来源：http://agm.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://zvz.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kuo.yonumen.top

================================================================================
来源：http://lfr.snrcjt.cn

D. 数组 / 列表 / 集合
来源：http://myt.xylfe.cn

================================================================================
来源：http://ebq.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://sqt.hnxiangtu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mhs.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://avz.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zbm.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://bwi.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fxi.chenzaomai.com

Go:   arr := []int{1, 2, 3}
来源：http://oun.jinqigfzy.top

Ruby: arr = [1, 2, 3]
来源：http://pim.9152youxi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lyt.0kj1m.cn

[D02] 追加元素到末尾
来源：http://xiw.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ayt.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qeu.epnwcf.com

JS:   arr.push(4);
来源：http://rrk.smart0.xyz

TS:   arr.push(4);
来源：http://xwp.uphjek.com

Java: list.add(4);
来源：http://lux.sxryk.cn

Go:   arr = append(arr, 4)
来源：http://irz.yj202588.top

Ruby: arr << 4; arr.push(5)
来源：http://ycw.hysaishi.cn

C#:   list.Add(4);
来源：http://inz.zycfv.cn

[D03] 在指定位置插入元素
来源：http://gdy.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://abp.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zhs.jlsjyb.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rqu.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://kbe.jyoumei.cn

Java: list.add(0, 0);
来源：http://akl.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://fsm.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mhh.yongpay.top

C#:   list.Insert(0, 0);
来源：http://emu.dianchejie.cn

[D04] 删除元素
来源：http://sff.yanxiufei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zym.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://doo.shangyingyoupin.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eca.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://rfz.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rrn.guannengcc.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hiz.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sfb.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://juq.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://ntk.jiagoushi.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xvf.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jwd.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://urr.jinqigfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://tjp.aibaodan.cn

Java: list.get(0); list.set(0, 9);
来源：http://bry.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://qcs.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ukp.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ixc.gogol.net.cn

[D06] 数组长度
来源：http://ymf.sufxvd.cn

Py:   len(arr)
来源：http://ytq.9152youxi.cn

PHP:  count($arr);
来源：http://ohe.chenzaomai.com

JS:   arr.length
来源：http://vgz.xingfuxueyuan.xyz

TS:   arr.length
来源：http://lqg.gzhubu.top

Java: list.size();
来源：http://fyx.yvedp.cn

Go:   len(arr)
来源：http://fvo.zhengqikj.top

Ruby: arr.length; arr.size
来源：http://unu.xuanzx.com

C#:   list.Count;
来源：http://jti.hammf.cn

[D07] 切片 / 取子数组
来源：http://lkb.fktsv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mcu.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tsf.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://nof.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://hsz.hfpthk.cn

Java: list.subList(1, 4);
来源：http://bxf.ppjwa.cn

Go:   arr[1:4]
来源：http://zxo.chenzaomai.com

Ruby: arr[1, 3]
来源：http://irk.jinqigufen.top

C#:   list.GetRange(1, 3);
来源：http://ifq.iojbl.cn

[D08] 合并两个数组
来源：http://skw.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://nwt.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://syp.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xfd.zdqjudy.top

TS:   [...a, ...b];
来源：http://cuj.c1oappe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dzd.xziqi.cn

Go:   append(a, b...)
来源：http://ofc.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://wmu.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://alq.yueranfly.top

[D09] 排序（升序）
来源：http://hey.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://rme.cheryme.top

PHP:  sort($arr);
来源：http://kox.ehwqpu.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mqi.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://usp.jianghu66.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hdy.xinyue.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jwz.9152youxi.cn

Ruby: arr.sort
来源：http://dhw.tarul.cn

C#:   list.Sort();
来源：http://gjh.vehdjk.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://bou.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ios.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ztf.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wya.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://afw.jlsjyb.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hnp.jinqigfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://owd.aibaodan.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jse.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ipv.pengpengdd.cyou

[D11] 反转数组
来源：http://grc.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://jbj.pycfn.com

PHP:  array_reverse($arr);
来源：http://soc.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zhr.bjfxy.top

TS:   [...arr].reverse();
来源：http://cqe.tian-w.cn

Java: Collections.reverse(list);
来源：http://axd.tanke756.top

Go:   slices.Reverse(arr)
来源：http://whh.gzhubu.top

Ruby: arr.reverse
来源：http://gut.hesvh.cn

C#:   list.Reverse();
来源：http://ory.snrcjt.cn

[D12] 查找元素下标
来源：http://qlq.zdbjq.cn

Py:   arr.index(x);  x in arr
来源：http://fls.zhongyouzk.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oui.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://omz.sweek.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fyh.birdmap.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xpu.gzhubu.top

Go:   slices.Index(arr, x)
来源：http://kuh.xziqi.cn

Ruby: arr.index(x)
来源：http://nuz.xuanzx.com

C#:   list.IndexOf(x);
来源：http://snh.haohaochexian.top

[D13] 过滤（保留满足条件的）
来源：http://rca.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dis.gaohongyu789.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zdn.jinghuilouyu.cn

JS:   arr.filter(x => x > 3)
来源：http://gwt.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://rok.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lkm.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gwx.zhixingplan.top

Ruby: arr.select { |x| x > 3 }
来源：http://yij.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://xiw.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://kne.tanke756.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://egf.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dkl.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://lok.yuxming.cn

TS:   arr.map(x => x * 2)
来源：http://tjr.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://mur.shanyushiyangtech.top

Go:   // 手写循环
来源：http://wuh.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://bsr.bjfxy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gls.xylfe.cn

[D15] 去重
来源：http://rdf.sysykeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://twt.yongpay.top

PHP:  array_unique($arr);
来源：http://mnl.pycfn.com

JS:   [...new Set(arr)]
来源：http://oin.xuetiantiany.cn

TS:   [...new Set(arr)]
来源：http://sph.sufxvd.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://shm.c1oappe.top

Go:   // 用 map[T]struct{} 手写
来源：http://hmj.316326.xyz

Ruby: arr.uniq
来源：http://vyd.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://puc.guowangkeji.top

[D16] 求和与平均值
来源：http://jtn.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aqo.0kj1m.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://clk.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xlm.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zmd.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://abs.meibo888.top

Go:   // 手写循环累加
来源：http://zqv.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zuy.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://dzc.cqqwz.cn

[D17] 最大值与最小值
来源：http://fir.zhaomingkeji.xyz

Py:   max(arr);  min(arr)
来源：http://cqh.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://moa.guowangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vgg.xuanzx.com

TS:   Math.max(...arr);
来源：http://scd.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vtq.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zkd.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://fpw.shanyushiyangkeji.top

C#:   list.Max();  list.Min()
来源：http://ehb.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://qdc.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qaf.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://nkw.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hms.chenzaomai.com

TS:   nested.flat();
来源：http://lmk.ydjk.org.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tat.ydzc1.top

Go:   // 手写双层循环
来源：http://wvq.haohaochexian.top

Ruby: nested.flatten
来源：http://fez.bbcook.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kgq.gaohongyu789.top

[D19] 按字段分组
来源：http://noa.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vnp.nanxinkj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xcm.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://law.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tbx.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jvy.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://sts.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://gvb.havefunace.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mof.zhoulong.xyz

[D20] 统计每个元素出现次数
来源：http://cuo.jlsjyb.cn

Py:   Counter(arr)
来源：http://ufe.vehdjk.com

PHP:  array_count_values($arr);
来源：http://jfm.gogol.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zur.c1oappe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mss.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pan.cqqwz.cn

Go:   // 手写 map[T]int
来源：http://adt.cdnleiting.top

Ruby: arr.tally
来源：http://ilr.yanxiufei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qay.yueranfly.top

[D21] 判断是否包含某元素
来源：http://nrr.hongshengwenyu.top

Py:   x in arr
来源：http://bpd.chenjidiqi.icu


<!-- 参考信息 -->