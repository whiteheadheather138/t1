代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qby.quarkkingdee.top

Go:   return a, b
来源：http://ehx.guannengcc.top

Ruby: return a, b
来源：http://adp.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://cgl.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://tee.cucudq.cn

Py:   square = lambda x: x * x
来源：http://rqj.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://szf.wangdashe.top

JS:   const square = x => x * x;
来源：http://xtw.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://omb.hywenlv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jkq.yangfankeji.com

Go:   sq := func(x int) int { return x * x }
来源：http://vqo.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://irc.ydjk.org.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qus.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://ofg.jqgfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wea.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wfh.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wyd.daria6918.cn

TS:   arr.map(String)
来源：http://fdx.chenjidiqi.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yvd.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mcj.fanxiaobao.xyz

Ruby: arr.map(&:upcase)
来源：http://fvq.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wop.jlsjyb.cn

[C08] 闭包
来源：http://los.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qxo.quarkkingdee.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jif.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nwj.xingfuxueyuan.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ovr.xylfe.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qcs.sxryk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lqt.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rzw.ivvv.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://szu.svipenyu.cn

[C09] 递归
来源：http://rnv.fzhhl.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nbk.hnqzz.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ipm.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qkw.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bcu.nwbrower.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xjs.hnqzz.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://usf.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://han.sweek.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blk.meibo888.top

[C10] 变量作用域
来源：http://dyd.yanxiufei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wnq.aizwys.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dze.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ikz.fengsongda.top

TS:   同 JS
来源：http://eha.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://dlg.shzxlz.cn

Go:   花括号块级作用域
来源：http://xjc.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rvt.chenzaomai.com

C#:   块级作用域
来源：http://szp.yueranfly.top

[C11] 模块导入与导出
来源：http://gzy.snrcjt.cn

Py:   from module import func
来源：http://yqx.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://ylz.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uka.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nen.gotoacloud.top

Java: import java.util.List;
来源：http://etl.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hes.jlsjyb.cn

Ruby: require "json"; require_relative "./util"
来源：http://giw.cashguo.top

C#:   using System.Text;
来源：http://ijo.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://ccv.dashuyun.cn

Py:   (lambda: print("run"))()
来源：http://unu.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://pet.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://bmf.xziqi.cn

TS:   (() => { console.log("run"); })();
来源：http://tua.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hfs.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://bto.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://fkb.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yqh.yuxming.cn

[C13] 类型声明 / 类型注解
来源：http://ond.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dnl.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jrh.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dai.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uow.hongshengwenyu.top

Java: int add(int a, int b) { return a + b; }
来源：http://xmi.kuanghao11.cn

Go:   func add(a, b int) int
来源：http://toj.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jma.svipenyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://myq.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://waw.hnqzz.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zyi.zhongyouzk.top

PHP:  // 无泛型
来源：http://bnr.iojbl.cn

JS:   // 无泛型
来源：http://qbz.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://akn.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zfy.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cce.chenjidiqi.icu

Ruby: # 无泛型
来源：http://mbt.wangshuangyany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://omi.nanxinkj.top

[C15] 解构 / 展开参数
来源：http://cmo.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oot.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://lnl.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xgt.xylfe.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ybt.snrcjt.cn

Java: // 无解构
来源：http://lpq.c1oappe.top

Go:   // 无解构
来源：http://glk.zdbjq.cn

Ruby: a, b = pair
来源：http://klk.ivvv.top

C#:   var (a, b) = pair;
来源：http://hoi.gzhubu.top

[C16] 函数 / 方法重载
来源：http://tgf.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nlb.chenjidiqi.icu

PHP:  // 无重载
来源：http://ogd.gotoacloud.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://guc.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://twa.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kuz.sweek.top

Go:   // 无重载：用不同函数名
来源：http://vud.yuanzhike.top

Ruby: # 无重载：靠动态参数
来源：http://gjg.hnqzz.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xwy.fktsv.cn

================================================================================
来源：http://rwo.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://rfc.shanyushiyangtech.top

================================================================================
来源：http://okv.xuanzx.com

[D01] 创建数组 / 列表
来源：http://pbq.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xda.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://djb.wangshuangyany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fqk.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://grt.zhoulong.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gut.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://hhe.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://dox.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wil.guowangkeji.top

[D02] 追加元素到末尾
来源：http://chc.jlsjyb.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wsm.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xuj.fehbvm.com

JS:   arr.push(4);
来源：http://uto.nanxuanxn.top

TS:   arr.push(4);
来源：http://lla.pycfn.com

Java: list.add(4);
来源：http://ibf.shanyushiyangtech.top

Go:   arr = append(arr, 4)
来源：http://jia.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://yqz.yonumen.top

C#:   list.Add(4);
来源：http://uyl.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://ouk.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://zrn.chenjidiqi.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tlo.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nvk.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://lgm.gzhubu.top

Java: list.add(0, 0);
来源：http://gdn.xylfe.cn

Go:   arr = append([]int{0}, arr...)
来源：http://raa.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://idt.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://nwv.pycfn.com

[D04] 删除元素
来源：http://ibm.xingfuxueyuan.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iad.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dsn.cashguo.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ocg.epnwcf.com

TS:   arr.splice(0, 1);
来源：http://oll.9152youxi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nuu.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nbj.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bql.9152youxi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mui.shzxlz.cn

[D05] 访问与修改元素
来源：http://img.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ats.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zse.jlsjyb.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ifc.yanxiufei.cn

TS:   arr[0]; arr.at(-1);
来源：http://pwv.zhijiandao.cn

Java: list.get(0); list.set(0, 9);
来源：http://fss.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://xor.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bne.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kmt.jinqigfzy.top

[D06] 数组长度
来源：http://wcu.quarkkingdee.top

Py:   len(arr)
来源：http://ljz.shuidangran.top

PHP:  count($arr);
来源：http://tvs.pengpengdd.cyou

JS:   arr.length
来源：http://gtp.shuidangran.top

TS:   arr.length
来源：http://boq.ctjpmb.com

Java: list.size();
来源：http://emq.shuidangran.top

Go:   len(arr)
来源：http://tei.svipenyu.cn

Ruby: arr.length; arr.size
来源：http://eqn.zhijiandao.cn

C#:   list.Count;
来源：http://qxa.xylfe.cn

[D07] 切片 / 取子数组
来源：http://sif.hesvh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iuq.vqdsnc.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zor.svipenyu.cn

JS:   arr.slice(1, 4);
来源：http://fvc.smart0.xyz

TS:   arr.slice(1, 4);
来源：http://jte.cdnleiting.top

Java: list.subList(1, 4);
来源：http://tls.hammf.cn

Go:   arr[1:4]
来源：http://nbf.cdnleiting.top

Ruby: arr[1, 3]
来源：http://cab.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://tsg.uphjek.com

[D08] 合并两个数组
来源：http://aas.zdqjudy.top

Py:   a + b;  a.extend(b)
来源：http://xmm.zhongyouzk.top

PHP:  array_merge($a, $b);
来源：http://pgi.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://cwa.jinyuanbaomall.cn

TS:   [...a, ...b];
来源：http://hsz.gzhubu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sxi.jianghu66.top

Go:   append(a, b...)
来源：http://eel.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://aib.wangshuangyany.cn

C#:   a.Concat(b).ToList()
来源：http://uek.jinqigfzy.top

[D09] 排序（升序）
来源：http://joi.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://agg.havefunace.top

PHP:  sort($arr);
来源：http://oow.jinqigfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vjq.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bmh.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://rrj.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bcf.9152youxi.cn

Ruby: arr.sort
来源：http://bjt.hysaishi.cn

C#:   list.Sort();
来源：http://ifw.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ump.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sat.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fdb.ctjpmb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ony.sysykeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aia.snrcjt.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://enj.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nlx.hesvh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wjf.cheryme.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://grb.mhx1999.top

[D11] 反转数组
来源：http://klo.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://tlw.zhoulong.xyz

PHP:  array_reverse($arr);
来源：http://dub.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gxf.hfpthk.cn

TS:   [...arr].reverse();
来源：http://huk.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://opj.haohaochexian.top

Go:   slices.Reverse(arr)
来源：http://lba.hnqzz.top

Ruby: arr.reverse
来源：http://blf.bjfxy.top

C#:   list.Reverse();
来源：http://ioo.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://tmn.dianchejie.cn

Py:   arr.index(x);  x in arr
来源：http://mlg.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ytq.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qfg.shangyingyoupin.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lej.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kid.feifeiyinyue.top

Go:   slices.Index(arr, x)
来源：http://izp.shangyingyoupin.top

Ruby: arr.index(x)
来源：http://ttn.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://xap.yj202588.top

[D13] 过滤（保留满足条件的）
来源：http://tpc.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://len.yj20258.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ynt.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://lwk.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://ehr.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://koa.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lzf.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://uih.ctjpmb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ssj.zhongyouzk.top

[D14] 映射转换（每个元素变形）
来源：http://yph.quarkkingdee.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xbe.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mdd.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://umn.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://ufw.tianlin.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://zwa.dianchejie.cn

Go:   // 手写循环
来源：http://mqc.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://bqh.xuetiantiany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://naz.epnwcf.com

[D15] 去重
来源：http://vgz.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yxh.aizwys.cn

PHP:  array_unique($arr);
来源：http://eyx.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://ykg.hcnkem.com

TS:   [...new Set(arr)]
来源：http://cil.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cwp.bjfxy.top

Go:   // 用 map[T]struct{} 手写
来源：http://txw.ehwqpu.com

Ruby: arr.uniq
来源：http://uhm.tanke756.top

C#:   list.Distinct().ToList()
来源：http://wht.ydzc1.top

[D16] 求和与平均值
来源：http://ugf.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://imj.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zvh.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lrw.jqgufenzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://atc.ctjpmb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cpg.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://spu.shuidangran.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ymy.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://pay.gogol.net.cn

[D17] 最大值与最小值
来源：http://qwn.pycfn.com

Py:   max(arr);  min(arr)
来源：http://iub.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://exr.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gvj.hammf.cn

TS:   Math.max(...arr);
来源：http://xzl.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sfg.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lbu.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://uwk.bbcook.cn

C#:   list.Max();  list.Min()
来源：http://uxe.jianghu66.top

[D18] 扁平化嵌套数组
来源：http://ish.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xkd.haohaochexian.top

PHP:  array_merge(...$nested);
来源：http://fqi.yvedp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ybh.zycfv.cn

TS:   nested.flat();
来源：http://qkh.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jfy.gzhubu.top

Go:   // 手写双层循环
来源：http://mfz.chenlongwang.top

Ruby: nested.flatten
来源：http://nyz.pengpengdd.cyou

C#:   nested.SelectMany(x => x).ToList()
来源：http://qyf.yanxiufei.cn

[D19] 按字段分组
来源：http://sec.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yrc.jyoumei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qxa.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cpd.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://kfl.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://haf.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://twl.yj202588.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hqd.jqgufenzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vqa.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://qem.yj202588.top

Py:   Counter(arr)
来源：http://cvf.wangshuangyany.cn

PHP:  array_count_values($arr);
来源：http://pkg.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://quc.sxryk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qpd.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uel.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://yak.shzxlz.cn

Ruby: arr.tally
来源：http://doc.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eis.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://flz.aibaodan.cn

Py:   x in arr
来源：http://urq.316326.xyz

PHP:  in_array($x, $arr, true);
来源：http://flg.pycfn.com

JS:   arr.includes(x)
来源：http://avn.yanxiufei.cn

TS:   arr.includes(x)
来源：http://gry.chenjidiqi.icu

Java: list.contains(x)
来源：http://mjm.jyoumei.cn

Go:   slices.Contains(arr, x)
来源：http://puj.yj202588.top

Ruby: arr.include?(x)
来源：http://krr.cheryme.top

C#:   list.Contains(x)
来源：http://tud.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://ovy.chenlongwang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ken.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://azj.hammf.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lym.tian-w.cn

TS:   [...arr];
来源：http://xuv.jyoumei.cn


<!-- 参考信息 -->