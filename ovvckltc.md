代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://dsg.zdbjq.cn

Ruby: f(a: 1, b: 2)
来源：http://icn.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://qnw.wangshuangyany.cn

[C05] 返回多个值
来源：http://dbk.nanxuanxn.top

Py:   return a, b
来源：http://enb.hammf.cn

PHP:  return [$a, $b];
来源：http://lcu.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://zpt.kuanghao11.cn

TS:   return { a, b };
来源：http://waa.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hqv.hnqzz.top

Go:   return a, b
来源：http://cqx.yonumen.top

Ruby: return a, b
来源：http://jlf.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://lyz.shanyushiyangkeji.top

[C06] 匿名函数 / lambda
来源：http://mhi.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://jim.yj202588.top

PHP:  $square = fn($x) => $x * $x;
来源：http://guy.zdbjq.cn

JS:   const square = x => x * x;
来源：http://ziz.xziqi.cn

TS:   const square = (x: number): number => x * x;
来源：http://njx.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kpm.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://tqa.xuetiantiany.cn

Ruby: square = ->(x) { x * x }
来源：http://qea.zdqjudy.top

C#:   Func<int, int> square = x => x * x;
来源：http://yih.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://bhp.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tve.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://bmf.cashguo.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://diy.quarkkingdee.top

TS:   arr.map(String)
来源：http://xeo.cucudq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bcs.jiagoushi.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ckb.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://lxq.wangshuangyany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ych.hysaishi.cn

[C08] 闭包
来源：http://mvv.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://igo.hesvh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://siy.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nbe.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hzz.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://coo.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mbf.hysaishi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ntl.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ksv.xuetiantiany.cn

[C09] 递归
来源：http://xhg.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ukh.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gqu.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gtu.svipenyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://igp.bjfxy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://anw.yfazqb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ejg.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ban.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mwt.52xcode.cn

[C10] 变量作用域
来源：http://bnf.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gxm.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lwt.sufxvd.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fwj.svipenyu.cn

TS:   同 JS
来源：http://ekk.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://bhe.nwbrower.top

Go:   花括号块级作用域
来源：http://ydg.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sqd.zhixingplan.top

C#:   块级作用域
来源：http://vyp.chenjidiqi.icu

[C11] 模块导入与导出
来源：http://ibd.shzxlz.cn

Py:   from module import func
来源：http://mxc.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bpk.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zan.ybcxt.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hqr.epnwcf.com

Java: import java.util.List;
来源：http://xdm.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dzp.sufxvd.cn

Ruby: require "json"; require_relative "./util"
来源：http://vge.ppjwa.cn

C#:   using System.Text;
来源：http://vop.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://ble.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://nje.ydjk.org.cn

PHP:  (function () { echo "run"; })();
来源：http://lbj.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://nkx.hongshengwenyu.top

TS:   (() => { console.log("run"); })();
来源：http://yjl.yongpay.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oli.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://ndn.havefunace.top

Ruby: -> { puts "run" }.call
来源：http://qaj.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://aec.feifeiyinyue.top

[C13] 类型声明 / 类型注解
来源：http://hgv.jianghu66.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://evy.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lkk.zhixingplan.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://als.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ijv.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://bjv.zycfv.cn

Go:   func add(a, b int) int
来源：http://zhi.svipenyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://est.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://xok.uphjek.com

[C14] 泛型函数
来源：http://qba.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://frv.cdnleiting.top

PHP:  // 无泛型
来源：http://ucc.wangshuangyany.cn

JS:   // 无泛型
来源：http://fqn.vqdsnc.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oqv.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tns.zhiwuduotai.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tun.bbcook.cn

Ruby: # 无泛型
来源：http://apv.dashuyun.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xyi.sweek.top

[C15] 解构 / 展开参数
来源：http://msi.yonumen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qfq.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://zcn.shanyushiyangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ggy.xinyue.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ytq.svipenyu.cn

Java: // 无解构
来源：http://kbh.yanxiufei.cn

Go:   // 无解构
来源：http://zqk.aibaodan.cn

Ruby: a, b = pair
来源：http://cxt.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://nfr.yj20258888.top

[C16] 函数 / 方法重载
来源：http://ygq.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rxh.yj20258.top

PHP:  // 无重载
来源：http://ots.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://sjj.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://xuo.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rec.xuanzx.com

Go:   // 无重载：用不同函数名
来源：http://qfd.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://lep.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hgx.tanke756.top

================================================================================
来源：http://lvh.wangdashe.top

D. 数组 / 列表 / 集合
来源：http://xgg.hammf.cn

================================================================================
来源：http://qyi.hammf.cn

[D01] 创建数组 / 列表
来源：http://dqo.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://dqu.tarul.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pzm.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dud.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nxg.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sar.gotoacloud.top

Go:   arr := []int{1, 2, 3}
来源：http://xha.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://uzt.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iee.sweek.top

[D02] 追加元素到末尾
来源：http://vrq.zdbjq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nin.sufxvd.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oxk.ivvv.top

JS:   arr.push(4);
来源：http://ogz.yfazqb.com

TS:   arr.push(4);
来源：http://hvb.yfazqb.com

Java: list.add(4);
来源：http://cea.sweek.top

Go:   arr = append(arr, 4)
来源：http://twd.yueranfly.top

Ruby: arr << 4; arr.push(5)
来源：http://snu.yangfankeji.com

C#:   list.Add(4);
来源：http://iqb.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://myc.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://tfm.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qwb.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ata.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://bvq.jyoumei.cn

Java: list.add(0, 0);
来源：http://dkt.fktsv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zqw.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zxi.52xcode.cn

C#:   list.Insert(0, 0);
来源：http://uqb.yj20258888.top

[D04] 删除元素
来源：http://vuf.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sjo.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dae.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nww.xziqi.cn

TS:   arr.splice(0, 1);
来源：http://yic.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ynk.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uzb.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uii.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qza.birdmap.top

[D05] 访问与修改元素
来源：http://uvt.jqgufenzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ioi.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zvm.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jkd.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://zcp.dianchejie.cn

Java: list.get(0); list.set(0, 9);
来源：http://rud.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://jeb.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wux.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kag.hongshengwenyu.top

[D06] 数组长度
来源：http://iee.bbcook.cn

Py:   len(arr)
来源：http://xtu.ybcxt.top

PHP:  count($arr);
来源：http://ehx.guannengcc.top

JS:   arr.length
来源：http://qci.c1oappe.top

TS:   arr.length
来源：http://vso.ydzc1.top

Java: list.size();
来源：http://ccc.yueranfly.top

Go:   len(arr)
来源：http://qai.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://ope.316326.xyz

C#:   list.Count;
来源：http://xqa.birdmap.top

[D07] 切片 / 取子数组
来源：http://wsw.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://heb.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://glz.hesvh.cn

JS:   arr.slice(1, 4);
来源：http://dor.c1oappe.top

TS:   arr.slice(1, 4);
来源：http://opp.jiagoushi.top

Java: list.subList(1, 4);
来源：http://lzp.tarul.cn

Go:   arr[1:4]
来源：http://exm.sxryk.cn

Ruby: arr[1, 3]
来源：http://unk.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://cxp.yanxiufei.cn

[D08] 合并两个数组
来源：http://qbd.pengpengdd.cyou

Py:   a + b;  a.extend(b)
来源：http://vgy.yanxiufei.cn

PHP:  array_merge($a, $b);
来源：http://doy.mhx1999.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ljl.tian-w.cn

TS:   [...a, ...b];
来源：http://ees.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uxq.smart0.xyz

Go:   append(a, b...)
来源：http://lfr.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://wtb.hnqzz.top

C#:   a.Concat(b).ToList()
来源：http://zrg.xylfe.cn

[D09] 排序（升序）
来源：http://cwd.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://lrb.snrcjt.cn

PHP:  sort($arr);
来源：http://ioo.yangfankeji.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ddu.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uhy.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rum.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jfd.xinyue.icu

Ruby: arr.sort
来源：http://rcs.cdnleiting.top

C#:   list.Sort();
来源：http://lml.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xho.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lgj.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hhz.hesvh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tua.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hkx.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uno.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eii.gotoacloud.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://egt.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://klm.feifeiyinyue.top

[D11] 反转数组
来源：http://gew.ydjk.org.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zyx.yj20258888.top

PHP:  array_reverse($arr);
来源：http://tyh.yfazqb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vge.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://mhj.ctjpmb.com

Java: Collections.reverse(list);
来源：http://xgv.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://ywk.gaohongyu789.top

Ruby: arr.reverse
来源：http://xcf.c1oappe.top

C#:   list.Reverse();
来源：http://ral.snrcjt.cn

[D12] 查找元素下标
来源：http://mva.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://nxv.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uex.xylfe.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qnn.hongshengwenyu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dko.haohaochexian.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sgm.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://was.zdqjudy.top

Ruby: arr.index(x)
来源：http://ntd.c1oappe.top

C#:   list.IndexOf(x);
来源：http://pfk.shzxlz.cn

[D13] 过滤（保留满足条件的）
来源：http://hjj.vqdsnc.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zwq.hfpthk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vzn.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://ixt.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://oqf.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yuv.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yaa.zdbjq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://aro.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://eaj.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://apu.cheryme.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nrb.iojbl.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wbo.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://pwo.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://cer.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://icx.sjlbkw.cn

Go:   // 手写循环
来源：http://zow.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://zer.dashuyun.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://etp.cheryme.top

[D15] 去重
来源：http://kcd.uphjek.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vux.nanxinkj.top

PHP:  array_unique($arr);
来源：http://yri.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://uni.aizwys.cn

TS:   [...new Set(arr)]
来源：http://gka.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ftx.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://eyy.quarkkingdee.top

Ruby: arr.uniq
来源：http://njg.jiagoushi.top

C#:   list.Distinct().ToList()
来源：http://nyj.xinyue.icu

[D16] 求和与平均值
来源：http://wzi.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://czx.shangyingyoupin.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wiy.aibaodan.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iol.zhiwuduotai.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kdm.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fzq.c1oappe.top

Go:   // 手写循环累加
来源：http://ncv.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jox.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://rxq.tanke756.top

[D17] 最大值与最小值
来源：http://krv.cqqwz.cn

Py:   max(arr);  min(arr)
来源：http://wyt.sweek.top

PHP:  max($arr);  min($arr);
来源：http://nnv.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lrp.ehwqpu.com

TS:   Math.max(...arr);
来源：http://cdf.jinyuanbaomall.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lsx.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dpn.fanxiaobao.xyz

Ruby: arr.max;  arr.min
来源：http://pqt.yfazqb.com

C#:   list.Max();  list.Min()
来源：http://gnd.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://zoq.sjlbkw.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qyk.andypj.xyz

PHP:  array_merge(...$nested);
来源：http://xfy.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://thx.chenlongwang.top

TS:   nested.flat();
来源：http://dry.smart0.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://duk.shangyingyoupin.top

Go:   // 手写双层循环
来源：http://bmh.bbcook.cn

Ruby: nested.flatten
来源：http://gzm.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://nck.ctjpmb.com

[D19] 按字段分组
来源：http://ies.mhx1999.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kda.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bqg.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dma.yj20258888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wbt.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://crv.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://jft.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jyt.hesvh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dsz.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://ahi.tianlin.xyz

Py:   Counter(arr)
来源：http://lmq.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://rbt.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xyw.zhiwuduotai.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oky.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://est.xuanzx.com

Go:   // 手写 map[T]int
来源：http://vqn.xziqi.cn

Ruby: arr.tally
来源：http://tvr.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ibu.daxiang520.top

[D21] 判断是否包含某元素
来源：http://oos.hysaishi.cn

Py:   x in arr
来源：http://ujs.tanke756.top

PHP:  in_array($x, $arr, true);
来源：http://jxr.yonumen.top

JS:   arr.includes(x)
来源：http://drf.aizwys.cn

TS:   arr.includes(x)
来源：http://nvm.chenzaomai.com

Java: list.contains(x)
来源：http://mpr.jianghu66.top


<!-- 参考信息 -->