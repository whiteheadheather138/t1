代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://plg.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://mel.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://msf.cucudq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sgn.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gwj.zhaomingkeji.xyz

TS:   arr.map(String)
来源：http://fmm.yuanzhike.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kvf.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qyg.smart0.xyz

Ruby: arr.map(&:upcase)
来源：http://qbt.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pck.ywan-chungtsiang.top

[C08] 闭包
来源：http://yvb.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oum.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mnq.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pla.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dxm.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mzi.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nod.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iev.jqgufenzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xnx.52xcode.cn

[C09] 递归
来源：http://ifl.zdbjq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vwv.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gif.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zvj.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://luy.hnxiangtu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ijn.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yfh.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gbv.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hrq.hammf.cn

[C10] 变量作用域
来源：http://tff.xylfe.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pcs.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gvn.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://apl.ydzc1.top

TS:   同 JS
来源：http://usd.haohaochexian.top

Java: 方法内为块级作用域
来源：http://nso.xylfe.cn

Go:   花括号块级作用域
来源：http://rfw.chenzaomai.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mlw.chenjidiqi.icu

C#:   块级作用域
来源：http://hvf.gaohongyu789.top

[C11] 模块导入与导出
来源：http://cjd.smart0.xyz

Py:   from module import func
来源：http://vae.zycfv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ohw.pengpengdd.cyou

JS:   export default function f() {};  import f from "./m.js";
来源：http://ugr.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qdb.smart0.xyz

Java: import java.util.List;
来源：http://yzl.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sam.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://iil.sweek.top

C#:   using System.Text;
来源：http://kpq.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://jna.birdmap.top

Py:   (lambda: print("run"))()
来源：http://wem.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://sbs.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://kle.fehbvm.com

TS:   (() => { console.log("run"); })();
来源：http://cel.yuxming.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vwx.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://pae.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://muk.ivvv.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yvr.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://rwx.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jjh.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bfv.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qef.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rgd.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://xwn.dianchejie.cn

Go:   func add(a, b int) int
来源：http://zyt.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tzf.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://qbe.wangdashe.top

[C14] 泛型函数
来源：http://ene.aibaodan.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cvd.gotoacloud.top

PHP:  // 无泛型
来源：http://bcc.sweek.top

JS:   // 无泛型
来源：http://pha.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dde.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hmk.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qeh.nwbrower.top

Ruby: # 无泛型
来源：http://dam.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mno.jianghu66.top

[C15] 解构 / 展开参数
来源：http://yzx.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ozj.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://xem.fktsv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fhy.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cbu.yueranfly.top

Java: // 无解构
来源：http://kfk.fzhhl.top

Go:   // 无解构
来源：http://bvt.0kj1m.cn

Ruby: a, b = pair
来源：http://yoc.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://mck.52xcode.cn

[C16] 函数 / 方法重载
来源：http://wrz.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nrv.cheryme.top

PHP:  // 无重载
来源：http://vnh.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://juf.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://zgi.xylfe.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nsv.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://wje.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://mok.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vnb.ehwqpu.com

================================================================================
来源：http://lea.yj20258.top

D. 数组 / 列表 / 集合
来源：http://anu.hesvh.cn

================================================================================
来源：http://sxk.wangshuangyany.cn

[D01] 创建数组 / 列表
来源：http://gbc.tianlin.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://fdf.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://alx.yangfankeji.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dis.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fow.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ljb.fktsv.cn

Go:   arr := []int{1, 2, 3}
来源：http://zpg.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://cnk.chenlongwang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xxr.tanke756.top

[D02] 追加元素到末尾
来源：http://vss.dashuyun.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fuy.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xpj.0kj1m.cn

JS:   arr.push(4);
来源：http://ibw.jinyuanbaomall.cn

TS:   arr.push(4);
来源：http://wwz.dianchejie.cn

Java: list.add(4);
来源：http://sup.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://pty.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://bkn.pycfn.com

C#:   list.Add(4);
来源：http://ztv.hammf.cn

[D03] 在指定位置插入元素
来源：http://yit.gogol.net.cn

Py:   arr.insert(0, 0)
来源：http://xgx.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cbj.jinqigufen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yzy.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://idq.sxryk.cn

Java: list.add(0, 0);
来源：http://khc.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bve.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yjl.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://btc.cdnleiting.top

[D04] 删除元素
来源：http://tzz.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://egs.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rat.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rgn.yj20258.top

TS:   arr.splice(0, 1);
来源：http://xdh.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pfp.jinyuanbaomall.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://arq.zhengqikj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fzx.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rfk.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://gck.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ead.shanyushiyangtech.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tzo.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ffh.feifeiyinyue.top

TS:   arr[0]; arr.at(-1);
来源：http://ohy.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://tas.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://vog.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bgh.ppjwa.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rlq.hammf.cn

[D06] 数组长度
来源：http://dud.havefunace.top

Py:   len(arr)
来源：http://rii.vehdjk.com

PHP:  count($arr);
来源：http://fdg.chenjidiqi.icu

JS:   arr.length
来源：http://aiu.yj20258888.top

TS:   arr.length
来源：http://vnp.redwolf501.top

Java: list.size();
来源：http://jeh.xylfe.cn

Go:   len(arr)
来源：http://bpp.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://ieh.cashguo.top

C#:   list.Count;
来源：http://uzl.shuidangran.top

[D07] 切片 / 取子数组
来源：http://rnf.fktsv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://awo.hysaishi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xdt.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://ztb.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://bkl.shuidangran.top

Java: list.subList(1, 4);
来源：http://wrj.zhixingplan.top

Go:   arr[1:4]
来源：http://tvh.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://myk.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://bit.9152youxi.cn

[D08] 合并两个数组
来源：http://yki.fengsongda.top

Py:   a + b;  a.extend(b)
来源：http://nyv.ydzc1.top

PHP:  array_merge($a, $b);
来源：http://zro.hnxiangtu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tri.zhoulong.xyz

TS:   [...a, ...b];
来源：http://xjq.gogol.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dnz.zhijiandao.cn

Go:   append(a, b...)
来源：http://mjv.zhongyouzk.top

Ruby: a + b;  a.concat(b)
来源：http://ynb.cucudq.cn

C#:   a.Concat(b).ToList()
来源：http://aai.daxiang520.top

[D09] 排序（升序）
来源：http://xjc.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://nzr.xylfe.cn

PHP:  sort($arr);
来源：http://yyp.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dbl.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://owf.yj20258.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ahr.jianghu66.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mlf.ydjk.org.cn

Ruby: arr.sort
来源：http://wgf.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://aec.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://xqm.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aya.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cjo.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jgk.mhx1999.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lcn.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qzv.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fmk.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cck.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fkn.snrcjt.cn

[D11] 反转数组
来源：http://gxo.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nxj.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://seb.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://msc.chenlongwang.top

TS:   [...arr].reverse();
来源：http://hdx.snrcjt.cn

Java: Collections.reverse(list);
来源：http://dle.fzhhl.top

Go:   slices.Reverse(arr)
来源：http://ckb.hcnkem.com

Ruby: arr.reverse
来源：http://xyy.sjlbkw.cn

C#:   list.Reverse();
来源：http://iij.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://doi.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://ayd.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ipj.fktsv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zts.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nui.hammf.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://reh.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://uzs.yj20258888.top

Ruby: arr.index(x)
来源：http://esp.hnqzz.top

C#:   list.IndexOf(x);
来源：http://rgx.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://qdp.jinyuanbaomall.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ufa.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pot.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://mwe.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://egg.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jee.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://grk.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://mxk.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://flf.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://ofw.gogol.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kej.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yni.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://odq.sufxvd.cn

TS:   arr.map(x => x * 2)
来源：http://yns.shanyushiyangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cju.xziqi.cn

Go:   // 手写循环
来源：http://wlo.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bae.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fsw.0kj1m.cn

[D15] 去重
来源：http://mue.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mox.ywan-chungtsiang.top

PHP:  array_unique($arr);
来源：http://wrl.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://onh.xingfuxueyuan.xyz

TS:   [...new Set(arr)]
来源：http://zvw.fktsv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ffn.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://dog.bbcook.cn

Ruby: arr.uniq
来源：http://svw.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://fdm.ybcxt.top

[D16] 求和与平均值
来源：http://eqf.fengsongda.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ezt.yanxiufei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qhh.guowangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ope.jqgufenzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fhl.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ulo.kuanghao11.cn

Go:   // 手写循环累加
来源：http://uav.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eju.dashuyun.cn

C#:   list.Sum();  list.Average()
来源：http://wmo.fengsongda.top

[D17] 最大值与最小值
来源：http://hcs.nanxuanxn.top

Py:   max(arr);  min(arr)
来源：http://zox.cashguo.top

PHP:  max($arr);  min($arr);
来源：http://agb.xinyue.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gfs.0kj1m.cn

TS:   Math.max(...arr);
来源：http://yrm.jinqigufen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fjw.tarul.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://chh.wangshuangyany.cn

Ruby: arr.max;  arr.min
来源：http://fmw.fktsv.cn

C#:   list.Max();  list.Min()
来源：http://dkt.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://luw.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ozz.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://luw.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sdc.zdqjudy.top

TS:   nested.flat();
来源：http://dlu.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rin.iojbl.cn

Go:   // 手写双层循环
来源：http://bbb.9152youxi.cn

Ruby: nested.flatten
来源：http://gcg.yfazqb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://buv.guannengcc.top

[D19] 按字段分组
来源：http://wmm.fktsv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xmd.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://edr.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fvf.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jes.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lnf.tanke756.top

Go:   // 手写 map[string][]T
来源：http://kor.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xnj.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oyw.dashuyun.cn

[D20] 统计每个元素出现次数
来源：http://ata.sweek.top

Py:   Counter(arr)
来源：http://jbf.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://csl.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cvt.jlsjyb.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://otd.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://asq.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://bbr.hcnkem.com

Ruby: arr.tally
来源：http://ddl.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nly.zhaomingkeji.xyz

[D21] 判断是否包含某元素
来源：http://zgu.shangyingyoupin.top

Py:   x in arr
来源：http://oje.epnwcf.com

PHP:  in_array($x, $arr, true);
来源：http://ijc.sxryk.cn

JS:   arr.includes(x)
来源：http://xhf.hongshengwenyu.top

TS:   arr.includes(x)
来源：http://nhv.tanke756.top

Java: list.contains(x)
来源：http://iys.guowangkeji.top

Go:   slices.Contains(arr, x)
来源：http://ffw.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://irc.aibaodan.cn

C#:   list.Contains(x)
来源：http://kmf.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://ane.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://trm.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jfp.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://voy.sjlbkw.cn

TS:   [...arr];
来源：http://ejq.pengpengdd.cyou

Java: new ArrayList<>(list);
来源：http://cre.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://err.xingfuxueyuan.xyz

Ruby: arr.dup;  arr.clone
来源：http://eca.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://dnq.fengsongda.top

[D23] reduce 累积计算
来源：http://spl.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dfl.uphjek.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lbg.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cvy.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bma.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fvh.feifeiyinyue.top

Go:   // 手写循环
来源：http://trk.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aoj.hnxiangtu.top


<!-- 参考信息 -->