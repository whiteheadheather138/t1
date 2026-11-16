代发 wailian999

[C10] 变量作用域
来源：http://pkk.iojbl.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://orh.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uag.smart0.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lyh.shanyushiyangtech.top

TS:   同 JS
来源：http://ivd.yvedp.cn

Java: 方法内为块级作用域
来源：http://cqt.svipenyu.cn

Go:   花括号块级作用域
来源：http://lxh.cheryme.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wnl.zhengqikj.top

C#:   块级作用域
来源：http://rwe.guowangkeji.top

[C11] 模块导入与导出
来源：http://wqz.zdbjq.cn

Py:   from module import func
来源：http://rlt.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ifi.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://enw.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qny.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://ona.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xct.gogol.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://hlq.gzhubu.top

C#:   using System.Text;
来源：http://qdo.xingfuxueyuan.xyz

[C12] 立即执行函数 IIFE
来源：http://gnj.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://uge.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://smj.cashguo.top

JS:   (() => { console.log("run"); })();
来源：http://rku.zhoulong.xyz

TS:   (() => { console.log("run"); })();
来源：http://hjq.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://khe.52xcode.cn

Go:   func() { fmt.Println("run") }()
来源：http://btc.cheryme.top

Ruby: -> { puts "run" }.call
来源：http://bec.ybcxt.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yhv.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://qvo.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oeq.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rqw.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zjh.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qlr.hongshengwenyu.top

Java: int add(int a, int b) { return a + b; }
来源：http://bkb.daria6918.cn

Go:   func add(a, b int) int
来源：http://nxf.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://czb.quarkkingdee.top

C#:   int Add(int a, int b) => a + b;
来源：http://sve.bjfxy.top

[C14] 泛型函数
来源：http://jre.fehbvm.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pho.chenlongwang.top

PHP:  // 无泛型
来源：http://igs.jinqigufen.top

JS:   // 无泛型
来源：http://ssz.gzhubu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ycn.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://abe.zhengqikj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jmj.sjlbkw.cn

Ruby: # 无泛型
来源：http://hnb.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fza.0kj1m.cn

[C15] 解构 / 展开参数
来源：http://cir.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://svf.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://jsk.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dzb.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xqb.zhengqikj.top

Java: // 无解构
来源：http://nuc.zdbjq.cn

Go:   // 无解构
来源：http://usb.yj20258.top

Ruby: a, b = pair
来源：http://pyy.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://tcc.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://cyg.svipenyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://itr.wangshuangyany.cn

PHP:  // 无重载
来源：http://xes.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://hzw.chenzaomai.com

TS:   // 用联合类型或重载签名声明
来源：http://anr.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tgn.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://fdv.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://ppc.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yem.nanxuanxn.top

================================================================================
来源：http://cdq.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://tgd.fktsv.cn

================================================================================
来源：http://kwj.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://sur.zhengqikj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://isq.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qiz.yuanzhike.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jkd.smart0.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://soy.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rmg.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://qbb.hongshengwenyu.top

Ruby: arr = [1, 2, 3]
来源：http://iht.sxryk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wdo.bbcook.cn

[D02] 追加元素到末尾
来源：http://alc.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hum.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hwm.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://itz.haohaochexian.top

TS:   arr.push(4);
来源：http://hwm.fehbvm.com

Java: list.add(4);
来源：http://gbs.vehdjk.com

Go:   arr = append(arr, 4)
来源：http://dvb.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://evr.aibaodan.cn

C#:   list.Add(4);
来源：http://hed.tanke756.top

[D03] 在指定位置插入元素
来源：http://dys.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://sdd.gotoacloud.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://znl.jiagoushi.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://axh.tian-w.cn

TS:   arr.splice(0, 0, 0);
来源：http://fil.ybcxt.top

Java: list.add(0, 0);
来源：http://psa.wangdashe.top

Go:   arr = append([]int{0}, arr...)
来源：http://wgq.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rvn.uphjek.com

C#:   list.Insert(0, 0);
来源：http://lcv.hnqzz.top

[D04] 删除元素
来源：http://dxw.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rig.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vdl.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jdu.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://jlk.zhongyouzk.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zgc.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sez.zhiwuduotai.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gvm.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yvf.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://omc.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iuf.fktsv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ddh.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://erl.shuidangran.top

TS:   arr[0]; arr.at(-1);
来源：http://qqz.ywan-chungtsiang.top

Java: list.get(0); list.set(0, 9);
来源：http://mzz.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://egi.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ymk.bbcook.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ydm.zhoulong.xyz

[D06] 数组长度
来源：http://zxn.daria6918.cn

Py:   len(arr)
来源：http://dwa.sufxvd.cn

PHP:  count($arr);
来源：http://vrt.jqgfzy.top

JS:   arr.length
来源：http://oqe.52xcode.cn

TS:   arr.length
来源：http://zpv.gzhubu.top

Java: list.size();
来源：http://uae.zhongyouzk.top

Go:   len(arr)
来源：http://ftr.yj20258.top

Ruby: arr.length; arr.size
来源：http://bfz.chenzaomai.com

C#:   list.Count;
来源：http://hxv.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://yum.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://foc.nwbrower.top

PHP:  array_slice($arr, 1, 3);
来源：http://yfk.birdmap.top

JS:   arr.slice(1, 4);
来源：http://ijv.shanyushiyangtech.top

TS:   arr.slice(1, 4);
来源：http://caj.yj20258.top

Java: list.subList(1, 4);
来源：http://gxx.quarkkingdee.top

Go:   arr[1:4]
来源：http://vjs.dashuyun.cn

Ruby: arr[1, 3]
来源：http://hff.epnwcf.com

C#:   list.GetRange(1, 3);
来源：http://qeu.yj20258.top

[D08] 合并两个数组
来源：http://wsh.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://erq.vehdjk.com

PHP:  array_merge($a, $b);
来源：http://ebg.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yff.tianlin.xyz

TS:   [...a, ...b];
来源：http://aop.hnxiangtu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qov.hcnkem.com

Go:   append(a, b...)
来源：http://lgf.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://jkf.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://vga.zhongyouzk.top

[D09] 排序（升序）
来源：http://msx.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://uts.52xcode.cn

PHP:  sort($arr);
来源：http://slr.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://trw.sxryk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iaf.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wvo.hfpthk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mjb.jqgfzy.top

Ruby: arr.sort
来源：http://sia.hammf.cn

C#:   list.Sort();
来源：http://frz.yvedp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://slj.haohaochexian.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sos.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bhv.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pem.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cqy.xinyue.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tga.xinyue.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aes.fehbvm.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tsg.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vlk.ydzc1.top

[D11] 反转数组
来源：http://jor.yfazqb.com

Py:   arr[::-1];  arr.reverse()
来源：http://hdq.hongshengwenyu.top

PHP:  array_reverse($arr);
来源：http://fvx.fengsongda.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sos.bbcook.cn

TS:   [...arr].reverse();
来源：http://fof.ydjk.org.cn

Java: Collections.reverse(list);
来源：http://pha.redwolf501.top

Go:   slices.Reverse(arr)
来源：http://iml.redwolf501.top

Ruby: arr.reverse
来源：http://ksw.xuetiantiany.cn

C#:   list.Reverse();
来源：http://smk.tanke756.top

[D12] 查找元素下标
来源：http://myv.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://kcz.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wiv.zhengqikj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bcp.uphjek.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://epd.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bme.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://klq.hcnkem.com

Ruby: arr.index(x)
来源：http://fyj.ivvv.top

C#:   list.IndexOf(x);
来源：http://sxs.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://bqy.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ppl.yvedp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ouq.sufxvd.cn

JS:   arr.filter(x => x > 3)
来源：http://atf.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://iwf.c1oappe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lhx.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kwr.bbcook.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pig.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cmk.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://zjf.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tjg.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://evq.mhx1999.top

JS:   arr.map(x => x * 2)
来源：http://vwt.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://hcr.52xcode.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://taw.zdbjq.cn

Go:   // 手写循环
来源：http://obo.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://ust.vehdjk.com

C#:   list.Select(x => x * 2).ToList()
来源：http://tmg.pycfn.com

[D15] 去重
来源：http://kkp.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://txv.iojbl.cn

PHP:  array_unique($arr);
来源：http://ooj.c1oappe.top

JS:   [...new Set(arr)]
来源：http://kwx.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://mgu.cdnleiting.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ffc.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://lma.jyoumei.cn

Ruby: arr.uniq
来源：http://yzi.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://unv.zhoulong.xyz

[D16] 求和与平均值
来源：http://auo.52xcode.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tmx.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://htx.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ugm.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zpw.svipenyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tbl.yuxming.cn

Go:   // 手写循环累加
来源：http://hlg.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tus.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://zgw.hywenlv.cn

[D17] 最大值与最小值
来源：http://jlu.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://hzv.316326.xyz

PHP:  max($arr);  min($arr);
来源：http://fsx.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mjk.yanxiufei.cn

TS:   Math.max(...arr);
来源：http://clc.yongpay.top

Java: Collections.max(list);  Collections.min(list);
来源：http://muh.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gxa.yj202588.top

Ruby: arr.max;  arr.min
来源：http://bjs.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://iyd.xylfe.cn

[D18] 扁平化嵌套数组
来源：http://cuh.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gfy.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://axt.tianlin.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xrj.yuxming.cn

TS:   nested.flat();
来源：http://obb.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hhk.zdbjq.cn

Go:   // 手写双层循环
来源：http://rgq.chenlongwang.top

Ruby: nested.flatten
来源：http://nag.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qem.cqqwz.cn

[D19] 按字段分组
来源：http://htt.sweek.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://liw.yanxiufei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kpz.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lyj.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://izo.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://swg.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://ycy.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cxf.guowangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jnp.yvedp.cn

[D20] 统计每个元素出现次数
来源：http://zst.snrcjt.cn

Py:   Counter(arr)
来源：http://gur.andypj.xyz

PHP:  array_count_values($arr);
来源：http://zcy.ywan-chungtsiang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iqj.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cob.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gxu.birdmap.top

Go:   // 手写 map[T]int
来源：http://seb.zhoulong.xyz

Ruby: arr.tally
来源：http://zxi.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cqs.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://vam.jlsjyb.cn

Py:   x in arr
来源：http://irs.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://oya.hnxiangtu.top

JS:   arr.includes(x)
来源：http://vrf.shuidangran.top

TS:   arr.includes(x)
来源：http://tmz.ctjpmb.com

Java: list.contains(x)
来源：http://gqr.zhongyouzk.top

Go:   slices.Contains(arr, x)
来源：http://opr.aizwys.cn

Ruby: arr.include?(x)
来源：http://ilw.zhoulong.xyz

C#:   list.Contains(x)
来源：http://ikl.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://ebe.haohaochexian.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://smt.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hdv.fehbvm.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ruy.hysaishi.cn

TS:   [...arr];
来源：http://ldm.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://pao.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://zoz.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://zjp.vehdjk.com

C#:   new List<int>(list);
来源：http://ljp.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://brm.hnxiangtu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cwe.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ond.shanyushiyangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ucj.jqgufenzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://alr.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vjw.gotoacloud.top

Go:   // 手写循环
来源：http://ifk.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ukw.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nlz.yanxiufei.cn

[D24] 字典 / Map 基本操作
来源：http://iwt.yj20258.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uyk.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qgk.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zpa.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wmf.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hvo.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ekc.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://byu.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lld.aizwys.cn

[D25] Set 集合去重与交并差
来源：http://jmm.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sww.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bhf.yanxiufei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gvt.yj20258888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gzv.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qkd.wangshuangyany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ort.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uqs.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xyl.quarkkingdee.top

[D26] 数组转字符串
来源：http://pht.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://nry.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://flz.shanyushiyangtech.top

JS:   arr.join(", ")
来源：http://llt.bbcook.cn

TS:   arr.join(", ")
来源：http://fht.cashguo.top

Java: String.join(", ", list)
来源：http://bvi.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://etj.hnqzz.top

Ruby: arr.join(", ")
来源：http://fon.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://mjo.dianchejie.cn


<!-- 参考信息 -->