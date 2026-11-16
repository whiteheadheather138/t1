代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hnw.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rzi.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xqi.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://vrt.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://csr.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://fnr.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://hsj.jqgufenzy.top

[C05] 返回多个值
来源：http://twm.9152youxi.cn

Py:   return a, b
来源：http://vme.hywenlv.cn

PHP:  return [$a, $b];
来源：http://aio.tanke756.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hym.ydjk.org.cn

TS:   return { a, b };
来源：http://obd.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zsg.yuanzhike.top

Go:   return a, b
来源：http://ejl.ydzc1.top

Ruby: return a, b
来源：http://nnw.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://ndd.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://pku.xinyue.icu

Py:   square = lambda x: x * x
来源：http://ndu.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nlg.uphjek.com

JS:   const square = x => x * x;
来源：http://nsu.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://isi.zhengqikj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pyq.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jay.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://jnb.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://vih.sweek.top

[C07] 把函数作为参数传入
来源：http://wuf.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tcf.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://sns.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ago.fktsv.cn

TS:   arr.map(String)
来源：http://nrd.gaohongyu789.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jpm.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nyd.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://kwh.yj20258.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ibt.uphjek.com

[C08] 闭包
来源：http://ziv.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ypp.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vba.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mbg.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wty.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tfy.zhijiandao.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lvs.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vwl.hnqzz.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lwk.smart0.xyz

[C09] 递归
来源：http://gmm.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qcl.zdqjudy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jxh.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://btb.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uls.guannengcc.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eej.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mmw.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zdz.bjfxy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zsy.tianlin.xyz

[C10] 变量作用域
来源：http://ivg.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://atn.sufxvd.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://llz.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vvm.guowangkeji.top

TS:   同 JS
来源：http://yaq.ctjpmb.com

Java: 方法内为块级作用域
来源：http://rsx.xylfe.cn

Go:   花括号块级作用域
来源：http://wyw.cdnleiting.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zms.yj20258.top

C#:   块级作用域
来源：http://cch.sufxvd.cn

[C11] 模块导入与导出
来源：http://wop.snrcjt.cn

Py:   from module import func
来源：http://usp.hnxiangtu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://omj.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lha.nanxuanxn.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://aqe.xylfe.cn

Java: import java.util.List;
来源：http://fig.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qwz.xingfuxueyuan.xyz

Ruby: require "json"; require_relative "./util"
来源：http://mcy.yongpay.top

C#:   using System.Text;
来源：http://cbx.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://zbm.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://ale.ivvv.top

PHP:  (function () { echo "run"; })();
来源：http://upc.jyoumei.cn

JS:   (() => { console.log("run"); })();
来源：http://ifz.hammf.cn

TS:   (() => { console.log("run"); })();
来源：http://unq.sysykeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ypp.jianghu66.top

Go:   func() { fmt.Println("run") }()
来源：http://oyk.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://feg.andypj.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://eou.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://dcl.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jal.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://maj.ydjk.org.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://scc.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://isp.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://snl.birdmap.top

Go:   func add(a, b int) int
来源：http://mzp.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bcw.uphjek.com

C#:   int Add(int a, int b) => a + b;
来源：http://pqw.haohaochexian.top

[C14] 泛型函数
来源：http://sjo.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://awh.9152youxi.cn

PHP:  // 无泛型
来源：http://ile.9152youxi.cn

JS:   // 无泛型
来源：http://fzl.xylfe.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dzg.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qvo.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://acn.zhixingplan.top

Ruby: # 无泛型
来源：http://cjr.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://giv.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://pyp.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uqh.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://yjs.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jrl.hammf.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://drh.quarkkingdee.top

Java: // 无解构
来源：http://xiv.havefunace.top

Go:   // 无解构
来源：http://ozd.yj20258.top

Ruby: a, b = pair
来源：http://xfb.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://wkc.chenzaomai.com

[C16] 函数 / 方法重载
来源：http://utm.xingfuxueyuan.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gbo.smart0.xyz

PHP:  // 无重载
来源：http://tii.gzhubu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ioo.cdnleiting.top

TS:   // 用联合类型或重载签名声明
来源：http://gye.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://opw.yfazqb.com

Go:   // 无重载：用不同函数名
来源：http://sxo.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://hld.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jfs.ppjwa.cn

================================================================================
来源：http://yru.havefunace.top

D. 数组 / 列表 / 集合
来源：http://asf.zdqjudy.top

================================================================================
来源：http://eyn.ybcxt.top

[D01] 创建数组 / 列表
来源：http://sdq.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://poc.tianlin.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tzx.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jiw.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xif.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eyk.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://epq.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://maz.jinghuilouyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ydd.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://djh.c1oappe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lga.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mzs.yfazqb.com

JS:   arr.push(4);
来源：http://cxn.hammf.cn

TS:   arr.push(4);
来源：http://frr.hfpthk.cn

Java: list.add(4);
来源：http://jhl.vehdjk.com

Go:   arr = append(arr, 4)
来源：http://wph.epnwcf.com

Ruby: arr << 4; arr.push(5)
来源：http://omz.dianchejie.cn

C#:   list.Add(4);
来源：http://lto.sysykeji.top

[D03] 在指定位置插入元素
来源：http://buk.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://yhv.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xkk.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tgi.zhiwuduotai.top

TS:   arr.splice(0, 0, 0);
来源：http://lhw.dianchejie.cn

Java: list.add(0, 0);
来源：http://lst.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://maz.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lsz.jinghuilouyu.cn

C#:   list.Insert(0, 0);
来源：http://stf.jiagoushi.top

[D04] 删除元素
来源：http://rnm.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hou.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ddi.sxryk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dcv.yongpay.top

TS:   arr.splice(0, 1);
来源：http://snl.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pfr.meibo888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bym.gzhubu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://czc.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lui.52xcode.cn

[D05] 访问与修改元素
来源：http://tlo.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://crx.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jzy.c1oappe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jlv.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://fhc.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://wcf.hywenlv.cn

Go:   arr[0]; arr[0] = 9
来源：http://ccv.zdbjq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://apw.hnxiangtu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jxz.cashguo.top

[D06] 数组长度
来源：http://dvn.ywan-chungtsiang.top

Py:   len(arr)
来源：http://hzf.zhiwuduotai.top

PHP:  count($arr);
来源：http://vtv.zhoulong.xyz

JS:   arr.length
来源：http://sla.birdmap.top

TS:   arr.length
来源：http://ojk.havefunace.top

Java: list.size();
来源：http://epg.xylfe.cn

Go:   len(arr)
来源：http://bad.gzhubu.top

Ruby: arr.length; arr.size
来源：http://pvb.fzhhl.top

C#:   list.Count;
来源：http://cgs.sweek.top

[D07] 切片 / 取子数组
来源：http://klo.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jgh.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rmy.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://llg.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://zvw.hnqzz.top

Java: list.subList(1, 4);
来源：http://fgs.zdbjq.cn

Go:   arr[1:4]
来源：http://wnw.hysaishi.cn

Ruby: arr[1, 3]
来源：http://xsf.yj20258.top

C#:   list.GetRange(1, 3);
来源：http://gad.cqqwz.cn

[D08] 合并两个数组
来源：http://afu.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://slg.ivvv.top

PHP:  array_merge($a, $b);
来源：http://ozk.jianghu66.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xgy.pengpengdd.cyou

TS:   [...a, ...b];
来源：http://wly.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://exl.cashguo.top

Go:   append(a, b...)
来源：http://lsl.yj202588.top

Ruby: a + b;  a.concat(b)
来源：http://zdh.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://tov.sxryk.cn

[D09] 排序（升序）
来源：http://dkg.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://ugn.xuetiantiany.cn

PHP:  sort($arr);
来源：http://hac.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eee.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://grp.sufxvd.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mxp.vqdsnc.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dqp.epnwcf.com

Ruby: arr.sort
来源：http://bgp.pycfn.com

C#:   list.Sort();
来源：http://oja.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oel.fengsongda.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tkw.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://emu.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ifv.nwbrower.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ylu.ivvv.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yed.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tkf.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qas.0kj1m.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lag.hammf.cn

[D11] 反转数组
来源：http://rfo.hongshengwenyu.top

Py:   arr[::-1];  arr.reverse()
来源：http://ovn.pycfn.com

PHP:  array_reverse($arr);
来源：http://bgc.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zmk.zdbjq.cn

TS:   [...arr].reverse();
来源：http://hxw.wangshuangyany.cn

Java: Collections.reverse(list);
来源：http://ouk.redwolf501.top

Go:   slices.Reverse(arr)
来源：http://pov.hammf.cn

Ruby: arr.reverse
来源：http://ppw.aizwys.cn

C#:   list.Reverse();
来源：http://rqv.epnwcf.com

[D12] 查找元素下标
来源：http://dmy.yj20258.top

Py:   arr.index(x);  x in arr
来源：http://wvg.jinghuilouyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tki.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fiy.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uer.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fvt.zhixingplan.top

Go:   slices.Index(arr, x)
来源：http://tvn.tanke756.top

Ruby: arr.index(x)
来源：http://cxt.yangfankeji.com

C#:   list.IndexOf(x);
来源：http://jwj.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://xun.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wyd.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ufq.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://bui.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://jtq.havefunace.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eqz.tanke756.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jhv.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yyw.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ckm.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://pam.mhx1999.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://chm.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kmc.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://qwq.xingfuxueyuan.xyz

TS:   arr.map(x => x * 2)
来源：http://fix.sufxvd.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ghn.andypj.xyz

Go:   // 手写循环
来源：http://mnq.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://ysc.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://snm.daria6918.cn

[D15] 去重
来源：http://gut.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zbk.daxiang520.top

PHP:  array_unique($arr);
来源：http://ami.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://ias.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://hib.svipenyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://diw.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fcm.zdqjudy.top

Ruby: arr.uniq
来源：http://rel.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://mro.chenjidiqi.icu

[D16] 求和与平均值
来源：http://fyu.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uqr.kuanghao11.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bhe.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gis.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oky.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bol.hesvh.cn

Go:   // 手写循环累加
来源：http://xbw.jiagoushi.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aig.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://yez.zdqjudy.top

[D17] 最大值与最小值
来源：http://nlg.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://zrm.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://qgt.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vyo.snrcjt.cn

TS:   Math.max(...arr);
来源：http://pml.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://tou.jinyuanbaomall.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gjh.gzhubu.top

Ruby: arr.max;  arr.min
来源：http://vey.daxiang520.top

C#:   list.Max();  list.Min()
来源：http://huf.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://vsb.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ump.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://nzf.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lmv.yangfankeji.com

TS:   nested.flat();
来源：http://sgk.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tjj.yj20258.top

Go:   // 手写双层循环
来源：http://mxf.fehbvm.com

Ruby: nested.flatten
来源：http://ppv.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://juq.sweek.top

[D19] 按字段分组
来源：http://oza.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vcp.nwbrower.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oko.birdmap.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://auf.svipenyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cpl.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uyt.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://yhu.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mdn.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vhh.shuidangran.top

[D20] 统计每个元素出现次数
来源：http://nrs.shzxlz.cn

Py:   Counter(arr)
来源：http://gey.quarkkingdee.top

PHP:  array_count_values($arr);
来源：http://paz.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cnz.zhiwuduotai.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tqo.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jxv.yj202588.top

Go:   // 手写 map[T]int
来源：http://fxg.ydjk.org.cn

Ruby: arr.tally
来源：http://tgt.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wfh.daria6918.cn

[D21] 判断是否包含某元素
来源：http://qhm.xylfe.cn

Py:   x in arr
来源：http://mgo.shzxlz.cn


<!-- 参考信息 -->