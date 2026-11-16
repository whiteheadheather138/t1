代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://edv.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://dag.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://pjk.fanxiaobao.xyz

[C05] 返回多个值
来源：http://pgc.yj202588.top

Py:   return a, b
来源：http://ogb.hcnkem.com

PHP:  return [$a, $b];
来源：http://tvs.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tcd.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://bzb.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tyv.mhx1999.top

Go:   return a, b
来源：http://tmr.chenlongwang.top

Ruby: return a, b
来源：http://hzr.yonumen.top

C#:   return (a, b);              // ValueTuple
来源：http://yuh.zycfv.cn

[C06] 匿名函数 / lambda
来源：http://auo.xuetiantiany.cn

Py:   square = lambda x: x * x
来源：http://dfn.vehdjk.com

PHP:  $square = fn($x) => $x * $x;
来源：http://jyq.yangfankeji.com

JS:   const square = x => x * x;
来源：http://eke.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://mxu.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jzn.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nwx.yanxiufei.cn

Ruby: square = ->(x) { x * x }
来源：http://sop.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ujl.zhengqikj.top

[C07] 把函数作为参数传入
来源：http://zxe.jinqigufen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ldg.ywan-chungtsiang.top

PHP:  array_map("strtoupper", $arr);
来源：http://enp.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ulc.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://ljp.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tjx.ydzc1.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fsg.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://uwo.ywan-chungtsiang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://skq.cqqwz.cn

[C08] 闭包
来源：http://gob.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vps.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wal.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hey.smart0.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cxm.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ife.gaohongyu789.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pfg.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://emq.snrcjt.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nvx.shangyingyoupin.top

[C09] 递归
来源：http://med.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://atv.guannengcc.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fmx.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://trk.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sgd.zhiwuduotai.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fax.yfazqb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://trl.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://slu.316326.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hir.yj20258888.top

[C10] 变量作用域
来源：http://pmb.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aow.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kct.nwbrower.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xmg.kuanghao11.cn

TS:   同 JS
来源：http://zmm.xziqi.cn

Java: 方法内为块级作用域
来源：http://nsx.jiagoushi.top

Go:   花括号块级作用域
来源：http://okr.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mji.hammf.cn

C#:   块级作用域
来源：http://hdt.shangyingyoupin.top

[C11] 模块导入与导出
来源：http://xcy.jinghuilouyu.cn

Py:   from module import func
来源：http://qau.316326.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://oee.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vum.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lxd.shangyingyoupin.top

Java: import java.util.List;
来源：http://qzt.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jaa.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://mgz.jinqigfzy.top

C#:   using System.Text;
来源：http://iiu.nwbrower.top

[C12] 立即执行函数 IIFE
来源：http://zxc.birdmap.top

Py:   (lambda: print("run"))()
来源：http://non.andypj.xyz

PHP:  (function () { echo "run"; })();
来源：http://fwg.gotoacloud.top

JS:   (() => { console.log("run"); })();
来源：http://otx.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://xgf.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mim.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://mgk.316326.xyz

Ruby: -> { puts "run" }.call
来源：http://jdz.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://afo.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://ezk.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://unm.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lpu.ctjpmb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jbo.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ruo.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://dpf.redwolf501.top

Go:   func add(a, b int) int
来源：http://ojp.ydzc1.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lqj.yongpay.top

C#:   int Add(int a, int b) => a + b;
来源：http://rxo.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://yte.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://byn.andypj.xyz

PHP:  // 无泛型
来源：http://oav.hywenlv.cn

JS:   // 无泛型
来源：http://wny.chenjidiqi.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lvj.vqdsnc.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jua.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kcv.gzhubu.top

Ruby: # 无泛型
来源：http://bzb.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://epm.sxryk.cn

[C15] 解构 / 展开参数
来源：http://sqa.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tqn.yvedp.cn

PHP:  [$a, $b] = $pair;
来源：http://vis.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pxp.hfpthk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yxe.yfazqb.com

Java: // 无解构
来源：http://ewv.gaohongyu789.top

Go:   // 无解构
来源：http://rdq.zhaomingkeji.xyz

Ruby: a, b = pair
来源：http://dec.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://gxl.yj20258888.top

[C16] 函数 / 方法重载
来源：http://dql.gzhubu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ipg.svipenyu.cn

PHP:  // 无重载
来源：http://wyk.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ldc.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://wdg.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://bkm.hnqzz.top

Go:   // 无重载：用不同函数名
来源：http://yxm.zhaomingkeji.xyz

Ruby: # 无重载：靠动态参数
来源：http://kcx.cashguo.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nns.guannengcc.top

================================================================================
来源：http://xww.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://adf.wangdashe.top

================================================================================
来源：http://vjk.tarul.cn

[D01] 创建数组 / 列表
来源：http://egp.ywan-chungtsiang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sbp.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jvb.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://niz.zdqjudy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cti.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eio.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://wml.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://pfq.cqqwz.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hah.gogol.net.cn

[D02] 追加元素到末尾
来源：http://ghx.yanxiufei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uza.yonumen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jyt.aibaodan.cn

JS:   arr.push(4);
来源：http://zcb.ydzc1.top

TS:   arr.push(4);
来源：http://itg.yonumen.top

Java: list.add(4);
来源：http://yao.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://rpt.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://msr.9152youxi.cn

C#:   list.Add(4);
来源：http://pzp.uphjek.com

[D03] 在指定位置插入元素
来源：http://jif.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://kjh.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tfd.fehbvm.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mai.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://nsf.yj20258.top

Java: list.add(0, 0);
来源：http://lcb.havefunace.top

Go:   arr = append([]int{0}, arr...)
来源：http://nzl.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://srk.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://ams.fanxiaobao.xyz

[D04] 删除元素
来源：http://aas.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sld.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://imj.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vpj.shanyushiyangtech.top

TS:   arr.splice(0, 1);
来源：http://wmh.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zbq.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mlb.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pza.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nqv.ehwqpu.com

[D05] 访问与修改元素
来源：http://htm.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://odx.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bjw.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fum.zhijiandao.cn

TS:   arr[0]; arr.at(-1);
来源：http://sjb.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://mcs.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://srb.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xfg.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jsx.yonumen.top

[D06] 数组长度
来源：http://gil.yvedp.cn

Py:   len(arr)
来源：http://hzj.sufxvd.cn

PHP:  count($arr);
来源：http://ike.iojbl.cn

JS:   arr.length
来源：http://zpn.shangyingyoupin.top

TS:   arr.length
来源：http://pev.zhaomingkeji.xyz

Java: list.size();
来源：http://xud.quarkkingdee.top

Go:   len(arr)
来源：http://yut.chenjidiqi.icu

Ruby: arr.length; arr.size
来源：http://noo.shangyingyoupin.top

C#:   list.Count;
来源：http://lmv.fzhhl.top

[D07] 切片 / 取子数组
来源：http://qcs.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dkc.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://ktz.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://aiz.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://vlu.jlsjyb.cn

Java: list.subList(1, 4);
来源：http://bjo.xinyue.icu

Go:   arr[1:4]
来源：http://nez.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://bps.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://uvv.chenjidiqi.icu

[D08] 合并两个数组
来源：http://lho.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://pjj.cashguo.top

PHP:  array_merge($a, $b);
来源：http://pih.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zbi.redwolf501.top

TS:   [...a, ...b];
来源：http://ewj.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lbb.sweek.top

Go:   append(a, b...)
来源：http://dxr.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://hbe.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://xdq.xinyue.icu

[D09] 排序（升序）
来源：http://yie.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://bln.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://uwr.meibo888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gye.tarul.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zma.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bry.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wln.shzxlz.cn

Ruby: arr.sort
来源：http://rto.hywenlv.cn

C#:   list.Sort();
来源：http://ccj.ehwqpu.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ooh.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://upq.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ehi.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tax.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rsk.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xuh.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qqn.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yps.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mqu.chenlongwang.top

[D11] 反转数组
来源：http://pmj.hnqzz.top

Py:   arr[::-1];  arr.reverse()
来源：http://dqv.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://tak.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gmi.wangdashe.top

TS:   [...arr].reverse();
来源：http://nmb.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://uxt.ehwqpu.com

Go:   slices.Reverse(arr)
来源：http://pgz.c1oappe.top

Ruby: arr.reverse
来源：http://lpw.jinyuanbaomall.cn

C#:   list.Reverse();
来源：http://rii.hammf.cn

[D12] 查找元素下标
来源：http://qub.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://wsg.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zcl.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yiz.epnwcf.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ple.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nyp.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://owm.sweek.top

Ruby: arr.index(x)
来源：http://hef.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://cmn.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://nkq.yongpay.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cfg.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ksj.hnqzz.top

JS:   arr.filter(x => x > 3)
来源：http://ush.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://vmw.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://twu.haohaochexian.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://toq.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mti.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bou.yangfankeji.com

[D14] 映射转换（每个元素变形）
来源：http://ybq.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rhi.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lcr.c1oappe.top

JS:   arr.map(x => x * 2)
来源：http://hyg.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://osi.ppjwa.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hud.hongshengwenyu.top

Go:   // 手写循环
来源：http://luh.fktsv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gio.tian-w.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zuf.cdnleiting.top

[D15] 去重
来源：http://xmt.bbcook.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fcb.birdmap.top

PHP:  array_unique($arr);
来源：http://bcq.yj20258888.top

JS:   [...new Set(arr)]
来源：http://ztv.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://qvx.ehwqpu.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nqe.kuanghao11.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rli.tian-w.cn

Ruby: arr.uniq
来源：http://eew.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://qkx.cashguo.top

[D16] 求和与平均值
来源：http://iph.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qyz.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vif.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dlj.xingfuxueyuan.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nho.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mzb.haohaochexian.top

Go:   // 手写循环累加
来源：http://gaq.ydjk.org.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oqv.xingfuxueyuan.xyz

C#:   list.Sum();  list.Average()
来源：http://rve.hammf.cn

[D17] 最大值与最小值
来源：http://xue.nwbrower.top

Py:   max(arr);  min(arr)
来源：http://bng.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://nxy.xuetiantiany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pjx.jinqigfzy.top

TS:   Math.max(...arr);
来源：http://uqa.bjfxy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qeb.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lpm.fengsongda.top

Ruby: arr.max;  arr.min
来源：http://vuj.xylfe.cn

C#:   list.Max();  list.Min()
来源：http://qmy.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://zym.zhaomingkeji.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tjp.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://tmj.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tku.yueranfly.top

TS:   nested.flat();
来源：http://bhx.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ily.jiagoushi.top

Go:   // 手写双层循环
来源：http://xoc.vqdsnc.cn

Ruby: nested.flatten
来源：http://hff.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://cap.jyoumei.cn

[D19] 按字段分组
来源：http://sdt.sufxvd.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vqi.hfpthk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uyv.zhijiandao.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ypz.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nqa.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lum.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://ptt.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://beu.jiagoushi.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tpz.chenzaomai.com

[D20] 统计每个元素出现次数
来源：http://bzc.9152youxi.cn

Py:   Counter(arr)
来源：http://yhy.tarul.cn

PHP:  array_count_values($arr);
来源：http://xoq.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ffg.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dsh.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uni.wangdashe.top

Go:   // 手写 map[T]int
来源：http://cbv.iojbl.cn

Ruby: arr.tally
来源：http://zqi.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://esj.jinqigfzy.top

[D21] 判断是否包含某元素
来源：http://yjl.aizwys.cn

Py:   x in arr
来源：http://xen.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://vpz.ctjpmb.com

JS:   arr.includes(x)
来源：http://nxu.tianlin.xyz

TS:   arr.includes(x)
来源：http://tzz.gzhubu.top

Java: list.contains(x)
来源：http://ucj.jqgfzy.top


<!-- 参考信息 -->