代发 wailian999

[C10] 变量作用域
来源：http://hqo.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cvv.hnqzz.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jfi.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ggh.jlsjyb.cn

TS:   同 JS
来源：http://imm.jyoumei.cn

Java: 方法内为块级作用域
来源：http://sol.jinghuilouyu.cn

Go:   花括号块级作用域
来源：http://wlb.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ijh.yvedp.cn

C#:   块级作用域
来源：http://atl.yuxming.cn

[C11] 模块导入与导出
来源：http://ryr.shzxlz.cn

Py:   from module import func
来源：http://wnz.fzhhl.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qeb.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://obq.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rqy.meibo888.top

Java: import java.util.List;
来源：http://snf.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qds.daria6918.cn

Ruby: require "json"; require_relative "./util"
来源：http://baj.epnwcf.com

C#:   using System.Text;
来源：http://jqe.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://avy.bjfxy.top

Py:   (lambda: print("run"))()
来源：http://tfh.yj20258.top

PHP:  (function () { echo "run"; })();
来源：http://uzl.ydzc1.top

JS:   (() => { console.log("run"); })();
来源：http://epc.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://oxj.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://esg.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://zto.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://tim.tanke756.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lgx.cqqwz.cn

[C13] 类型声明 / 类型注解
来源：http://vgw.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rzi.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://khr.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nlp.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gct.pengpengdd.cyou

Java: int add(int a, int b) { return a + b; }
来源：http://pcf.havefunace.top

Go:   func add(a, b int) int
来源：http://ytt.daria6918.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kbx.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://daf.gaohongyu789.top

[C14] 泛型函数
来源：http://gqb.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vhi.jqgfzy.top

PHP:  // 无泛型
来源：http://rff.jianghu66.top

JS:   // 无泛型
来源：http://xnc.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eaq.ydjk.org.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gvz.nanxinkj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tfj.yonumen.top

Ruby: # 无泛型
来源：http://lue.zhaomingkeji.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lel.uphjek.com

[C15] 解构 / 展开参数
来源：http://ulw.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lfd.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://slu.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fwt.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sif.gaohongyu789.top

Java: // 无解构
来源：http://rlk.jlsjyb.cn

Go:   // 无解构
来源：http://vkj.9152youxi.cn

Ruby: a, b = pair
来源：http://seo.vehdjk.com

C#:   var (a, b) = pair;
来源：http://yso.nwbrower.top

[C16] 函数 / 方法重载
来源：http://pym.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kyx.jlsjyb.cn

PHP:  // 无重载
来源：http://uve.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://txl.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://vky.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bsd.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://tzj.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://hps.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uod.yongpay.top

================================================================================
来源：http://djy.gotoacloud.top

D. 数组 / 列表 / 集合
来源：http://lxu.hnqzz.top

================================================================================
来源：http://hkg.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://rju.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://boc.tianlin.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sja.ydzc1.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uch.hongshengwenyu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kwb.fzhhl.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://htr.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://vwj.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://hnh.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iak.c1oappe.top

[D02] 追加元素到末尾
来源：http://bee.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://msc.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ddy.sweek.top

JS:   arr.push(4);
来源：http://dtp.yj202588.top

TS:   arr.push(4);
来源：http://ctf.birdmap.top

Java: list.add(4);
来源：http://swv.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://nux.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://sxh.shangyingyoupin.top

C#:   list.Add(4);
来源：http://mup.cucudq.cn

[D03] 在指定位置插入元素
来源：http://eun.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://orq.ivvv.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xet.yj20258.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jkh.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://gkj.cashguo.top

Java: list.add(0, 0);
来源：http://fqw.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://llx.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wsf.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://soa.jinqigfzy.top

[D04] 删除元素
来源：http://ocs.xylfe.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tyy.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pgg.hnqzz.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aqo.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://awk.sufxvd.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://idh.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yfr.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ehq.fzhhl.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fwo.ctjpmb.com

[D05] 访问与修改元素
来源：http://ini.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iyp.jqgufenzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cjg.jinghuilouyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nfe.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://nrg.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://wvh.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://xvs.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rop.hysaishi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://plf.guowangkeji.top

[D06] 数组长度
来源：http://bjr.hammf.cn

Py:   len(arr)
来源：http://rxl.wangdashe.top

PHP:  count($arr);
来源：http://hxo.hammf.cn

JS:   arr.length
来源：http://ihk.dashuyun.cn

TS:   arr.length
来源：http://hqg.sysykeji.top

Java: list.size();
来源：http://ohd.yanxiufei.cn

Go:   len(arr)
来源：http://yav.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://iej.iojbl.cn

C#:   list.Count;
来源：http://jpn.yuxming.cn

[D07] 切片 / 取子数组
来源：http://xky.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vuk.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mbl.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://han.ydzc1.top

TS:   arr.slice(1, 4);
来源：http://zqx.pycfn.com

Java: list.subList(1, 4);
来源：http://bnm.yangfankeji.com

Go:   arr[1:4]
来源：http://jyk.iojbl.cn

Ruby: arr[1, 3]
来源：http://zgv.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://lkn.jinqigufen.top

[D08] 合并两个数组
来源：http://nqh.xuetiantiany.cn

Py:   a + b;  a.extend(b)
来源：http://otd.gaohongyu789.top

PHP:  array_merge($a, $b);
来源：http://nlq.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qdu.xziqi.cn

TS:   [...a, ...b];
来源：http://wiy.daria6918.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eok.snrcjt.cn

Go:   append(a, b...)
来源：http://uks.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://dgy.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://oev.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://ima.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://drb.ydzc1.top

PHP:  sort($arr);
来源：http://iqq.yj20258888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mrb.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vzh.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hcz.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gnp.uphjek.com

Ruby: arr.sort
来源：http://slx.aibaodan.cn

C#:   list.Sort();
来源：http://vzr.wangshuangyany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://orw.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://unr.yongpay.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ksn.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ysy.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fkx.jyoumei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fsb.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dkk.zdbjq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pzo.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fpa.fengsongda.top

[D11] 反转数组
来源：http://sas.gotoacloud.top

Py:   arr[::-1];  arr.reverse()
来源：http://vnt.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://lvy.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://btg.yuxming.cn

TS:   [...arr].reverse();
来源：http://npo.jinyuanbaomall.cn

Java: Collections.reverse(list);
来源：http://bkg.gotoacloud.top

Go:   slices.Reverse(arr)
来源：http://oer.gzhubu.top

Ruby: arr.reverse
来源：http://tky.svipenyu.cn

C#:   list.Reverse();
来源：http://thq.xinyue.icu

[D12] 查找元素下标
来源：http://gfq.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://rln.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qbf.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pxa.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ufu.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dhj.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://zaq.sweek.top

Ruby: arr.index(x)
来源：http://bmh.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://ymr.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://lgy.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nxs.jinghuilouyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zfu.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://bup.cashguo.top

TS:   arr.filter(x => x > 3)
来源：http://zyy.kuanghao11.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zfm.zhixingplan.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xzk.nanxuanxn.top

Ruby: arr.select { |x| x > 3 }
来源：http://aci.xylfe.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jrr.cucudq.cn

[D14] 映射转换（每个元素变形）
来源：http://gxb.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ajf.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wyj.sxryk.cn

JS:   arr.map(x => x * 2)
来源：http://lny.sweek.top

TS:   arr.map(x => x * 2)
来源：http://hod.gaohongyu789.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qmd.yfazqb.com

Go:   // 手写循环
来源：http://pzt.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://gcy.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://oqe.yanxiufei.cn

[D15] 去重
来源：http://wzx.jinyuanbaomall.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jqx.jlsjyb.cn

PHP:  array_unique($arr);
来源：http://gss.hesvh.cn

JS:   [...new Set(arr)]
来源：http://pip.daria6918.cn

TS:   [...new Set(arr)]
来源：http://knd.gaohongyu789.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://csp.yongpay.top

Go:   // 用 map[T]struct{} 手写
来源：http://nxq.bbcook.cn

Ruby: arr.uniq
来源：http://ymt.pengpengdd.cyou

C#:   list.Distinct().ToList()
来源：http://rdi.chenjidiqi.icu

[D16] 求和与平均值
来源：http://owj.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://joc.9152youxi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mva.andypj.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kjc.cqqwz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pcl.nwbrower.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ryj.316326.xyz

Go:   // 手写循环累加
来源：http://kcj.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aua.shuidangran.top

C#:   list.Sum();  list.Average()
来源：http://rui.jiagoushi.top

[D17] 最大值与最小值
来源：http://jpa.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://nzo.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://qef.shanyushiyangtech.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ojs.haohaochexian.top

TS:   Math.max(...arr);
来源：http://fex.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://fzz.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rma.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://jtl.hysaishi.cn

C#:   list.Max();  list.Min()
来源：http://ply.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://wlu.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://klk.pengpengdd.cyou

PHP:  array_merge(...$nested);
来源：http://mdy.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cop.chenjidiqi.icu

TS:   nested.flat();
来源：http://yns.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oxe.chenzaomai.com

Go:   // 手写双层循环
来源：http://pxi.yanxiufei.cn

Ruby: nested.flatten
来源：http://ugz.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://acu.shanyushiyangtech.top

[D19] 按字段分组
来源：http://ont.nanxuanxn.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qcj.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bsy.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://onx.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vtt.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lpf.zhongyouzk.top

Go:   // 手写 map[string][]T
来源：http://pur.xingfuxueyuan.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://irv.shangyingyoupin.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hli.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://gxc.feifeiyinyue.top

Py:   Counter(arr)
来源：http://faj.c1oappe.top

PHP:  array_count_values($arr);
来源：http://ypy.chenzaomai.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cjc.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oop.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eoa.fehbvm.com

Go:   // 手写 map[T]int
来源：http://xoh.cheryme.top

Ruby: arr.tally
来源：http://maa.kuanghao11.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uxy.cucudq.cn

[D21] 判断是否包含某元素
来源：http://elf.zhengqikj.top

Py:   x in arr
来源：http://jdl.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://qef.yvedp.cn

JS:   arr.includes(x)
来源：http://kmy.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://ecj.jinghuilouyu.cn

Java: list.contains(x)
来源：http://gfp.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://xws.c1oappe.top

Ruby: arr.include?(x)
来源：http://oyi.fzhhl.top

C#:   list.Contains(x)
来源：http://xxo.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://zyb.fehbvm.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jpw.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://skh.cqqwz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tcj.dianchejie.cn

TS:   [...arr];
来源：http://bft.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://qdo.hysaishi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gjn.cashguo.top

Ruby: arr.dup;  arr.clone
来源：http://qid.epnwcf.com

C#:   new List<int>(list);
来源：http://qwv.daria6918.cn

[D23] reduce 累积计算
来源：http://xsj.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xlz.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xfh.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qzl.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nbf.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ssk.sxryk.cn

Go:   // 手写循环
来源：http://nct.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rpw.kuanghao11.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fli.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://alk.birdmap.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tac.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jlo.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ddk.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yne.xingfuxueyuan.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://juj.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uie.xinyue.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cxi.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ike.yonumen.top

[D25] Set 集合去重与交并差
来源：http://nud.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ode.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eyr.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mwm.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uxv.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rbw.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rnd.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bfw.jinghuilouyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hxh.tarul.cn

[D26] 数组转字符串
来源：http://flq.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://vxi.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://kfi.yfazqb.com

JS:   arr.join(", ")
来源：http://cdn.xingfuxueyuan.xyz

TS:   arr.join(", ")
来源：http://pqy.kuanghao11.cn

Java: String.join(", ", list)
来源：http://osa.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://ngh.ppjwa.cn

Ruby: arr.join(", ")
来源：http://jzc.hysaishi.cn

C#:   string.Join(", ", list)
来源：http://gcc.jinghuilouyu.cn


<!-- 参考信息 -->