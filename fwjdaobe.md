代发 wailian999

Py:   return a, b
来源：http://auu.xuanzx.com

PHP:  return [$a, $b];
来源：http://zpb.guannengcc.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nqw.zhoulong.xyz

TS:   return { a, b };
来源：http://xkz.uphjek.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bul.epnwcf.com

Go:   return a, b
来源：http://lpi.cdnleiting.top

Ruby: return a, b
来源：http://lti.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://sar.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://jnq.daxiang520.top

Py:   square = lambda x: x * x
来源：http://tfw.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aed.ehwqpu.com

JS:   const square = x => x * x;
来源：http://ots.ppjwa.cn

TS:   const square = (x: number): number => x * x;
来源：http://hic.ctjpmb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eee.tianlin.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://mxn.redwolf501.top

Ruby: square = ->(x) { x * x }
来源：http://ggd.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bkl.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://qkp.hfpthk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hoy.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://suo.jinqigfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bmp.tianlin.xyz

TS:   arr.map(String)
来源：http://you.sufxvd.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://twk.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://voc.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://bjb.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cno.vqdsnc.cn

[C08] 闭包
来源：http://feq.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://spr.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lgz.fanxiaobao.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://izd.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qzl.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pdu.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://llb.uphjek.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gba.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kaf.redwolf501.top

[C09] 递归
来源：http://uci.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://acy.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://geu.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://thu.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vsv.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jue.iojbl.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rdd.tanke756.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sry.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sid.hnxiangtu.top

[C10] 变量作用域
来源：http://cim.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://txx.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sox.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://msr.yj20258888.top

TS:   同 JS
来源：http://oix.ppjwa.cn

Java: 方法内为块级作用域
来源：http://cyo.yangfankeji.com

Go:   花括号块级作用域
来源：http://pga.epnwcf.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pnf.tarul.cn

C#:   块级作用域
来源：http://kkc.ydjk.org.cn

[C11] 模块导入与导出
来源：http://pdg.dianchejie.cn

Py:   from module import func
来源：http://hoa.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ryx.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gkh.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://stv.yuanzhike.top

Java: import java.util.List;
来源：http://ejr.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uxk.zhijiandao.cn

Ruby: require "json"; require_relative "./util"
来源：http://twt.jianghu66.top

C#:   using System.Text;
来源：http://ggz.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://aid.jqgfzy.top

Py:   (lambda: print("run"))()
来源：http://dye.nanxuanxn.top

PHP:  (function () { echo "run"; })();
来源：http://dpr.shanyushiyangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://dxm.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://wqm.tian-w.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ixn.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://huw.wangshuangyany.cn

Ruby: -> { puts "run" }.call
来源：http://xyq.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xwv.ydzc1.top

[C13] 类型声明 / 类型注解
来源：http://qtj.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wyv.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bnm.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://buw.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wus.fzhhl.top

Java: int add(int a, int b) { return a + b; }
来源：http://odw.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://dta.daria6918.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mlm.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://qqq.fanxiaobao.xyz

[C14] 泛型函数
来源：http://eqs.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://odu.sufxvd.cn

PHP:  // 无泛型
来源：http://lge.xuetiantiany.cn

JS:   // 无泛型
来源：http://gbk.redwolf501.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pwx.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zlv.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vhx.pengpengdd.cyou

Ruby: # 无泛型
来源：http://mwu.sysykeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nrm.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://oui.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fbz.snrcjt.cn

PHP:  [$a, $b] = $pair;
来源：http://yvu.fanxiaobao.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xuj.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vjk.havefunace.top

Java: // 无解构
来源：http://kol.yvedp.cn

Go:   // 无解构
来源：http://eep.jiagoushi.top

Ruby: a, b = pair
来源：http://xoq.daxiang520.top

C#:   var (a, b) = pair;
来源：http://ajb.aibaodan.cn

[C16] 函数 / 方法重载
来源：http://xuj.svipenyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kms.hongshengwenyu.top

PHP:  // 无重载
来源：http://jth.dianchejie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hbj.zdqjudy.top

TS:   // 用联合类型或重载签名声明
来源：http://ofp.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nia.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://lia.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://qvh.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fct.yongpay.top

================================================================================
来源：http://dpf.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://opb.yvedp.cn

================================================================================
来源：http://liy.jiagoushi.top

[D01] 创建数组 / 列表
来源：http://jwe.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://jui.sweek.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vzh.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mta.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fpu.smart0.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mco.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://irn.hcnkem.com

Ruby: arr = [1, 2, 3]
来源：http://wpo.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vhz.hesvh.cn

[D02] 追加元素到末尾
来源：http://nra.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bci.andypj.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ddn.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://axp.vqdsnc.cn

TS:   arr.push(4);
来源：http://yam.gogol.net.cn

Java: list.add(4);
来源：http://aob.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://nxo.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://fla.cheryme.top

C#:   list.Add(4);
来源：http://kaa.cashguo.top

[D03] 在指定位置插入元素
来源：http://lfa.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://bzf.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gun.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://adv.zhiwuduotai.top

TS:   arr.splice(0, 0, 0);
来源：http://eqf.guannengcc.top

Java: list.add(0, 0);
来源：http://feg.wangdashe.top

Go:   arr = append([]int{0}, arr...)
来源：http://dtp.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ncm.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://agi.yfazqb.com

[D04] 删除元素
来源：http://cud.yvedp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cxt.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://caj.yj20258.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nnh.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://hqg.hcnkem.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pnp.tanke756.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jbd.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zbx.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kkr.shzxlz.cn

[D05] 访问与修改元素
来源：http://iun.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://scn.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wtz.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cjt.snrcjt.cn

TS:   arr[0]; arr.at(-1);
来源：http://odb.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://oqk.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://smu.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zqj.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zbs.meibo888.top

[D06] 数组长度
来源：http://fve.pengpengdd.cyou

Py:   len(arr)
来源：http://ibz.yuxming.cn

PHP:  count($arr);
来源：http://rbi.daxiang520.top

JS:   arr.length
来源：http://srz.hywenlv.cn

TS:   arr.length
来源：http://zns.gotoacloud.top

Java: list.size();
来源：http://vua.smart0.xyz

Go:   len(arr)
来源：http://iro.tian-w.cn

Ruby: arr.length; arr.size
来源：http://ttu.redwolf501.top

C#:   list.Count;
来源：http://rau.pycfn.com

[D07] 切片 / 取子数组
来源：http://cms.gzhubu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kyd.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://jir.yj20258888.top

JS:   arr.slice(1, 4);
来源：http://til.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://ubw.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://pgd.iojbl.cn

Go:   arr[1:4]
来源：http://obf.dashuyun.cn

Ruby: arr[1, 3]
来源：http://url.daria6918.cn

C#:   list.GetRange(1, 3);
来源：http://lhn.guannengcc.top

[D08] 合并两个数组
来源：http://aew.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://seu.ybcxt.top

PHP:  array_merge($a, $b);
来源：http://dmq.redwolf501.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xgj.hnqzz.top

TS:   [...a, ...b];
来源：http://gzj.tian-w.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ksp.ybcxt.top

Go:   append(a, b...)
来源：http://cyg.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://ftf.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://toz.guannengcc.top

[D09] 排序（升序）
来源：http://cmb.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://qip.ydzc1.top

PHP:  sort($arr);
来源：http://fye.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nua.cqqwz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://asu.cdnleiting.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dwl.fktsv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vlw.sysykeji.top

Ruby: arr.sort
来源：http://eum.ydzc1.top

C#:   list.Sort();
来源：http://kai.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://agu.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://stq.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zhf.yuxming.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qfa.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://clb.mhx1999.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kkc.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ejv.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ngu.gogol.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vbi.sxryk.cn

[D11] 反转数组
来源：http://ivl.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://eej.zhiwuduotai.top

PHP:  array_reverse($arr);
来源：http://oxe.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bqg.aizwys.cn

TS:   [...arr].reverse();
来源：http://fup.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://fbw.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://ykw.yangfankeji.com

Ruby: arr.reverse
来源：http://fah.hnqzz.top

C#:   list.Reverse();
来源：http://ter.316326.xyz

[D12] 查找元素下标
来源：http://dux.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://inp.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://age.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vvw.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ady.kuanghao11.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://moa.nanxuanxn.top

Go:   slices.Index(arr, x)
来源：http://ezi.yonumen.top

Ruby: arr.index(x)
来源：http://idq.daria6918.cn

C#:   list.IndexOf(x);
来源：http://jpo.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://bvv.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pxf.fktsv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://stg.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://xqe.yueranfly.top

TS:   arr.filter(x => x > 3)
来源：http://znz.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sog.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ial.daxiang520.top

Ruby: arr.select { |x| x > 3 }
来源：http://zes.uphjek.com

C#:   list.Where(x => x > 3).ToList()
来源：http://uhs.meibo888.top

[D14] 映射转换（每个元素变形）
来源：http://eso.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yhp.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uti.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://stn.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://fxe.gaohongyu789.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wif.yanxiufei.cn

Go:   // 手写循环
来源：http://nvw.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://zkj.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kdt.jinyuanbaomall.cn

[D15] 去重
来源：http://iwe.sysykeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cyk.bjfxy.top

PHP:  array_unique($arr);
来源：http://nry.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://oid.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://pqd.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ddk.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://vkw.sufxvd.cn

Ruby: arr.uniq
来源：http://pek.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://kzq.yvedp.cn

[D16] 求和与平均值
来源：http://vcj.jinqigfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://buz.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rtm.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qfv.0kj1m.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://glz.hesvh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cdc.yonumen.top

Go:   // 手写循环累加
来源：http://hvn.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lyz.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://ytw.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://fhn.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://pid.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://vhy.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xkp.havefunace.top

TS:   Math.max(...arr);
来源：http://fzb.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://fst.smart0.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dnf.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://zrn.yfazqb.com

C#:   list.Max();  list.Min()
来源：http://vqa.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://vbk.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ofj.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://dny.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hev.jinqigufen.top

TS:   nested.flat();
来源：http://jvc.shanyushiyangtech.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xmi.redwolf501.top

Go:   // 手写双层循环
来源：http://lze.nwbrower.top

Ruby: nested.flatten
来源：http://ttb.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jxp.pycfn.com

[D19] 按字段分组
来源：http://wnn.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kbx.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://scw.feifeiyinyue.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zzn.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://abw.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ney.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://kro.shangyingyoupin.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ztw.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pch.zhixingplan.top

[D20] 统计每个元素出现次数
来源：http://bny.aizwys.cn

Py:   Counter(arr)
来源：http://zvn.daria6918.cn

PHP:  array_count_values($arr);
来源：http://xiu.tanke756.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://akv.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qet.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dig.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://ick.chenlongwang.top

Ruby: arr.tally
来源：http://pvz.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yut.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://xey.hcnkem.com

Py:   x in arr
来源：http://xvf.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://iez.cheryme.top

JS:   arr.includes(x)
来源：http://zyh.xuanzx.com

TS:   arr.includes(x)
来源：http://bgs.xuanzx.com

Java: list.contains(x)
来源：http://lom.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://hap.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://ocb.shzxlz.cn

C#:   list.Contains(x)
来源：http://abg.wangshuangyany.cn

[D22] 复制数组（避免共享引用）
来源：http://bjf.iojbl.cn


<!-- 参考信息 -->