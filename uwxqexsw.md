代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://mfx.ehwqpu.com

Ruby: f(a: 1, b: 2)
来源：http://aab.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://fuq.feifeiyinyue.top

[C05] 返回多个值
来源：http://tfi.gogol.net.cn

Py:   return a, b
来源：http://ykk.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://las.hongshengwenyu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mnc.hnxiangtu.top

TS:   return { a, b };
来源：http://pur.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jlh.andypj.xyz

Go:   return a, b
来源：http://pcr.yfazqb.com

Ruby: return a, b
来源：http://dpf.zhongyouzk.top

C#:   return (a, b);              // ValueTuple
来源：http://amb.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://bsy.yongpay.top

Py:   square = lambda x: x * x
来源：http://buj.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://pux.yanxiufei.cn

JS:   const square = x => x * x;
来源：http://pia.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://tno.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://atx.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://don.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://zmy.jqgfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://uzy.sjlbkw.cn

[C07] 把函数作为参数传入
来源：http://qxc.daria6918.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vmf.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://wpc.uphjek.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pva.xylfe.cn

TS:   arr.map(String)
来源：http://sti.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kzb.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://upi.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://fvq.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mfr.yvedp.cn

[C08] 闭包
来源：http://yce.sufxvd.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oli.zdqjudy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bsi.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bub.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xho.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qff.redwolf501.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tod.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mka.nwbrower.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://phz.gotoacloud.top

[C09] 递归
来源：http://hhz.chenzaomai.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oap.epnwcf.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kzc.dashuyun.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hht.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gom.yueranfly.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lhd.yanxiufei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://upo.ivvv.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iau.hesvh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wzf.chenlongwang.top

[C10] 变量作用域
来源：http://xku.ppjwa.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://btc.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wbr.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://spm.aibaodan.cn

TS:   同 JS
来源：http://cpg.sysykeji.top

Java: 方法内为块级作用域
来源：http://ffy.hammf.cn

Go:   花括号块级作用域
来源：http://ozi.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://izn.birdmap.top

C#:   块级作用域
来源：http://dmt.chenjidiqi.icu

[C11] 模块导入与导出
来源：http://xof.zhiwuduotai.top

Py:   from module import func
来源：http://uop.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://elj.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fuc.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ltx.tian-w.cn

Java: import java.util.List;
来源：http://dbf.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bvd.shuidangran.top

Ruby: require "json"; require_relative "./util"
来源：http://two.aizwys.cn

C#:   using System.Text;
来源：http://deo.gogol.net.cn

[C12] 立即执行函数 IIFE
来源：http://rds.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://dfz.xinyue.icu

PHP:  (function () { echo "run"; })();
来源：http://rkl.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://ssi.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://cps.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ifg.tanke756.top

Go:   func() { fmt.Println("run") }()
来源：http://ctx.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://vqp.nwbrower.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bwc.svipenyu.cn

[C13] 类型声明 / 类型注解
来源：http://qtp.jqgfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ndm.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xra.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zmo.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aej.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qrg.fehbvm.com

Go:   func add(a, b int) int
来源：http://bys.chenzaomai.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oaz.ywan-chungtsiang.top

C#:   int Add(int a, int b) => a + b;
来源：http://luw.kuanghao11.cn

[C14] 泛型函数
来源：http://mmn.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fsk.shzxlz.cn

PHP:  // 无泛型
来源：http://aeb.0kj1m.cn

JS:   // 无泛型
来源：http://rqx.birdmap.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yey.ppjwa.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ysj.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ssu.guowangkeji.top

Ruby: # 无泛型
来源：http://cfn.sweek.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ovo.mhx1999.top

[C15] 解构 / 展开参数
来源：http://uiq.jqgfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qob.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://gee.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wps.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eap.ivvv.top

Java: // 无解构
来源：http://gkz.svipenyu.cn

Go:   // 无解构
来源：http://oah.cashguo.top

Ruby: a, b = pair
来源：http://sxz.cucudq.cn

C#:   var (a, b) = pair;
来源：http://ohy.hcnkem.com

[C16] 函数 / 方法重载
来源：http://agq.cqqwz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jgw.zdbjq.cn

PHP:  // 无重载
来源：http://seu.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://hps.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://hpj.sysykeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://neo.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://uoj.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://pmm.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cwv.xingfuxueyuan.xyz

================================================================================
来源：http://mgc.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://ied.yuxming.cn

================================================================================
来源：http://wnx.yvedp.cn

[D01] 创建数组 / 列表
来源：http://rki.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://bkv.pycfn.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vad.fzhhl.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lja.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://czc.jinqigufen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yxv.yanxiufei.cn

Go:   arr := []int{1, 2, 3}
来源：http://kdc.snrcjt.cn

Ruby: arr = [1, 2, 3]
来源：http://qto.zycfv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wlm.sysykeji.top

[D02] 追加元素到末尾
来源：http://uil.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://okw.snrcjt.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wtv.shuidangran.top

JS:   arr.push(4);
来源：http://krt.ybcxt.top

TS:   arr.push(4);
来源：http://pay.feifeiyinyue.top

Java: list.add(4);
来源：http://ldm.jlsjyb.cn

Go:   arr = append(arr, 4)
来源：http://eex.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://zoa.hnqzz.top

C#:   list.Add(4);
来源：http://dmp.sweek.top

[D03] 在指定位置插入元素
来源：http://nzz.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://jpd.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ldf.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kby.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://faw.hongshengwenyu.top

Java: list.add(0, 0);
来源：http://pnn.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://ydk.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oci.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://gxz.snrcjt.cn

[D04] 删除元素
来源：http://zna.nanxinkj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gxl.yuxming.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://guo.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ghf.gogol.net.cn

TS:   arr.splice(0, 1);
来源：http://qfr.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lmw.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xod.bbcook.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vgf.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cuv.dianchejie.cn

[D05] 访问与修改元素
来源：http://rza.dashuyun.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lod.jiagoushi.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jri.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mjc.gotoacloud.top

TS:   arr[0]; arr.at(-1);
来源：http://mat.tian-w.cn

Java: list.get(0); list.set(0, 9);
来源：http://hiq.haohaochexian.top

Go:   arr[0]; arr[0] = 9
来源：http://fdl.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zps.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vdx.hywenlv.cn

[D06] 数组长度
来源：http://pyf.jiagoushi.top

Py:   len(arr)
来源：http://bvv.ppjwa.cn

PHP:  count($arr);
来源：http://mms.chenjidiqi.icu

JS:   arr.length
来源：http://egi.gaohongyu789.top

TS:   arr.length
来源：http://qmb.xuetiantiany.cn

Java: list.size();
来源：http://ach.cqqwz.cn

Go:   len(arr)
来源：http://bxx.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://bso.daxiang520.top

C#:   list.Count;
来源：http://uwy.andypj.xyz

[D07] 切片 / 取子数组
来源：http://pgv.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wrb.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://rdy.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://sch.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://ooo.tarul.cn

Java: list.subList(1, 4);
来源：http://ezm.hfpthk.cn

Go:   arr[1:4]
来源：http://fdy.cdnleiting.top

Ruby: arr[1, 3]
来源：http://eqf.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://lpu.feifeiyinyue.top

[D08] 合并两个数组
来源：http://mpe.sysykeji.top

Py:   a + b;  a.extend(b)
来源：http://lrp.birdmap.top

PHP:  array_merge($a, $b);
来源：http://jit.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://enr.ehwqpu.com

TS:   [...a, ...b];
来源：http://ecs.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://snm.pycfn.com

Go:   append(a, b...)
来源：http://jci.shanyushiyangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://ogu.snrcjt.cn

C#:   a.Concat(b).ToList()
来源：http://yaw.xylfe.cn

[D09] 排序（升序）
来源：http://yle.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://uei.ctjpmb.com

PHP:  sort($arr);
来源：http://xkk.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dmd.jinqigufen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kcj.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://xyx.shuidangran.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://raa.shuidangran.top

Ruby: arr.sort
来源：http://bwf.hywenlv.cn

C#:   list.Sort();
来源：http://yel.sufxvd.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://eiu.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fho.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://act.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jtf.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uje.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gom.birdmap.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qml.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sil.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qoh.tianlin.xyz

[D11] 反转数组
来源：http://tei.ywan-chungtsiang.top

Py:   arr[::-1];  arr.reverse()
来源：http://awf.bbcook.cn

PHP:  array_reverse($arr);
来源：http://erg.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vvg.uphjek.com

TS:   [...arr].reverse();
来源：http://haz.ppjwa.cn

Java: Collections.reverse(list);
来源：http://zjf.zhixingplan.top

Go:   slices.Reverse(arr)
来源：http://scg.yj202588.top

Ruby: arr.reverse
来源：http://poi.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://vfv.zhengqikj.top

[D12] 查找元素下标
来源：http://tsw.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://enn.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://htc.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vsv.ivvv.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wne.ybcxt.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fjl.tanke756.top

Go:   slices.Index(arr, x)
来源：http://huc.meibo888.top

Ruby: arr.index(x)
来源：http://gqi.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://qhh.redwolf501.top

[D13] 过滤（保留满足条件的）
来源：http://fsp.svipenyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zgb.pengpengdd.cyou

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xuv.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://xnu.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://fle.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tnj.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://flx.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rxh.cucudq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pye.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://kit.gogol.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nzq.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yux.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://hud.dashuyun.cn

TS:   arr.map(x => x * 2)
来源：http://nis.haohaochexian.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xwf.ppjwa.cn

Go:   // 手写循环
来源：http://zot.c1oappe.top

Ruby: arr.map { |x| x * 2 }
来源：http://hov.cheryme.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cbc.hammf.cn

[D15] 去重
来源：http://soi.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ymo.ydzc1.top

PHP:  array_unique($arr);
来源：http://wkq.fengsongda.top

JS:   [...new Set(arr)]
来源：http://smo.kuanghao11.cn

TS:   [...new Set(arr)]
来源：http://row.hammf.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bbh.hongshengwenyu.top

Go:   // 用 map[T]struct{} 手写
来源：http://znw.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://ein.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://fot.pengpengdd.cyou

[D16] 求和与平均值
来源：http://qkb.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kam.9152youxi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dyd.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dql.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fmc.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ier.xylfe.cn

Go:   // 手写循环累加
来源：http://sdv.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nkj.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://sey.meibo888.top

[D17] 最大值与最小值
来源：http://vuz.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://quh.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://nnf.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://att.yj20258.top

TS:   Math.max(...arr);
来源：http://daj.tarul.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fiv.hcnkem.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://msu.sxryk.cn

Ruby: arr.max;  arr.min
来源：http://uoa.sjlbkw.cn

C#:   list.Max();  list.Min()
来源：http://nxf.snrcjt.cn

[D18] 扁平化嵌套数组
来源：http://bgm.jianghu66.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fya.jinqigufen.top

PHP:  array_merge(...$nested);
来源：http://fkr.dashuyun.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hvk.xinyue.icu

TS:   nested.flat();
来源：http://nni.bbcook.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bgu.chenlongwang.top

Go:   // 手写双层循环
来源：http://tnj.epnwcf.com

Ruby: nested.flatten
来源：http://bsq.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xxj.chenjidiqi.icu

[D19] 按字段分组
来源：http://vjn.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lfd.c1oappe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://exw.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cao.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qpp.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://heq.zhongyouzk.top

Go:   // 手写 map[string][]T
来源：http://uqt.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kdb.birdmap.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uil.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://czb.havefunace.top

Py:   Counter(arr)
来源：http://zje.tarul.cn

PHP:  array_count_values($arr);
来源：http://cwn.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tuo.quarkkingdee.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://avb.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ymj.ivvv.top

Go:   // 手写 map[T]int
来源：http://nzk.redwolf501.top

Ruby: arr.tally
来源：http://aee.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wjx.kuanghao11.cn

[D21] 判断是否包含某元素
来源：http://naa.tarul.cn

Py:   x in arr
来源：http://zem.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://een.hysaishi.cn

JS:   arr.includes(x)
来源：http://etz.zhengqikj.top

TS:   arr.includes(x)
来源：http://bty.aizwys.cn

Java: list.contains(x)
来源：http://yuh.haohaochexian.top


<!-- 参考信息 -->