代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nyh.feifeiyinyue.top

TS:   arr.map(String)
来源：http://mip.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://znw.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://udz.yj20258.top

Ruby: arr.map(&:upcase)
来源：http://nec.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://olk.hnxiangtu.top

[C08] 闭包
来源：http://gip.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vek.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dld.guowangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://egu.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://svg.hywenlv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gcp.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://smo.xuanzx.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xfp.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nhj.cqqwz.cn

[C09] 递归
来源：http://ttg.bjfxy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uqk.pycfn.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://toa.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tkw.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eet.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dkk.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://msh.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vlp.gogol.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ozd.uphjek.com

[C10] 变量作用域
来源：http://iuc.chenlongwang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tty.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ogf.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kse.jinyuanbaomall.cn

TS:   同 JS
来源：http://ymj.iojbl.cn

Java: 方法内为块级作用域
来源：http://xhb.xuanzx.com

Go:   花括号块级作用域
来源：http://bii.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://awb.shuidangran.top

C#:   块级作用域
来源：http://kyv.sweek.top

[C11] 模块导入与导出
来源：http://bie.yangfankeji.com

Py:   from module import func
来源：http://qrc.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ban.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jug.andypj.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ueh.bjfxy.top

Java: import java.util.List;
来源：http://gay.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oss.yongpay.top

Ruby: require "json"; require_relative "./util"
来源：http://njo.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://xgh.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://vhf.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://iuo.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://owp.tarul.cn

JS:   (() => { console.log("run"); })();
来源：http://ifp.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://pth.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nmm.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://mni.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://ezz.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://czj.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://kig.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ndv.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mqn.hesvh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ymi.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zoo.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cgs.iojbl.cn

Go:   func add(a, b int) int
来源：http://lhj.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vmk.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://pcc.hesvh.cn

[C14] 泛型函数
来源：http://yxb.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wnq.cheryme.top

PHP:  // 无泛型
来源：http://czy.9152youxi.cn

JS:   // 无泛型
来源：http://vtx.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ncw.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jke.gzhubu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://raz.sjlbkw.cn

Ruby: # 无泛型
来源：http://sxo.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kxi.pycfn.com

[C15] 解构 / 展开参数
来源：http://cav.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uas.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://wgj.fktsv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zuk.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zxs.chenzaomai.com

Java: // 无解构
来源：http://zgb.hnxiangtu.top

Go:   // 无解构
来源：http://akh.shanyushiyangkeji.top

Ruby: a, b = pair
来源：http://xoz.ctjpmb.com

C#:   var (a, b) = pair;
来源：http://kyh.smart0.xyz

[C16] 函数 / 方法重载
来源：http://wjg.andypj.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gqc.chenzaomai.com

PHP:  // 无重载
来源：http://rmj.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ile.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://aya.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bed.shangyingyoupin.top

Go:   // 无重载：用不同函数名
来源：http://xzx.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://mer.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://frt.ctjpmb.com

================================================================================
来源：http://cyh.sweek.top

D. 数组 / 列表 / 集合
来源：http://umh.tianlin.xyz

================================================================================
来源：http://rag.shanyushiyangtech.top

[D01] 创建数组 / 列表
来源：http://djb.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mcz.fanxiaobao.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://apq.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://aek.gogol.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dpl.nanxinkj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uxf.bjfxy.top

Go:   arr := []int{1, 2, 3}
来源：http://ovc.andypj.xyz

Ruby: arr = [1, 2, 3]
来源：http://jyq.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://czh.yuxming.cn

[D02] 追加元素到末尾
来源：http://ply.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jgo.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yjx.jqgfzy.top

JS:   arr.push(4);
来源：http://uhl.sjlbkw.cn

TS:   arr.push(4);
来源：http://ffv.redwolf501.top

Java: list.add(4);
来源：http://tbl.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://liq.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://vdv.tanke756.top

C#:   list.Add(4);
来源：http://obn.zhaomingkeji.xyz

[D03] 在指定位置插入元素
来源：http://ykf.zhoulong.xyz

Py:   arr.insert(0, 0)
来源：http://wno.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://umi.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ibb.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://bfv.aizwys.cn

Java: list.add(0, 0);
来源：http://ckd.zdqjudy.top

Go:   arr = append([]int{0}, arr...)
来源：http://ohu.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xur.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://wmj.xziqi.cn

[D04] 删除元素
来源：http://wyn.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dca.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wlj.gaohongyu789.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ynq.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://fdd.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bfz.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rlq.ivvv.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ido.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://swg.ydzc1.top

[D05] 访问与修改元素
来源：http://lfv.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yln.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cvu.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xnc.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://nce.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://zoy.yj202588.top

Go:   arr[0]; arr[0] = 9
来源：http://zcd.ybcxt.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pfc.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ufl.snrcjt.cn

[D06] 数组长度
来源：http://wni.epnwcf.com

Py:   len(arr)
来源：http://fbt.xziqi.cn

PHP:  count($arr);
来源：http://upa.jinyuanbaomall.cn

JS:   arr.length
来源：http://xmm.ppjwa.cn

TS:   arr.length
来源：http://rfu.sysykeji.top

Java: list.size();
来源：http://iib.jinqigufen.top

Go:   len(arr)
来源：http://ocy.sweek.top

Ruby: arr.length; arr.size
来源：http://lqt.jqgfzy.top

C#:   list.Count;
来源：http://blb.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://itz.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wry.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xgo.tarul.cn

JS:   arr.slice(1, 4);
来源：http://pth.ivvv.top

TS:   arr.slice(1, 4);
来源：http://pil.tarul.cn

Java: list.subList(1, 4);
来源：http://uym.quarkkingdee.top

Go:   arr[1:4]
来源：http://cev.0kj1m.cn

Ruby: arr[1, 3]
来源：http://xnx.guowangkeji.top

C#:   list.GetRange(1, 3);
来源：http://oqh.316326.xyz

[D08] 合并两个数组
来源：http://qtw.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://fse.cheryme.top

PHP:  array_merge($a, $b);
来源：http://lkx.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://led.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://mnt.jyoumei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zth.gotoacloud.top

Go:   append(a, b...)
来源：http://flm.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://lhy.iojbl.cn

C#:   a.Concat(b).ToList()
来源：http://skw.9152youxi.cn

[D09] 排序（升序）
来源：http://cdr.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://yzx.jqgfzy.top

PHP:  sort($arr);
来源：http://vwj.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bcs.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fcm.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ooj.jianghu66.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tgn.sufxvd.cn

Ruby: arr.sort
来源：http://vir.jlsjyb.cn

C#:   list.Sort();
来源：http://jlh.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://esj.yj202588.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cpt.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bms.jianghu66.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cip.redwolf501.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qgw.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iym.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cog.cheryme.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cth.epnwcf.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lgd.jlsjyb.cn

[D11] 反转数组
来源：http://meg.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://pgw.gogol.net.cn

PHP:  array_reverse($arr);
来源：http://eqw.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bot.shangyingyoupin.top

TS:   [...arr].reverse();
来源：http://eud.kuanghao11.cn

Java: Collections.reverse(list);
来源：http://fwy.hnqzz.top

Go:   slices.Reverse(arr)
来源：http://zus.tanke756.top

Ruby: arr.reverse
来源：http://ccf.hnqzz.top

C#:   list.Reverse();
来源：http://hpq.zhoulong.xyz

[D12] 查找元素下标
来源：http://lzv.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://uwk.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bnv.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qot.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ygs.epnwcf.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fqg.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://dxh.fzhhl.top

Ruby: arr.index(x)
来源：http://nni.jlsjyb.cn

C#:   list.IndexOf(x);
来源：http://kpz.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://vhk.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://emx.xingfuxueyuan.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qko.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://hez.zhijiandao.cn

TS:   arr.filter(x => x > 3)
来源：http://rkl.fengsongda.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lnp.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ckg.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dbc.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gxw.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://vtk.tarul.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uel.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bqz.yvedp.cn

JS:   arr.map(x => x * 2)
来源：http://aoz.ppjwa.cn

TS:   arr.map(x => x * 2)
来源：http://ihx.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lck.zdqjudy.top

Go:   // 手写循环
来源：http://szu.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yma.zhengqikj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tdl.52xcode.cn

[D15] 去重
来源：http://ofj.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lbu.bbcook.cn

PHP:  array_unique($arr);
来源：http://vdk.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://ocb.yongpay.top

TS:   [...new Set(arr)]
来源：http://gym.yueranfly.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wna.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rni.tian-w.cn

Ruby: arr.uniq
来源：http://ldh.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://vyf.pengpengdd.cyou

[D16] 求和与平均值
来源：http://zdb.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ghv.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bpa.sweek.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dag.yonumen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://crx.hesvh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xav.aibaodan.cn

Go:   // 手写循环累加
来源：http://gmt.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fvm.yanxiufei.cn

C#:   list.Sum();  list.Average()
来源：http://rpw.chenlongwang.top

[D17] 最大值与最小值
来源：http://vsx.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://lhf.hesvh.cn

PHP:  max($arr);  min($arr);
来源：http://wjq.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://snu.jianghu66.top

TS:   Math.max(...arr);
来源：http://isg.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://dhv.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vhd.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://tab.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://adh.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://nph.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nku.zycfv.cn

PHP:  array_merge(...$nested);
来源：http://jnc.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://adr.cdnleiting.top

TS:   nested.flat();
来源：http://cyk.shuidangran.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nye.zycfv.cn

Go:   // 手写双层循环
来源：http://yqw.sweek.top

Ruby: nested.flatten
来源：http://uap.havefunace.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qza.yanxiufei.cn

[D19] 按字段分组
来源：http://wpr.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dbb.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://caf.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uia.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vsw.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ovj.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://ctu.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nnf.zhaomingkeji.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ejq.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://ikl.nanxinkj.top

Py:   Counter(arr)
来源：http://tym.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://xto.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://geq.ehwqpu.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hnb.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kzp.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://khs.xingfuxueyuan.xyz

Ruby: arr.tally
来源：http://tti.zhijiandao.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ctf.guannengcc.top

[D21] 判断是否包含某元素
来源：http://xag.cdnleiting.top

Py:   x in arr
来源：http://xzj.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://tiv.aizwys.cn

JS:   arr.includes(x)
来源：http://wpa.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://lif.yanxiufei.cn

Java: list.contains(x)
来源：http://hpa.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://mlh.c1oappe.top

Ruby: arr.include?(x)
来源：http://bkj.havefunace.top

C#:   list.Contains(x)
来源：http://kuu.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://oac.jqgufenzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ivs.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ncz.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eaf.havefunace.top

TS:   [...arr];
来源：http://fnn.yuxming.cn

Java: new ArrayList<>(list);
来源：http://ftm.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://ffw.yueranfly.top

Ruby: arr.dup;  arr.clone
来源：http://vid.hcnkem.com

C#:   new List<int>(list);
来源：http://nfg.cashguo.top

[D23] reduce 累积计算
来源：http://del.hesvh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cnw.fanxiaobao.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lyp.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ozy.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lcn.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lnz.quarkkingdee.top

Go:   // 手写循环
来源：http://zrp.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://viu.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://izr.ppjwa.cn

[D24] 字典 / Map 基本操作
来源：http://zoq.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pdd.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://drx.uphjek.com


<!-- 参考信息 -->