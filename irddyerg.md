代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oue.xuetiantiany.cn

TS:   arr.map(String)
来源：http://njx.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vef.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xfv.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://uhr.jinghuilouyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jqi.xinyue.icu

[C08] 闭包
来源：http://pds.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xuh.pengpengdd.cyou

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ghl.wangshuangyany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eit.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eow.c1oappe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qdn.daria6918.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hcr.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eov.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://avd.ydzc1.top

[C09] 递归
来源：http://ytb.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hgu.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vly.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hkw.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dpc.haohaochexian.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cpl.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gzg.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ajn.kuanghao11.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bnh.andypj.xyz

[C10] 变量作用域
来源：http://omu.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yjz.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qyh.tanke756.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rpf.gogol.net.cn

TS:   同 JS
来源：http://ibm.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://buw.jiagoushi.top

Go:   花括号块级作用域
来源：http://lct.bbcook.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mwi.shuidangran.top

C#:   块级作用域
来源：http://fkq.cqqwz.cn

[C11] 模块导入与导出
来源：http://fno.sysykeji.top

Py:   from module import func
来源：http://tem.yj20258888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gvc.cqqwz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ofh.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jpt.nanxinkj.top

Java: import java.util.List;
来源：http://lpe.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xri.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://lts.quarkkingdee.top

C#:   using System.Text;
来源：http://qow.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://jtr.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://zob.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://lwe.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://gha.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://izg.jinyuanbaomall.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ifa.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://xau.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://efa.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gus.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://lvb.ybcxt.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kqr.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mud.cqqwz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zfm.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wmq.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://obl.dashuyun.cn

Go:   func add(a, b int) int
来源：http://lhd.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xdu.zdqjudy.top

C#:   int Add(int a, int b) => a + b;
来源：http://kdy.sweek.top

[C14] 泛型函数
来源：http://khz.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wkf.daxiang520.top

PHP:  // 无泛型
来源：http://hwi.xingfuxueyuan.xyz

JS:   // 无泛型
来源：http://huc.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hdi.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jrq.fengsongda.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ugy.316326.xyz

Ruby: # 无泛型
来源：http://emb.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tdd.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://rmc.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jcz.pengpengdd.cyou

PHP:  [$a, $b] = $pair;
来源：http://alz.guannengcc.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qxk.hfpthk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hmf.redwolf501.top

Java: // 无解构
来源：http://dut.hywenlv.cn

Go:   // 无解构
来源：http://pmn.chenlongwang.top

Ruby: a, b = pair
来源：http://ssx.yuanzhike.top

C#:   var (a, b) = pair;
来源：http://inb.yvedp.cn

[C16] 函数 / 方法重载
来源：http://vug.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pix.316326.xyz

PHP:  // 无重载
来源：http://ewh.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dbj.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://llp.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://iak.jinqigufen.top

Go:   // 无重载：用不同函数名
来源：http://upc.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://wjt.c1oappe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fdn.dashuyun.cn

================================================================================
来源：http://peg.xinyue.icu

D. 数组 / 列表 / 集合
来源：http://zyp.nanxinkj.top

================================================================================
来源：http://bgj.yvedp.cn

[D01] 创建数组 / 列表
来源：http://msb.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tbw.chenzaomai.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ovy.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ayt.gogol.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://geb.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nar.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://unt.ehwqpu.com

Ruby: arr = [1, 2, 3]
来源：http://gdp.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wws.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://oao.zdbjq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yts.yonumen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://trs.hammf.cn

JS:   arr.push(4);
来源：http://uhx.jianghu66.top

TS:   arr.push(4);
来源：http://kgf.feifeiyinyue.top

Java: list.add(4);
来源：http://oau.52xcode.cn

Go:   arr = append(arr, 4)
来源：http://quo.kuanghao11.cn

Ruby: arr << 4; arr.push(5)
来源：http://gez.jqgufenzy.top

C#:   list.Add(4);
来源：http://qsn.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://xzj.snrcjt.cn

Py:   arr.insert(0, 0)
来源：http://sbp.cheryme.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zas.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dex.c1oappe.top

TS:   arr.splice(0, 0, 0);
来源：http://beq.bbcook.cn

Java: list.add(0, 0);
来源：http://coo.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://ecr.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lsf.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://oar.andypj.xyz

[D04] 删除元素
来源：http://udy.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mlv.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://law.sysykeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://snc.guowangkeji.top

TS:   arr.splice(0, 1);
来源：http://cri.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://npm.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cwq.pycfn.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jmt.haohaochexian.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gxj.hywenlv.cn

[D05] 访问与修改元素
来源：http://hxs.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cwb.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qhx.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sbd.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://emv.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://zbg.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://jpu.snrcjt.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dno.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://toi.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://aea.aibaodan.cn

Py:   len(arr)
来源：http://pse.andypj.xyz

PHP:  count($arr);
来源：http://ylh.jinghuilouyu.cn

JS:   arr.length
来源：http://poq.yuanzhike.top

TS:   arr.length
来源：http://ibe.52xcode.cn

Java: list.size();
来源：http://ozj.hywenlv.cn

Go:   len(arr)
来源：http://zxg.fzhhl.top

Ruby: arr.length; arr.size
来源：http://ajz.dianchejie.cn

C#:   list.Count;
来源：http://ubl.yongpay.top

[D07] 切片 / 取子数组
来源：http://psc.fktsv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wpy.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ocp.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://yzy.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://ujx.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://enb.zdbjq.cn

Go:   arr[1:4]
来源：http://agm.smart0.xyz

Ruby: arr[1, 3]
来源：http://huj.9152youxi.cn

C#:   list.GetRange(1, 3);
来源：http://ahu.fengsongda.top

[D08] 合并两个数组
来源：http://fid.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://ngj.pycfn.com

PHP:  array_merge($a, $b);
来源：http://yzt.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nss.jyoumei.cn

TS:   [...a, ...b];
来源：http://bxo.ybcxt.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qof.hcnkem.com

Go:   append(a, b...)
来源：http://hib.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://efk.hfpthk.cn

C#:   a.Concat(b).ToList()
来源：http://gpx.ydjk.org.cn

[D09] 排序（升序）
来源：http://hvb.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://bbp.jianghu66.top

PHP:  sort($arr);
来源：http://nzp.chenzaomai.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rsz.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://igg.vehdjk.com

Java: Collections.sort(list);  list.sort(null);
来源：http://ojy.aizwys.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jhf.cdnleiting.top

Ruby: arr.sort
来源：http://ejq.bbcook.cn

C#:   list.Sort();
来源：http://pqn.sysykeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://emj.shzxlz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nmq.c1oappe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gsx.zhiwuduotai.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hsc.ppjwa.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aqm.snrcjt.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xrd.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pld.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vec.havefunace.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pcj.fktsv.cn

[D11] 反转数组
来源：http://ieg.iojbl.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yfg.chenjidiqi.icu

PHP:  array_reverse($arr);
来源：http://dwc.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mxt.gzhubu.top

TS:   [...arr].reverse();
来源：http://idu.yuxming.cn

Java: Collections.reverse(list);
来源：http://whs.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://dtx.yonumen.top

Ruby: arr.reverse
来源：http://tzp.shzxlz.cn

C#:   list.Reverse();
来源：http://iya.zhijiandao.cn

[D12] 查找元素下标
来源：http://lth.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://vkg.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uqn.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://quy.jinqigfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ogb.hammf.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://njq.nanxuanxn.top

Go:   slices.Index(arr, x)
来源：http://hej.zhiwuduotai.top

Ruby: arr.index(x)
来源：http://jqq.daria6918.cn

C#:   list.IndexOf(x);
来源：http://ejp.ybcxt.top

[D13] 过滤（保留满足条件的）
来源：http://ldd.hywenlv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xek.chenzaomai.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xul.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://wpq.vqdsnc.cn

TS:   arr.filter(x => x > 3)
来源：http://myc.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cki.zycfv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lzj.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jma.shanyushiyangtech.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ovp.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://ydr.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dfs.jinghuilouyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ohc.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://nyl.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://vur.9152youxi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hvz.yj20258888.top

Go:   // 手写循环
来源：http://mis.svipenyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xel.vehdjk.com

C#:   list.Select(x => x * 2).ToList()
来源：http://tcn.jianghu66.top

[D15] 去重
来源：http://niw.cashguo.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lcu.zycfv.cn

PHP:  array_unique($arr);
来源：http://ylz.sysykeji.top

JS:   [...new Set(arr)]
来源：http://bhx.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://zlg.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tzz.xinyue.icu

Go:   // 用 map[T]struct{} 手写
来源：http://pir.feifeiyinyue.top

Ruby: arr.uniq
来源：http://zyy.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://kam.mhx1999.top

[D16] 求和与平均值
来源：http://jxl.hnxiangtu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pnp.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jxb.epnwcf.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tqm.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mme.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hcu.cheryme.top

Go:   // 手写循环累加
来源：http://msf.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ved.tanke756.top

C#:   list.Sum();  list.Average()
来源：http://tux.vehdjk.com

[D17] 最大值与最小值
来源：http://fub.haohaochexian.top

Py:   max(arr);  min(arr)
来源：http://seh.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://hcz.cheryme.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cwr.yj20258.top

TS:   Math.max(...arr);
来源：http://irh.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dls.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rkb.mhx1999.top

Ruby: arr.max;  arr.min
来源：http://tgj.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://ewv.fanxiaobao.xyz

[D18] 扁平化嵌套数组
来源：http://kfn.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jip.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://ait.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pcw.fzhhl.top

TS:   nested.flat();
来源：http://yjp.cashguo.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tou.uphjek.com

Go:   // 手写双层循环
来源：http://ykv.52xcode.cn

Ruby: nested.flatten
来源：http://kjo.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://dzi.jinqigfzy.top

[D19] 按字段分组
来源：http://xrw.pengpengdd.cyou

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xxe.yuxming.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jmd.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vjo.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://hwo.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kby.redwolf501.top

Go:   // 手写 map[string][]T
来源：http://wsl.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qfu.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://izz.zdbjq.cn

[D20] 统计每个元素出现次数
来源：http://amg.nwbrower.top

Py:   Counter(arr)
来源：http://pmy.guannengcc.top

PHP:  array_count_values($arr);
来源：http://ogw.fanxiaobao.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jxg.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qpl.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ahy.gotoacloud.top

Go:   // 手写 map[T]int
来源：http://tzf.gaohongyu789.top

Ruby: arr.tally
来源：http://nbu.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tem.meibo888.top

[D21] 判断是否包含某元素
来源：http://rrx.epnwcf.com

Py:   x in arr
来源：http://wov.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://hdq.jinghuilouyu.cn

JS:   arr.includes(x)
来源：http://xqi.c1oappe.top

TS:   arr.includes(x)
来源：http://zty.iojbl.cn

Java: list.contains(x)
来源：http://vrq.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://ptt.c1oappe.top

Ruby: arr.include?(x)
来源：http://lce.tian-w.cn

C#:   list.Contains(x)
来源：http://paa.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://iad.yongpay.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rsu.hammf.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mvv.jqgfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vkj.zhoulong.xyz

TS:   [...arr];
来源：http://jft.yj20258.top

Java: new ArrayList<>(list);
来源：http://rli.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://cua.wangshuangyany.cn

Ruby: arr.dup;  arr.clone
来源：http://gpk.jqgufenzy.top

C#:   new List<int>(list);
来源：http://udy.0kj1m.cn

[D23] reduce 累积计算
来源：http://mus.zhijiandao.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nkh.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gmy.yj202588.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dml.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oos.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rod.mhx1999.top

Go:   // 手写循环
来源：http://nbe.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://svu.meibo888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nfn.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://nwr.fanxiaobao.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jfl.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cqy.jinghuilouyu.cn


<!-- 参考信息 -->