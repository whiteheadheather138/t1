代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://byu.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gsj.ehwqpu.com

Java: import java.util.List;
来源：http://amn.chenzaomai.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oxa.jlsjyb.cn

Ruby: require "json"; require_relative "./util"
来源：http://poq.aibaodan.cn

C#:   using System.Text;
来源：http://hav.xingfuxueyuan.xyz

[C12] 立即执行函数 IIFE
来源：http://peh.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://hwy.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://iib.jyoumei.cn

JS:   (() => { console.log("run"); })();
来源：http://qxw.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://flu.yangfankeji.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xun.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://bbw.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://ncc.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mwt.jianghu66.top

[C13] 类型声明 / 类型注解
来源：http://ghi.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cuf.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aje.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fuz.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bnd.yuxming.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pjb.52xcode.cn

Go:   func add(a, b int) int
来源：http://uqf.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lwc.yj202588.top

C#:   int Add(int a, int b) => a + b;
来源：http://nrc.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://yer.dianchejie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ngi.zhengqikj.top

PHP:  // 无泛型
来源：http://fmo.chenlongwang.top

JS:   // 无泛型
来源：http://cfg.redwolf501.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zuh.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mlv.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ymb.uphjek.com

Ruby: # 无泛型
来源：http://hwx.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tkb.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://pxm.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cbw.snrcjt.cn

PHP:  [$a, $b] = $pair;
来源：http://htk.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rmc.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://odf.bbcook.cn

Java: // 无解构
来源：http://gtf.kuanghao11.cn

Go:   // 无解构
来源：http://slx.0kj1m.cn

Ruby: a, b = pair
来源：http://kgf.cashguo.top

C#:   var (a, b) = pair;
来源：http://ira.cheryme.top

[C16] 函数 / 方法重载
来源：http://tzi.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gej.shanyushiyangkeji.top

PHP:  // 无重载
来源：http://tre.sysykeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uiy.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://asq.fehbvm.com

Java: void f(int a) {}  void f(String a) {}
来源：http://trn.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://fdq.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://ive.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tne.gzhubu.top

================================================================================
来源：http://drp.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://hnv.jyoumei.cn

================================================================================
来源：http://nlo.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://vsb.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://grq.ivvv.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qfl.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xpi.nanxuanxn.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wip.316326.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://opf.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://ebi.yj20258888.top

Ruby: arr = [1, 2, 3]
来源：http://iex.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vuv.xuanzx.com

[D02] 追加元素到末尾
来源：http://ysj.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dlv.yj202588.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qwg.uphjek.com

JS:   arr.push(4);
来源：http://hzg.ydjk.org.cn

TS:   arr.push(4);
来源：http://lub.jlsjyb.cn

Java: list.add(4);
来源：http://ugf.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://qyu.hesvh.cn

Ruby: arr << 4; arr.push(5)
来源：http://avr.cheryme.top

C#:   list.Add(4);
来源：http://jer.ydjk.org.cn

[D03] 在指定位置插入元素
来源：http://zzy.yongpay.top

Py:   arr.insert(0, 0)
来源：http://dsc.hysaishi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lca.epnwcf.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gpg.jianghu66.top

TS:   arr.splice(0, 0, 0);
来源：http://rxn.ivvv.top

Java: list.add(0, 0);
来源：http://ujq.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jyu.yj202588.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://feh.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://svk.andypj.xyz

[D04] 删除元素
来源：http://use.jianghu66.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jah.redwolf501.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://chd.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vvf.jiagoushi.top

TS:   arr.splice(0, 1);
来源：http://zio.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fxp.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fwl.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jiy.shanyushiyangtech.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mkk.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://lpl.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://san.ydzc1.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://shb.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://plf.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://evg.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://dis.zhongyouzk.top

Go:   arr[0]; arr[0] = 9
来源：http://cwr.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yjs.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pst.daria6918.cn

[D06] 数组长度
来源：http://jwg.yfazqb.com

Py:   len(arr)
来源：http://boy.yuanzhike.top

PHP:  count($arr);
来源：http://vox.nanxuanxn.top

JS:   arr.length
来源：http://rcl.meibo888.top

TS:   arr.length
来源：http://whd.hywenlv.cn

Java: list.size();
来源：http://wko.jianghu66.top

Go:   len(arr)
来源：http://mqt.ydzc1.top

Ruby: arr.length; arr.size
来源：http://wbq.pycfn.com

C#:   list.Count;
来源：http://tzi.hfpthk.cn

[D07] 切片 / 取子数组
来源：http://yza.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jbq.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://mvy.ydzc1.top

JS:   arr.slice(1, 4);
来源：http://ocr.ehwqpu.com

TS:   arr.slice(1, 4);
来源：http://bne.pycfn.com

Java: list.subList(1, 4);
来源：http://fps.zhixingplan.top

Go:   arr[1:4]
来源：http://vnm.iojbl.cn

Ruby: arr[1, 3]
来源：http://lze.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://tgd.zhixingplan.top

[D08] 合并两个数组
来源：http://dgg.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://nrj.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://zjn.cheryme.top

JS:   [...a, ...b];  a.concat(b);
来源：http://miu.52xcode.cn

TS:   [...a, ...b];
来源：http://qxq.guannengcc.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zkk.yuanzhike.top

Go:   append(a, b...)
来源：http://owd.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://uze.fanxiaobao.xyz

C#:   a.Concat(b).ToList()
来源：http://sjc.aibaodan.cn

[D09] 排序（升序）
来源：http://sfy.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://tjc.hcnkem.com

PHP:  sort($arr);
来源：http://fur.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dif.gotoacloud.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ccs.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://dmi.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pjt.svipenyu.cn

Ruby: arr.sort
来源：http://vpc.xuetiantiany.cn

C#:   list.Sort();
来源：http://xdd.9152youxi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dsg.hfpthk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ael.fktsv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wui.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pfz.fehbvm.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kiv.shangyingyoupin.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://shy.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bou.cashguo.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hry.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xsj.sysykeji.top

[D11] 反转数组
来源：http://kto.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://nqu.shanyushiyangkeji.top

PHP:  array_reverse($arr);
来源：http://mni.hywenlv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cfc.nwbrower.top

TS:   [...arr].reverse();
来源：http://ydm.yuxming.cn

Java: Collections.reverse(list);
来源：http://vil.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://lad.bbcook.cn

Ruby: arr.reverse
来源：http://hcs.hcnkem.com

C#:   list.Reverse();
来源：http://tvk.feifeiyinyue.top

[D12] 查找元素下标
来源：http://crk.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://lhl.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jdj.cucudq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dvc.sxryk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fgs.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://slh.shzxlz.cn

Go:   slices.Index(arr, x)
来源：http://lqw.bjfxy.top

Ruby: arr.index(x)
来源：http://oyz.fengsongda.top

C#:   list.IndexOf(x);
来源：http://hwe.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://ptz.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qpz.bjfxy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hdd.mhx1999.top

JS:   arr.filter(x => x > 3)
来源：http://oan.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://yxt.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oed.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kvv.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fld.yfazqb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://yzj.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://fii.sweek.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vpp.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://waw.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://nll.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://nsy.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://yhx.zhiwuduotai.top

Go:   // 手写循环
来源：http://zfc.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hva.hnqzz.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zat.sxryk.cn

[D15] 去重
来源：http://rsa.ywan-chungtsiang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://epo.yuanzhike.top

PHP:  array_unique($arr);
来源：http://mof.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://kqa.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://pem.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dht.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uii.hammf.cn

Ruby: arr.uniq
来源：http://nvh.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://tpi.zycfv.cn

[D16] 求和与平均值
来源：http://uia.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://enf.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rrm.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vvp.zycfv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tax.316326.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xfi.zhoulong.xyz

Go:   // 手写循环累加
来源：http://oxr.9152youxi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xiv.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://wso.yj20258.top

[D17] 最大值与最小值
来源：http://nzb.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://yrb.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://vfr.shanyushiyangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xic.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://doj.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://mxo.aibaodan.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qgt.cashguo.top

Ruby: arr.max;  arr.min
来源：http://pon.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://ojx.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://uzo.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zfe.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://ewm.nanxuanxn.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ycl.shuidangran.top

TS:   nested.flat();
来源：http://tvk.guannengcc.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kha.fehbvm.com

Go:   // 手写双层循环
来源：http://qxm.xylfe.cn

Ruby: nested.flatten
来源：http://fsd.jlsjyb.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vkw.0kj1m.cn

[D19] 按字段分组
来源：http://cxi.yanxiufei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ckq.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yyt.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://exx.c1oappe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ovd.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://awc.fanxiaobao.xyz

Go:   // 手写 map[string][]T
来源：http://dcj.wangshuangyany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pac.tianlin.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://guy.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://gmi.bjfxy.top

Py:   Counter(arr)
来源：http://bkz.tanke756.top

PHP:  array_count_values($arr);
来源：http://cqc.sysykeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ynz.yonumen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jmq.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gri.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://ytc.tian-w.cn

Ruby: arr.tally
来源：http://cnq.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hvu.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://ufq.cashguo.top

Py:   x in arr
来源：http://jnw.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://xis.nanxinkj.top

JS:   arr.includes(x)
来源：http://esr.52xcode.cn

TS:   arr.includes(x)
来源：http://fvx.sweek.top

Java: list.contains(x)
来源：http://kom.xuetiantiany.cn

Go:   slices.Contains(arr, x)
来源：http://yan.cdnleiting.top

Ruby: arr.include?(x)
来源：http://qub.9152youxi.cn

C#:   list.Contains(x)
来源：http://jqg.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://kbv.yj20258888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uxl.fengsongda.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nmt.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ecs.smart0.xyz

TS:   [...arr];
来源：http://oew.yj20258.top

Java: new ArrayList<>(list);
来源：http://zvp.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://mmj.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://vuq.tian-w.cn

C#:   new List<int>(list);
来源：http://dro.guowangkeji.top

[D23] reduce 累积计算
来源：http://pze.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ylw.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ask.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iyg.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tua.fehbvm.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://zpu.iojbl.cn

Go:   // 手写循环
来源：http://ufn.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rxq.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dqj.yvedp.cn

[D24] 字典 / Map 基本操作
来源：http://xnx.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://amo.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lzr.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://skv.daxiang520.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://axv.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vwm.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://twr.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://asf.redwolf501.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hca.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://fhw.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mtj.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dyj.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qye.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ftg.yj20258888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://osd.gzhubu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aqh.sxryk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zdf.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dqc.hnxiangtu.top

[D26] 数组转字符串
来源：http://hzf.tarul.cn

Py:   ", ".join(map(str, arr))
来源：http://ejq.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://zpq.jyoumei.cn

JS:   arr.join(", ")
来源：http://tdx.yj20258.top

TS:   arr.join(", ")
来源：http://pwn.uphjek.com

Java: String.join(", ", list)
来源：http://kob.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://qti.shuidangran.top

Ruby: arr.join(", ")
来源：http://jfn.jqgufenzy.top

C#:   string.Join(", ", list)
来源：http://vlk.tanke756.top

================================================================================
来源：http://gvu.chenlongwang.top

E. 字符串处理
来源：http://hcz.havefunace.top

================================================================================
来源：http://rtt.zhoulong.xyz

[E01] 拼接字符串
来源：http://zet.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uzu.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://piy.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nky.yj20258.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sav.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dhv.wangshuangyany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gms.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vmv.daxiang520.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ygt.9152youxi.cn


<!-- 参考信息 -->