代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://xnp.chenlongwang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gvh.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://pyk.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vkw.zhiwuduotai.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lhj.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pql.zhijiandao.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://efr.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://nxd.redwolf501.top

Go:   // 无：用配置结构体参数
来源：http://jqz.feifeiyinyue.top

Ruby: f(a: 1, b: 2)
来源：http://qdb.shanyushiyangtech.top

C#:   f(a: 1, b: 2)
来源：http://kxd.hnqzz.top

[C05] 返回多个值
来源：http://hny.shzxlz.cn

Py:   return a, b
来源：http://dcf.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://pyy.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sjm.quarkkingdee.top

TS:   return { a, b };
来源：http://elx.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://egt.hesvh.cn

Go:   return a, b
来源：http://cvh.c1oappe.top

Ruby: return a, b
来源：http://pfx.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://xln.ehwqpu.com

[C06] 匿名函数 / lambda
来源：http://tkb.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://oea.52xcode.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ser.sysykeji.top

JS:   const square = x => x * x;
来源：http://yzd.shuidangran.top

TS:   const square = (x: number): number => x * x;
来源：http://lsj.52xcode.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gdr.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://ugm.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://jgc.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://nqc.daxiang520.top

[C07] 把函数作为参数传入
来源：http://dqy.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ywc.iojbl.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fvj.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hbb.tianlin.xyz

TS:   arr.map(String)
来源：http://xxh.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ybj.yuanzhike.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zxi.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://srv.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oix.yongpay.top

[C08] 闭包
来源：http://cfm.hcnkem.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uou.shangyingyoupin.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yfg.shanyushiyangtech.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://orz.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vnc.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ype.yvedp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ydz.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wnw.zhaomingkeji.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nxq.jinghuilouyu.cn

[C09] 递归
来源：http://yem.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cis.zdqjudy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lxt.chenzaomai.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wbw.gzhubu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://brn.ivvv.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cer.bjfxy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hfn.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ice.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jhb.cqqwz.cn

[C10] 变量作用域
来源：http://elo.dianchejie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kfn.ehwqpu.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://knm.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qxk.sweek.top

TS:   同 JS
来源：http://sjd.yonumen.top

Java: 方法内为块级作用域
来源：http://fkg.meibo888.top

Go:   花括号块级作用域
来源：http://gnr.aizwys.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jrv.yuanzhike.top

C#:   块级作用域
来源：http://axn.svipenyu.cn

[C11] 模块导入与导出
来源：http://sxm.aibaodan.cn

Py:   from module import func
来源：http://faf.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fco.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ltl.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xhy.zdqjudy.top

Java: import java.util.List;
来源：http://uim.bbcook.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bkb.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://mip.zhijiandao.cn

C#:   using System.Text;
来源：http://ltn.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://vtl.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://jnn.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://uiy.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://zfs.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://sfg.iojbl.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zyw.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://mpm.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://qig.nanxinkj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ywk.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://azh.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xvs.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ndi.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ysp.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://svn.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://gsx.ppjwa.cn

Go:   func add(a, b int) int
来源：http://tti.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pto.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://xkk.hnxiangtu.top

[C14] 泛型函数
来源：http://yaq.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bpi.chenzaomai.com

PHP:  // 无泛型
来源：http://mxs.ehwqpu.com

JS:   // 无泛型
来源：http://qbs.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rvx.xylfe.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qxu.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://brq.chenlongwang.top

Ruby: # 无泛型
来源：http://mut.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xjk.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://lba.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dun.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://fxl.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uaa.hfpthk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wzm.svipenyu.cn

Java: // 无解构
来源：http://cge.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://xex.0kj1m.cn

Ruby: a, b = pair
来源：http://bea.birdmap.top

C#:   var (a, b) = pair;
来源：http://xvn.zycfv.cn

[C16] 函数 / 方法重载
来源：http://dlk.redwolf501.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://feg.jqgufenzy.top

PHP:  // 无重载
来源：http://jcm.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hbq.yj202588.top

TS:   // 用联合类型或重载签名声明
来源：http://fud.yanxiufei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vmx.jyoumei.cn

Go:   // 无重载：用不同函数名
来源：http://eou.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://eee.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://yno.sweek.top

================================================================================
来源：http://ujm.52xcode.cn

D. 数组 / 列表 / 集合
来源：http://yxv.316326.xyz

================================================================================
来源：http://puw.52xcode.cn

[D01] 创建数组 / 列表
来源：http://zmb.cucudq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wdc.gaohongyu789.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jtm.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rgy.ppjwa.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gun.tarul.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bww.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://qaf.sjlbkw.cn

Ruby: arr = [1, 2, 3]
来源：http://xul.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wst.gogol.net.cn

[D02] 追加元素到末尾
来源：http://xcz.c1oappe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nsa.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qcv.wangdashe.top

JS:   arr.push(4);
来源：http://giu.meibo888.top

TS:   arr.push(4);
来源：http://cie.cucudq.cn

Java: list.add(4);
来源：http://yko.yonumen.top

Go:   arr = append(arr, 4)
来源：http://vgv.gogol.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://rip.yj20258.top

C#:   list.Add(4);
来源：http://kxu.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://omk.aizwys.cn

Py:   arr.insert(0, 0)
来源：http://iqt.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nhe.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ovh.jlsjyb.cn

TS:   arr.splice(0, 0, 0);
来源：http://cus.svipenyu.cn

Java: list.add(0, 0);
来源：http://tyb.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://xks.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ubu.0kj1m.cn

C#:   list.Insert(0, 0);
来源：http://dsk.birdmap.top

[D04] 删除元素
来源：http://vtp.cheryme.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ktm.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://upk.hcnkem.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://adq.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://fjs.hammf.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kxw.tarul.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lqp.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tcu.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xzb.cdnleiting.top

[D05] 访问与修改元素
来源：http://nhg.wangshuangyany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rjj.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wmd.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gvj.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://dbi.shuidangran.top

Java: list.get(0); list.set(0, 9);
来源：http://vhc.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://juq.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://prx.cucudq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qcu.zdqjudy.top

[D06] 数组长度
来源：http://pou.nanxuanxn.top

Py:   len(arr)
来源：http://mpb.jiagoushi.top

PHP:  count($arr);
来源：http://seb.zhoulong.xyz

JS:   arr.length
来源：http://cab.hcnkem.com

TS:   arr.length
来源：http://ydp.nanxinkj.top

Java: list.size();
来源：http://wis.sjlbkw.cn

Go:   len(arr)
来源：http://qyz.daria6918.cn

Ruby: arr.length; arr.size
来源：http://anw.uphjek.com

C#:   list.Count;
来源：http://qoz.xinyue.icu

[D07] 切片 / 取子数组
来源：http://pom.gaohongyu789.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tey.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kta.zhengqikj.top

JS:   arr.slice(1, 4);
来源：http://vuj.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://qhl.vehdjk.com

Java: list.subList(1, 4);
来源：http://wsr.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://iaj.jinqigufen.top

Ruby: arr[1, 3]
来源：http://jbt.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://jxh.hesvh.cn

[D08] 合并两个数组
来源：http://sin.redwolf501.top

Py:   a + b;  a.extend(b)
来源：http://fqc.xuetiantiany.cn

PHP:  array_merge($a, $b);
来源：http://lfk.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pcm.hywenlv.cn

TS:   [...a, ...b];
来源：http://vns.pycfn.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jdg.yongpay.top

Go:   append(a, b...)
来源：http://ugq.yanxiufei.cn

Ruby: a + b;  a.concat(b)
来源：http://hcv.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://ott.mhx1999.top

[D09] 排序（升序）
来源：http://crs.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://nuw.sysykeji.top

PHP:  sort($arr);
来源：http://xbd.yangfankeji.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qjb.9152youxi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qqd.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dfo.gaohongyu789.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tll.yj202588.top

Ruby: arr.sort
来源：http://fuc.vqdsnc.cn

C#:   list.Sort();
来源：http://ovl.shangyingyoupin.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://urn.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ugb.shanyushiyangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sll.vehdjk.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ove.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zbq.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qsc.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eue.yj20258.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://asc.cheryme.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://saj.hywenlv.cn

[D11] 反转数组
来源：http://jdm.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://giu.ybcxt.top

PHP:  array_reverse($arr);
来源：http://ssw.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ymm.ywan-chungtsiang.top

TS:   [...arr].reverse();
来源：http://cdm.vehdjk.com

Java: Collections.reverse(list);
来源：http://drv.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://hfe.ctjpmb.com

Ruby: arr.reverse
来源：http://gep.yj20258888.top

C#:   list.Reverse();
来源：http://jyu.pengpengdd.cyou

[D12] 查找元素下标
来源：http://udq.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://xub.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://auh.zhiwuduotai.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eqi.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mjv.zhengqikj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://prv.birdmap.top

Go:   slices.Index(arr, x)
来源：http://qlv.yuanzhike.top

Ruby: arr.index(x)
来源：http://rjv.jinqigfzy.top

C#:   list.IndexOf(x);
来源：http://apn.hesvh.cn

[D13] 过滤（保留满足条件的）
来源：http://dqs.snrcjt.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fvw.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zdn.tanke756.top

JS:   arr.filter(x => x > 3)
来源：http://fls.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://qed.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://our.52xcode.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hkf.dashuyun.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ylr.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qcm.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://nbk.zhixingplan.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hqu.vehdjk.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ymh.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://bwx.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://ghf.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://krp.mhx1999.top

Go:   // 手写循环
来源：http://bte.fktsv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ktk.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://duq.sxryk.cn

[D15] 去重
来源：http://hbz.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vnb.dianchejie.cn

PHP:  array_unique($arr);
来源：http://xmy.meibo888.top

JS:   [...new Set(arr)]
来源：http://tmn.jlsjyb.cn

TS:   [...new Set(arr)]
来源：http://foh.chenzaomai.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://les.cheryme.top

Go:   // 用 map[T]struct{} 手写
来源：http://vjw.zhixingplan.top

Ruby: arr.uniq
来源：http://xlz.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://btn.cdnleiting.top

[D16] 求和与平均值
来源：http://ljy.xinyue.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lfa.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kqw.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pqv.dashuyun.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xcm.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://prh.zhixingplan.top

Go:   // 手写循环累加
来源：http://mpy.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uyy.fehbvm.com

C#:   list.Sum();  list.Average()
来源：http://int.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://zqz.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://bhq.jqgufenzy.top

PHP:  max($arr);  min($arr);
来源：http://gwl.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://odn.hcnkem.com

TS:   Math.max(...arr);
来源：http://wcz.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mlc.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kxw.pengpengdd.cyou

Ruby: arr.max;  arr.min
来源：http://jhi.jianghu66.top

C#:   list.Max();  list.Min()
来源：http://hpw.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://ris.wangshuangyany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://esu.gogol.net.cn

PHP:  array_merge(...$nested);
来源：http://kzs.0kj1m.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fhs.jiagoushi.top

TS:   nested.flat();
来源：http://ygg.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ium.ydzc1.top

Go:   // 手写双层循环
来源：http://nmw.pengpengdd.cyou

Ruby: nested.flatten
来源：http://ziu.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xro.chenlongwang.top

[D19] 按字段分组
来源：http://xou.hongshengwenyu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sfw.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xxk.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yhh.zhoulong.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://urr.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eid.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://crq.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wtm.yuanzhike.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yjs.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://kkv.guannengcc.top

Py:   Counter(arr)
来源：http://vgv.sxryk.cn

PHP:  array_count_values($arr);
来源：http://ucd.mhx1999.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jpt.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bnm.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://szb.cucudq.cn

Go:   // 手写 map[T]int
来源：http://amk.nanxinkj.top


<!-- 参考信息 -->