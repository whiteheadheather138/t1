代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tny.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vzd.0kj1m.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gxo.cashguo.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tpy.yfazqb.com

Ruby: def total(*nums); nums.sum; end
来源：http://fno.quarkkingdee.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://otr.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://ixd.bjfxy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mit.tanke756.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sub.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ppb.chenzaomai.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wcx.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://hli.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://akj.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://gmg.cdnleiting.top

C#:   f(a: 1, b: 2)
来源：http://frt.shuidangran.top

[C05] 返回多个值
来源：http://dvh.chenzaomai.com

Py:   return a, b
来源：http://lqx.zhixingplan.top

PHP:  return [$a, $b];
来源：http://iup.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lye.zdqjudy.top

TS:   return { a, b };
来源：http://kxk.cashguo.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gzs.ehwqpu.com

Go:   return a, b
来源：http://ptk.ybcxt.top

Ruby: return a, b
来源：http://ney.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://vhd.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://pmh.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://uiz.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jdd.sxryk.cn

JS:   const square = x => x * x;
来源：http://hhp.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://jzk.xingfuxueyuan.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ydq.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fhi.gzhubu.top

Ruby: square = ->(x) { x * x }
来源：http://rsc.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://ihz.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://qya.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://igt.haohaochexian.top

PHP:  array_map("strtoupper", $arr);
来源：http://bnv.sjlbkw.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bvz.52xcode.cn

TS:   arr.map(String)
来源：http://tfo.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jlc.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ymj.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://baw.9152youxi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ove.haohaochexian.top

[C08] 闭包
来源：http://dzc.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dwg.aizwys.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jvi.dashuyun.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ifi.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qdf.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ilq.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uzm.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dlt.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cjs.yonumen.top

[C09] 递归
来源：http://ols.yuanzhike.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rxh.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oev.cheryme.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://suc.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nel.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nnk.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mye.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://epr.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rim.fzhhl.top

[C10] 变量作用域
来源：http://mlp.tanke756.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fdy.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uhp.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ksi.zycfv.cn

TS:   同 JS
来源：http://lly.hcnkem.com

Java: 方法内为块级作用域
来源：http://qim.cdnleiting.top

Go:   花括号块级作用域
来源：http://rmk.sysykeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xlv.smart0.xyz

C#:   块级作用域
来源：http://fnz.wangdashe.top

[C11] 模块导入与导出
来源：http://uhq.jqgfzy.top

Py:   from module import func
来源：http://suw.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eyd.bbcook.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xle.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pkh.smart0.xyz

Java: import java.util.List;
来源：http://yym.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hhg.zhengqikj.top

Ruby: require "json"; require_relative "./util"
来源：http://cne.hnxiangtu.top

C#:   using System.Text;
来源：http://gdg.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://ida.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://tbb.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://mur.hysaishi.cn

JS:   (() => { console.log("run"); })();
来源：http://fli.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://hkl.smart0.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jjc.tian-w.cn

Go:   func() { fmt.Println("run") }()
来源：http://vhx.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://zrr.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://khj.ybcxt.top

[C13] 类型声明 / 类型注解
来源：http://hzx.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ydf.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pwv.shzxlz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eoh.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cdm.chenlongwang.top

Java: int add(int a, int b) { return a + b; }
来源：http://wvh.bbcook.cn

Go:   func add(a, b int) int
来源：http://lmr.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qyr.guannengcc.top

C#:   int Add(int a, int b) => a + b;
来源：http://zkx.sufxvd.cn

[C14] 泛型函数
来源：http://dzy.dashuyun.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fzr.yfazqb.com

PHP:  // 无泛型
来源：http://fqk.ehwqpu.com

JS:   // 无泛型
来源：http://koa.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hjq.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vjc.ppjwa.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ydq.yongpay.top

Ruby: # 无泛型
来源：http://grr.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bca.nwbrower.top

[C15] 解构 / 展开参数
来源：http://xbj.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://idh.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://rnv.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://srn.xylfe.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kml.bbcook.cn

Java: // 无解构
来源：http://cyk.yongpay.top

Go:   // 无解构
来源：http://wkl.jianghu66.top

Ruby: a, b = pair
来源：http://tnv.fanxiaobao.xyz

C#:   var (a, b) = pair;
来源：http://odp.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://feo.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dol.jyoumei.cn

PHP:  // 无重载
来源：http://hur.c1oappe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rnt.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://duv.jinyuanbaomall.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://edd.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://xwx.pengpengdd.cyou

Ruby: # 无重载：靠动态参数
来源：http://qmy.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gmz.nanxuanxn.top

================================================================================
来源：http://qqp.guowangkeji.top

D. 数组 / 列表 / 集合
来源：http://eqk.shangyingyoupin.top

================================================================================
来源：http://qeb.fengsongda.top

[D01] 创建数组 / 列表
来源：http://kgh.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://hov.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ipa.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://aew.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qhi.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hgy.gotoacloud.top

Go:   arr := []int{1, 2, 3}
来源：http://nce.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://lpi.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fxx.zycfv.cn

[D02] 追加元素到末尾
来源：http://anx.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lef.ivvv.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kfy.cashguo.top

JS:   arr.push(4);
来源：http://mak.ydjk.org.cn

TS:   arr.push(4);
来源：http://pfs.svipenyu.cn

Java: list.add(4);
来源：http://nbn.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://tbp.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://aty.nanxuanxn.top

C#:   list.Add(4);
来源：http://vso.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://wbl.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://xrr.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://llk.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vcw.jianghu66.top

TS:   arr.splice(0, 0, 0);
来源：http://ofn.9152youxi.cn

Java: list.add(0, 0);
来源：http://tza.cucudq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gyh.uphjek.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oim.jinghuilouyu.cn

C#:   list.Insert(0, 0);
来源：http://ulc.gotoacloud.top

[D04] 删除元素
来源：http://mef.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ryj.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jdo.hammf.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bkh.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://oqi.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fyr.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bqi.chenjidiqi.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lzy.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cvs.fktsv.cn

[D05] 访问与修改元素
来源：http://haw.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://emn.jiagoushi.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uyy.bjfxy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cvb.hnqzz.top

TS:   arr[0]; arr.at(-1);
来源：http://dhk.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://dnw.ydjk.org.cn

Go:   arr[0]; arr[0] = 9
来源：http://qej.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hlr.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tnh.gaohongyu789.top

[D06] 数组长度
来源：http://mwk.zhongyouzk.top

Py:   len(arr)
来源：http://sfk.shanyushiyangtech.top

PHP:  count($arr);
来源：http://aer.ctjpmb.com

JS:   arr.length
来源：http://qui.tanke756.top

TS:   arr.length
来源：http://aqq.chenzaomai.com

Java: list.size();
来源：http://gii.hongshengwenyu.top

Go:   len(arr)
来源：http://rnq.ctjpmb.com

Ruby: arr.length; arr.size
来源：http://xaq.tarul.cn

C#:   list.Count;
来源：http://eio.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://zzx.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://noc.fanxiaobao.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://rpv.cheryme.top

JS:   arr.slice(1, 4);
来源：http://zcl.jinghuilouyu.cn

TS:   arr.slice(1, 4);
来源：http://wis.sweek.top

Java: list.subList(1, 4);
来源：http://wjw.yueranfly.top

Go:   arr[1:4]
来源：http://jqk.sxryk.cn

Ruby: arr[1, 3]
来源：http://fyy.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://znv.hongshengwenyu.top

[D08] 合并两个数组
来源：http://zxl.sufxvd.cn

Py:   a + b;  a.extend(b)
来源：http://ewj.yuxming.cn

PHP:  array_merge($a, $b);
来源：http://vek.fktsv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hlh.sxryk.cn

TS:   [...a, ...b];
来源：http://jne.quarkkingdee.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ope.fengsongda.top

Go:   append(a, b...)
来源：http://igb.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://sud.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://uyc.ctjpmb.com

[D09] 排序（升序）
来源：http://haw.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://esp.hcnkem.com

PHP:  sort($arr);
来源：http://niw.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qjz.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://npi.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fxa.hywenlv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aou.cucudq.cn

Ruby: arr.sort
来源：http://ceu.ivvv.top

C#:   list.Sort();
来源：http://oql.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sus.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ecq.aizwys.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jgg.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wii.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dkj.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qhm.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://csa.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hbt.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qne.yj20258.top

[D11] 反转数组
来源：http://msx.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://ayz.xylfe.cn

PHP:  array_reverse($arr);
来源：http://qck.hcnkem.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iru.daria6918.cn

TS:   [...arr].reverse();
来源：http://fwx.cashguo.top

Java: Collections.reverse(list);
来源：http://lyr.yangfankeji.com

Go:   slices.Reverse(arr)
来源：http://qkm.iojbl.cn

Ruby: arr.reverse
来源：http://mch.yanxiufei.cn

C#:   list.Reverse();
来源：http://syi.zhixingplan.top

[D12] 查找元素下标
来源：http://wjf.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://zux.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pzu.fanxiaobao.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://szq.hcnkem.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wga.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qph.yj20258.top

Go:   slices.Index(arr, x)
来源：http://wds.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://mfo.ctjpmb.com

C#:   list.IndexOf(x);
来源：http://rtj.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://nwd.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rdq.sweek.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dcc.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://zjl.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://mhe.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uxv.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://swi.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eqf.aizwys.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ntz.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://uud.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bno.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yej.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://jgx.sysykeji.top

TS:   arr.map(x => x * 2)
来源：http://fsw.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://njy.xinyue.icu

Go:   // 手写循环
来源：http://spr.yvedp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://udg.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nfy.pycfn.com

[D15] 去重
来源：http://owu.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qpi.xziqi.cn

PHP:  array_unique($arr);
来源：http://ivl.jianghu66.top

JS:   [...new Set(arr)]
来源：http://pgj.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://jlf.c1oappe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ydj.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kir.fanxiaobao.xyz

Ruby: arr.uniq
来源：http://exd.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://npy.hongshengwenyu.top

[D16] 求和与平均值
来源：http://imq.zhiwuduotai.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bzs.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rqw.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jzp.zhijiandao.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mpy.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://igo.svipenyu.cn

Go:   // 手写循环累加
来源：http://ios.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://urv.shanyushiyangtech.top

C#:   list.Sum();  list.Average()
来源：http://tqc.ydjk.org.cn

[D17] 最大值与最小值
来源：http://ykg.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://fol.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://kdk.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://scv.chenzaomai.com

TS:   Math.max(...arr);
来源：http://vcx.hysaishi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rnz.jianghu66.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://coj.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://zms.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://tdg.chenjidiqi.icu

[D18] 扁平化嵌套数组
来源：http://gla.nwbrower.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vei.gogol.net.cn

PHP:  array_merge(...$nested);
来源：http://xuq.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://upt.zhixingplan.top

TS:   nested.flat();
来源：http://kit.uphjek.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yja.tanke756.top

Go:   // 手写双层循环
来源：http://mhu.fengsongda.top

Ruby: nested.flatten
来源：http://qiq.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xcb.ydzc1.top

[D19] 按字段分组
来源：http://yrd.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lvu.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://abr.yvedp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vab.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zmh.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tzk.52xcode.cn

Go:   // 手写 map[string][]T
来源：http://deo.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://odq.vqdsnc.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qqa.tian-w.cn

[D20] 统计每个元素出现次数
来源：http://nep.yonumen.top

Py:   Counter(arr)
来源：http://yec.chenlongwang.top

PHP:  array_count_values($arr);
来源：http://jtk.fanxiaobao.xyz


<!-- 参考信息 -->