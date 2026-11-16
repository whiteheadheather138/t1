代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bmn.hnqzz.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gwd.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://faa.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://kud.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://mfh.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://cav.cashguo.top

C#:   f(a: 1, b: 2)
来源：http://iqi.yuxming.cn

[C05] 返回多个值
来源：http://dao.kuanghao11.cn

Py:   return a, b
来源：http://ibh.yangfankeji.com

PHP:  return [$a, $b];
来源：http://jzn.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wse.shzxlz.cn

TS:   return { a, b };
来源：http://ttm.yongpay.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bza.ctjpmb.com

Go:   return a, b
来源：http://ekg.uphjek.com

Ruby: return a, b
来源：http://yfv.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://tqv.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://kke.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://mkf.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://otq.0kj1m.cn

JS:   const square = x => x * x;
来源：http://ucr.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://sjg.chenzaomai.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://noz.hesvh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zhc.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://xqm.zhixingplan.top

C#:   Func<int, int> square = x => x * x;
来源：http://qts.hammf.cn

[C07] 把函数作为参数传入
来源：http://unl.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xnk.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://jhs.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uza.hammf.cn

TS:   arr.map(String)
来源：http://gjc.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hkj.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rbs.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://kax.vqdsnc.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gvo.sufxvd.cn

[C08] 闭包
来源：http://kmd.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jlt.epnwcf.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dmc.zhoulong.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nfo.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ptx.nwbrower.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://enf.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nef.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://awj.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ydx.xingfuxueyuan.xyz

[C09] 递归
来源：http://psz.zycfv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://frv.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://caw.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jyx.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ydq.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://knz.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bbj.gzhubu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bbw.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://npj.c1oappe.top

[C10] 变量作用域
来源：http://bxe.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://geq.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://roj.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qxk.zdqjudy.top

TS:   同 JS
来源：http://jle.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://ahe.cucudq.cn

Go:   花括号块级作用域
来源：http://fao.guannengcc.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ghh.yueranfly.top

C#:   块级作用域
来源：http://aqq.cucudq.cn

[C11] 模块导入与导出
来源：http://zna.quarkkingdee.top

Py:   from module import func
来源：http://rqh.hysaishi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tak.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qjx.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kfm.sxryk.cn

Java: import java.util.List;
来源：http://myc.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yeb.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://aha.hnxiangtu.top

C#:   using System.Text;
来源：http://hab.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://ubb.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://wyi.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://oyq.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://kps.yangfankeji.com

TS:   (() => { console.log("run"); })();
来源：http://mfu.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hts.zhaomingkeji.xyz

Go:   func() { fmt.Println("run") }()
来源：http://tha.0kj1m.cn

Ruby: -> { puts "run" }.call
来源：http://iex.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xip.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://gwh.gogol.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://awo.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ely.316326.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ezh.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xpj.hysaishi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wti.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://egg.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gtc.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://fda.zhengqikj.top

[C14] 泛型函数
来源：http://etp.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uct.ybcxt.top

PHP:  // 无泛型
来源：http://wzk.sjlbkw.cn

JS:   // 无泛型
来源：http://osz.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oqi.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zcv.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ufb.yj20258888.top

Ruby: # 无泛型
来源：http://rqr.nanxuanxn.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qzr.yonumen.top

[C15] 解构 / 展开参数
来源：http://qvq.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mhf.guowangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://goy.aizwys.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hsa.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iiw.c1oappe.top

Java: // 无解构
来源：http://kzw.zhaomingkeji.xyz

Go:   // 无解构
来源：http://pga.jinqigfzy.top

Ruby: a, b = pair
来源：http://hvp.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://auo.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://jny.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://djl.yanxiufei.cn

PHP:  // 无重载
来源：http://bvr.mhx1999.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pwd.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://crd.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cik.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://zci.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://ifq.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ani.zhengqikj.top

================================================================================
来源：http://chn.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://wgf.shanyushiyangtech.top

================================================================================
来源：http://woi.cashguo.top

[D01] 创建数组 / 列表
来源：http://pnj.xuanzx.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://uob.iojbl.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://akr.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gme.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yjd.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wja.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://jhp.shuidangran.top

Ruby: arr = [1, 2, 3]
来源：http://jdl.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nhi.xuanzx.com

[D02] 追加元素到末尾
来源：http://dpj.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://osx.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bza.svipenyu.cn

JS:   arr.push(4);
来源：http://mjv.hesvh.cn

TS:   arr.push(4);
来源：http://pha.jlsjyb.cn

Java: list.add(4);
来源：http://pwn.chenjidiqi.icu

Go:   arr = append(arr, 4)
来源：http://sfl.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://neq.cucudq.cn

C#:   list.Add(4);
来源：http://uhw.hesvh.cn

[D03] 在指定位置插入元素
来源：http://eah.nwbrower.top

Py:   arr.insert(0, 0)
来源：http://nbe.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lbe.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rro.dashuyun.cn

TS:   arr.splice(0, 0, 0);
来源：http://kaw.bbcook.cn

Java: list.add(0, 0);
来源：http://qte.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://ruh.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gkp.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://esg.zhongyouzk.top

[D04] 删除元素
来源：http://cwh.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zwq.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rhc.yj20258888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rza.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://ipv.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ccb.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vwj.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vgk.bjfxy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qah.fzhhl.top

[D05] 访问与修改元素
来源：http://fge.52xcode.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://enc.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gla.havefunace.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cbn.jqgfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://gxx.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://jgv.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://mxt.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dza.yfazqb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yly.fktsv.cn

[D06] 数组长度
来源：http://ubw.yvedp.cn

Py:   len(arr)
来源：http://msh.hcnkem.com

PHP:  count($arr);
来源：http://fuo.hysaishi.cn

JS:   arr.length
来源：http://izb.quarkkingdee.top

TS:   arr.length
来源：http://mlv.birdmap.top

Java: list.size();
来源：http://hvj.zhongyouzk.top

Go:   len(arr)
来源：http://dig.sxryk.cn

Ruby: arr.length; arr.size
来源：http://mtq.aizwys.cn

C#:   list.Count;
来源：http://ckh.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://ybw.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rpi.gzhubu.top

PHP:  array_slice($arr, 1, 3);
来源：http://tfs.c1oappe.top

JS:   arr.slice(1, 4);
来源：http://oer.fengsongda.top

TS:   arr.slice(1, 4);
来源：http://ukf.ppjwa.cn

Java: list.subList(1, 4);
来源：http://sbd.kuanghao11.cn

Go:   arr[1:4]
来源：http://rem.tarul.cn

Ruby: arr[1, 3]
来源：http://avt.ydjk.org.cn

C#:   list.GetRange(1, 3);
来源：http://xzh.hnqzz.top

[D08] 合并两个数组
来源：http://ynb.tarul.cn

Py:   a + b;  a.extend(b)
来源：http://ahs.yuxming.cn

PHP:  array_merge($a, $b);
来源：http://xei.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://aic.andypj.xyz

TS:   [...a, ...b];
来源：http://xko.xylfe.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uha.gaohongyu789.top

Go:   append(a, b...)
来源：http://ioi.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://jho.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://lbm.ctjpmb.com

[D09] 排序（升序）
来源：http://usy.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://qem.vqdsnc.cn

PHP:  sort($arr);
来源：http://qua.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kmo.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rdg.jinqigufen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cow.ehwqpu.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mlp.zhengqikj.top

Ruby: arr.sort
来源：http://wkp.dashuyun.cn

C#:   list.Sort();
来源：http://rtw.birdmap.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lgz.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oyr.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gis.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pqo.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ern.zdbjq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pcu.feifeiyinyue.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xqh.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qeo.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ian.yueranfly.top

[D11] 反转数组
来源：http://ejn.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://rql.yueranfly.top

PHP:  array_reverse($arr);
来源：http://aes.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mbz.daxiang520.top

TS:   [...arr].reverse();
来源：http://ihg.havefunace.top

Java: Collections.reverse(list);
来源：http://cep.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://lev.fehbvm.com

Ruby: arr.reverse
来源：http://cxx.xziqi.cn

C#:   list.Reverse();
来源：http://xjb.hnqzz.top

[D12] 查找元素下标
来源：http://emt.shuidangran.top

Py:   arr.index(x);  x in arr
来源：http://pok.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qnl.pycfn.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eii.xuetiantiany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ehk.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://orw.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://stl.yuanzhike.top

Ruby: arr.index(x)
来源：http://mhr.yongpay.top

C#:   list.IndexOf(x);
来源：http://fbv.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://sqf.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ype.yfazqb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zqi.jianghu66.top

JS:   arr.filter(x => x > 3)
来源：http://bhc.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://nbw.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qok.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uqe.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://vtk.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://wib.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://zho.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gkl.cqqwz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eyn.xylfe.cn

JS:   arr.map(x => x * 2)
来源：http://pft.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://vga.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://idl.nwbrower.top

Go:   // 手写循环
来源：http://sui.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lwr.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://qvx.yuanzhike.top

[D15] 去重
来源：http://wjq.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zgp.xingfuxueyuan.xyz

PHP:  array_unique($arr);
来源：http://vlu.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://bql.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://oyg.vqdsnc.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hcs.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://qbh.zycfv.cn

Ruby: arr.uniq
来源：http://cgu.haohaochexian.top

C#:   list.Distinct().ToList()
来源：http://brt.chenlongwang.top

[D16] 求和与平均值
来源：http://noq.fehbvm.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sdk.yvedp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pgi.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ggf.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tpk.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://plz.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://sey.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rmf.tianlin.xyz

C#:   list.Sum();  list.Average()
来源：http://oqy.yueranfly.top

[D17] 最大值与最小值
来源：http://qob.andypj.xyz

Py:   max(arr);  min(arr)
来源：http://dzv.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://aub.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mmb.chenzaomai.com

TS:   Math.max(...arr);
来源：http://iqi.bjfxy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://clo.zdbjq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mza.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://kkl.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://bki.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://gga.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tam.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://ama.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qsv.andypj.xyz

TS:   nested.flat();
来源：http://ljt.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tks.chenlongwang.top

Go:   // 手写双层循环
来源：http://bwa.dianchejie.cn

Ruby: nested.flatten
来源：http://tgt.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yci.mhx1999.top

[D19] 按字段分组
来源：http://nzt.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yyh.zdbjq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://upe.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://chp.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zjz.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wpd.yuanzhike.top

Go:   // 手写 map[string][]T
来源：http://dhn.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sai.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vwc.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://cpa.jqgfzy.top

Py:   Counter(arr)
来源：http://byv.gzhubu.top

PHP:  array_count_values($arr);
来源：http://vpy.guowangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bvn.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://edw.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pwo.gzhubu.top

Go:   // 手写 map[T]int
来源：http://juz.dashuyun.cn

Ruby: arr.tally
来源：http://tjo.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://woz.ivvv.top

[D21] 判断是否包含某元素
来源：http://ccg.fktsv.cn

Py:   x in arr
来源：http://fsg.jinghuilouyu.cn


<!-- 参考信息 -->