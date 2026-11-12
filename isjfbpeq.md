代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://opa.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cbp.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rbf.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zld.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qgq.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qzo.ywan-chungtsiang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vfy.hywenlv.cn

[C09] 递归
来源：http://wtv.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dnu.zhijiandao.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dnt.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lsv.shanyushiyangtech.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rws.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qdw.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aod.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hqp.yuanzhike.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cay.jqgfzy.top

[C10] 变量作用域
来源：http://ehm.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://drx.yfazqb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lqt.tarul.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aps.xingfuxueyuan.xyz

TS:   同 JS
来源：http://kxx.yvedp.cn

Java: 方法内为块级作用域
来源：http://kzd.zhoulong.xyz

Go:   花括号块级作用域
来源：http://chi.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nte.epnwcf.com

C#:   块级作用域
来源：http://sqj.sysykeji.top

[C11] 模块导入与导出
来源：http://lov.guannengcc.top

Py:   from module import func
来源：http://jqz.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://ccf.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ngb.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xhc.vehdjk.com

Java: import java.util.List;
来源：http://qaa.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blc.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://iro.zhengqikj.top

C#:   using System.Text;
来源：http://klu.hysaishi.cn

[C12] 立即执行函数 IIFE
来源：http://dja.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://ckq.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://iqi.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://ykk.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://ikj.yuxming.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wvy.tianlin.xyz

Go:   func() { fmt.Println("run") }()
来源：http://gto.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://rfc.mhx1999.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rxg.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://dfw.hfpthk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oxo.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cwx.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bik.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vlm.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://fyh.cashguo.top

Go:   func add(a, b int) int
来源：http://jva.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://weh.cheryme.top

C#:   int Add(int a, int b) => a + b;
来源：http://uej.snrcjt.cn

[C14] 泛型函数
来源：http://egq.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://png.hfpthk.cn

PHP:  // 无泛型
来源：http://bee.jqgufenzy.top

JS:   // 无泛型
来源：http://jze.bbcook.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tlw.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://png.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://njn.daria6918.cn

Ruby: # 无泛型
来源：http://qwr.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gdn.haohaochexian.top

[C15] 解构 / 展开参数
来源：http://luj.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hee.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://evo.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kyi.yuxming.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ffx.shanyushiyangtech.top

Java: // 无解构
来源：http://vqb.sufxvd.cn

Go:   // 无解构
来源：http://etm.hfpthk.cn

Ruby: a, b = pair
来源：http://wmm.gotoacloud.top

C#:   var (a, b) = pair;
来源：http://djt.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://yoi.xingfuxueyuan.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bfq.redwolf501.top

PHP:  // 无重载
来源：http://udl.shangyingyoupin.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://udh.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://tyo.ywan-chungtsiang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dxw.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://oym.cheryme.top

Ruby: # 无重载：靠动态参数
来源：http://yzs.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://woj.daria6918.cn

================================================================================
来源：http://xuk.jyoumei.cn

D. 数组 / 列表 / 集合
来源：http://wbv.andypj.xyz

================================================================================
来源：http://dcb.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://leb.yongpay.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://huf.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ruc.zhixingplan.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://skl.xingfuxueyuan.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://vol.uphjek.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lnt.daxiang520.top

Go:   arr := []int{1, 2, 3}
来源：http://yla.mhx1999.top

Ruby: arr = [1, 2, 3]
来源：http://gcb.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xtr.sufxvd.cn

[D02] 追加元素到末尾
来源：http://blm.jinghuilouyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://imu.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gji.yonumen.top

JS:   arr.push(4);
来源：http://byy.redwolf501.top

TS:   arr.push(4);
来源：http://ird.zhengqikj.top

Java: list.add(4);
来源：http://ywi.zhixingplan.top

Go:   arr = append(arr, 4)
来源：http://kgg.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://ljc.nanxinkj.top

C#:   list.Add(4);
来源：http://udo.redwolf501.top

[D03] 在指定位置插入元素
来源：http://jgu.52xcode.cn

Py:   arr.insert(0, 0)
来源：http://hhh.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://upb.yuanzhike.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pbd.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://khm.hcnkem.com

Java: list.add(0, 0);
来源：http://hrd.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://vvw.xuetiantiany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sru.xuanzx.com

C#:   list.Insert(0, 0);
来源：http://brq.hnxiangtu.top

[D04] 删除元素
来源：http://phm.hesvh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kqq.zhiwuduotai.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://udq.jlsjyb.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wyg.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://jyc.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aqa.52xcode.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ivx.mhx1999.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xpn.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lbq.jinqigfzy.top

[D05] 访问与修改元素
来源：http://sdn.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tjf.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://enz.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kmm.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://nrr.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://utm.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://bjo.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ivl.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://twc.shuidangran.top

[D06] 数组长度
来源：http://ogj.quarkkingdee.top

Py:   len(arr)
来源：http://tag.havefunace.top

PHP:  count($arr);
来源：http://hea.smart0.xyz

JS:   arr.length
来源：http://rnp.havefunace.top

TS:   arr.length
来源：http://ayk.shanyushiyangkeji.top

Java: list.size();
来源：http://hnq.jinyuanbaomall.cn

Go:   len(arr)
来源：http://pox.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://icn.jinqigufen.top

C#:   list.Count;
来源：http://yci.daria6918.cn

[D07] 切片 / 取子数组
来源：http://aai.dashuyun.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://quk.hysaishi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uga.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://qkx.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://bhs.yj20258888.top

Java: list.subList(1, 4);
来源：http://olf.sweek.top

Go:   arr[1:4]
来源：http://vuu.sxryk.cn

Ruby: arr[1, 3]
来源：http://wcj.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://drd.zdbjq.cn

[D08] 合并两个数组
来源：http://ozx.daria6918.cn

Py:   a + b;  a.extend(b)
来源：http://cod.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://buz.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nig.yj202588.top

TS:   [...a, ...b];
来源：http://dfa.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qrc.quarkkingdee.top

Go:   append(a, b...)
来源：http://ljn.cheryme.top

Ruby: a + b;  a.concat(b)
来源：http://huq.pycfn.com

C#:   a.Concat(b).ToList()
来源：http://fvc.snrcjt.cn

[D09] 排序（升序）
来源：http://zek.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://bdk.zhiwuduotai.top

PHP:  sort($arr);
来源：http://ihq.zhijiandao.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nqq.bjfxy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xdd.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vmf.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pox.yj202588.top

Ruby: arr.sort
来源：http://rfi.pycfn.com

C#:   list.Sort();
来源：http://rog.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xob.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zmw.gzhubu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xwr.zhengqikj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ghk.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aoo.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gsb.zhiwuduotai.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xdz.yj202588.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kkz.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wfc.pycfn.com

[D11] 反转数组
来源：http://ken.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://cuq.zhengqikj.top

PHP:  array_reverse($arr);
来源：http://ejo.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://acq.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://igs.jinyuanbaomall.cn

Java: Collections.reverse(list);
来源：http://mfu.shzxlz.cn

Go:   slices.Reverse(arr)
来源：http://qvp.yongpay.top

Ruby: arr.reverse
来源：http://uxu.bjfxy.top

C#:   list.Reverse();
来源：http://ucy.uphjek.com

[D12] 查找元素下标
来源：http://ifk.jinqigufen.top

Py:   arr.index(x);  x in arr
来源：http://wev.dianchejie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iko.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xoj.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bau.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://led.pycfn.com

Go:   slices.Index(arr, x)
来源：http://kya.redwolf501.top

Ruby: arr.index(x)
来源：http://hnr.tian-w.cn

C#:   list.IndexOf(x);
来源：http://pgz.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://qyk.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rmw.ywan-chungtsiang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gxq.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://lqh.ivvv.top

TS:   arr.filter(x => x > 3)
来源：http://wjq.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gyr.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://smh.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://rew.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hbg.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://ugn.tanke756.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qco.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aey.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://lac.zhoulong.xyz

TS:   arr.map(x => x * 2)
来源：http://qfl.yongpay.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://waf.yangfankeji.com

Go:   // 手写循环
来源：http://lrj.hnqzz.top

Ruby: arr.map { |x| x * 2 }
来源：http://ncb.pycfn.com

C#:   list.Select(x => x * 2).ToList()
来源：http://bun.gzhubu.top

[D15] 去重
来源：http://ekn.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ktc.shanyushiyangkeji.top

PHP:  array_unique($arr);
来源：http://aho.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://rov.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://rgr.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zzt.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gho.fehbvm.com

Ruby: arr.uniq
来源：http://kga.yanxiufei.cn

C#:   list.Distinct().ToList()
来源：http://dlq.bjfxy.top

[D16] 求和与平均值
来源：http://cjb.yueranfly.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rfx.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jsl.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lrz.316326.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://plq.ivvv.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bjq.yj20258.top

Go:   // 手写循环累加
来源：http://hzj.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bzf.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://joc.yuanzhike.top

[D17] 最大值与最小值
来源：http://ajo.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://mar.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://pez.wangshuangyany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://obf.yj20258.top

TS:   Math.max(...arr);
来源：http://acs.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://sey.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ycb.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://xdr.wangshuangyany.cn

C#:   list.Max();  list.Min()
来源：http://xkm.cqqwz.cn

[D18] 扁平化嵌套数组
来源：http://dit.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ijy.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://ppt.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wau.kuanghao11.cn

TS:   nested.flat();
来源：http://bzw.shuidangran.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jno.xuanzx.com

Go:   // 手写双层循环
来源：http://eaj.nanxinkj.top

Ruby: nested.flatten
来源：http://pja.shuidangran.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hdi.jyoumei.cn

[D19] 按字段分组
来源：http://jkp.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yns.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pva.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hsu.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ama.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kss.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://yvp.chenlongwang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xyc.jiagoushi.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://krk.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://uiv.mhx1999.top

Py:   Counter(arr)
来源：http://awp.316326.xyz

PHP:  array_count_values($arr);
来源：http://hde.guowangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qug.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hrw.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://szf.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://qer.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://fef.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sug.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://mxw.birdmap.top

Py:   x in arr
来源：http://rox.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://mdo.pycfn.com

JS:   arr.includes(x)
来源：http://wrl.yonumen.top

TS:   arr.includes(x)
来源：http://xez.zdbjq.cn

Java: list.contains(x)
来源：http://lzt.fanxiaobao.xyz

Go:   slices.Contains(arr, x)
来源：http://wse.cucudq.cn

Ruby: arr.include?(x)
来源：http://ssm.316326.xyz

C#:   list.Contains(x)
来源：http://fva.yueranfly.top

[D22] 复制数组（避免共享引用）
来源：http://tyu.gogol.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pju.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://coi.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jhe.0kj1m.cn

TS:   [...arr];
来源：http://lbb.yueranfly.top

Java: new ArrayList<>(list);
来源：http://rcg.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hhu.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://iny.yj20258888.top

C#:   new List<int>(list);
来源：http://dbk.chenzaomai.com

[D23] reduce 累积计算
来源：http://wyl.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ibn.jinqigufen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yvw.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hll.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ftn.zhijiandao.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://brt.jianghu66.top

Go:   // 手写循环
来源：http://zbf.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://own.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rvj.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://tue.ywan-chungtsiang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fnc.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bia.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ksl.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eir.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uys.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baw.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fle.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jen.xylfe.cn

[D25] Set 集合去重与交并差
来源：http://yfe.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://guz.gaohongyu789.top


<!-- 参考信息 -->