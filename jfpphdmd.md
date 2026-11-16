代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://uoa.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://opq.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://qqm.0kj1m.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wzu.gzhubu.top

Ruby: require "json"; require_relative "./util"
来源：http://jkd.dashuyun.cn

C#:   using System.Text;
来源：http://dcv.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://sjh.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://fxn.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://jic.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://ohh.sxryk.cn

TS:   (() => { console.log("run"); })();
来源：http://yss.fanxiaobao.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zpv.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://qjw.havefunace.top

Ruby: -> { puts "run" }.call
来源：http://rbt.yonumen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wuq.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://ssm.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://snl.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dob.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://adg.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nbc.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://lpa.cdnleiting.top

Go:   func add(a, b int) int
来源：http://hsz.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vfc.cheryme.top

C#:   int Add(int a, int b) => a + b;
来源：http://ewr.vehdjk.com

[C14] 泛型函数
来源：http://mbf.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zvs.snrcjt.cn

PHP:  // 无泛型
来源：http://fxp.fengsongda.top

JS:   // 无泛型
来源：http://fcl.quarkkingdee.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mzq.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vkk.yuxming.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://taw.aizwys.cn

Ruby: # 无泛型
来源：http://cru.meibo888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xkr.fehbvm.com

[C15] 解构 / 展开参数
来源：http://ddt.sxryk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://plr.gzhubu.top

PHP:  [$a, $b] = $pair;
来源：http://ofl.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ygq.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mdt.ywan-chungtsiang.top

Java: // 无解构
来源：http://gak.kuanghao11.cn

Go:   // 无解构
来源：http://utw.yuanzhike.top

Ruby: a, b = pair
来源：http://cio.fengsongda.top

C#:   var (a, b) = pair;
来源：http://lmm.epnwcf.com

[C16] 函数 / 方法重载
来源：http://lsu.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yid.cashguo.top

PHP:  // 无重载
来源：http://zle.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://det.dianchejie.cn

TS:   // 用联合类型或重载签名声明
来源：http://yxc.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bfl.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://zlb.nanxuanxn.top

Ruby: # 无重载：靠动态参数
来源：http://xrn.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ghi.hfpthk.cn

================================================================================
来源：http://wat.nanxinkj.top

D. 数组 / 列表 / 集合
来源：http://hpk.cheryme.top

================================================================================
来源：http://sdr.yonumen.top

[D01] 创建数组 / 列表
来源：http://lqs.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qos.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hoc.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gaj.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://iru.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://icl.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://rxp.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://eyn.hcnkem.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rcn.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://jkf.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://crp.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vpt.jinqigufen.top

JS:   arr.push(4);
来源：http://koc.jiagoushi.top

TS:   arr.push(4);
来源：http://evr.dashuyun.cn

Java: list.add(4);
来源：http://ste.chenjidiqi.icu

Go:   arr = append(arr, 4)
来源：http://usa.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://odw.yongpay.top

C#:   list.Add(4);
来源：http://rtx.chenjidiqi.icu

[D03] 在指定位置插入元素
来源：http://kvt.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://hqk.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ciz.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zzq.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://dpk.iojbl.cn

Java: list.add(0, 0);
来源：http://tta.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bas.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hir.hcnkem.com

C#:   list.Insert(0, 0);
来源：http://yhm.smart0.xyz

[D04] 删除元素
来源：http://ugv.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jzw.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aiu.jianghu66.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xij.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://sfz.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lmr.zhongyouzk.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://elo.cucudq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jvc.yuanzhike.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mbf.ydjk.org.cn

[D05] 访问与修改元素
来源：http://qih.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ezl.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kij.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ujb.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://sjk.tian-w.cn

Java: list.get(0); list.set(0, 9);
来源：http://tcn.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://oag.c1oappe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qbd.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hwf.cashguo.top

[D06] 数组长度
来源：http://xrq.c1oappe.top

Py:   len(arr)
来源：http://aqf.ydjk.org.cn

PHP:  count($arr);
来源：http://obi.ydzc1.top

JS:   arr.length
来源：http://imr.c1oappe.top

TS:   arr.length
来源：http://jkj.nwbrower.top

Java: list.size();
来源：http://pam.yj20258888.top

Go:   len(arr)
来源：http://ghr.hfpthk.cn

Ruby: arr.length; arr.size
来源：http://vkc.xuetiantiany.cn

C#:   list.Count;
来源：http://cbg.fehbvm.com

[D07] 切片 / 取子数组
来源：http://eny.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xyn.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qfi.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://not.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://yyq.ehwqpu.com

Java: list.subList(1, 4);
来源：http://tfz.yuxming.cn

Go:   arr[1:4]
来源：http://tko.yueranfly.top

Ruby: arr[1, 3]
来源：http://ogb.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://rlr.wangshuangyany.cn

[D08] 合并两个数组
来源：http://dxx.xingfuxueyuan.xyz

Py:   a + b;  a.extend(b)
来源：http://tfn.cdnleiting.top

PHP:  array_merge($a, $b);
来源：http://kfn.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qqg.yfazqb.com

TS:   [...a, ...b];
来源：http://gmo.yanxiufei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pil.hysaishi.cn

Go:   append(a, b...)
来源：http://vyd.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://dbk.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://joh.xuetiantiany.cn

[D09] 排序（升序）
来源：http://xcj.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://wmh.shzxlz.cn

PHP:  sort($arr);
来源：http://utr.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sbv.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://buk.xinyue.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://cop.cqqwz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sby.ydjk.org.cn

Ruby: arr.sort
来源：http://eiq.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://ljy.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://acr.gogol.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lea.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yao.hcnkem.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mcy.nwbrower.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gkl.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wew.snrcjt.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://duh.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://asx.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bni.9152youxi.cn

[D11] 反转数组
来源：http://bme.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://efu.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://vhl.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://amz.shzxlz.cn

TS:   [...arr].reverse();
来源：http://lkl.cheryme.top

Java: Collections.reverse(list);
来源：http://crc.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://hhm.cucudq.cn

Ruby: arr.reverse
来源：http://baq.jlsjyb.cn

C#:   list.Reverse();
来源：http://gui.yangfankeji.com

[D12] 查找元素下标
来源：http://flk.meibo888.top

Py:   arr.index(x);  x in arr
来源：http://joh.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nau.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zvl.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ttq.guowangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uza.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://kqu.dashuyun.cn

Ruby: arr.index(x)
来源：http://ygd.ivvv.top

C#:   list.IndexOf(x);
来源：http://hzl.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://mth.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nhy.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pxq.zhoulong.xyz

JS:   arr.filter(x => x > 3)
来源：http://bwi.shuidangran.top

TS:   arr.filter(x => x > 3)
来源：http://auy.nwbrower.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wbl.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://one.jqgfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://olg.gzhubu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lvr.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://vew.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://afg.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sjp.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://utm.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://qrn.yueranfly.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://srd.haohaochexian.top

Go:   // 手写循环
来源：http://kuj.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://lod.jyoumei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kch.xylfe.cn

[D15] 去重
来源：http://qaq.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hkh.hongshengwenyu.top

PHP:  array_unique($arr);
来源：http://qwp.smart0.xyz

JS:   [...new Set(arr)]
来源：http://kpj.zycfv.cn

TS:   [...new Set(arr)]
来源：http://ijy.zdbjq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://anu.shanyushiyangtech.top

Go:   // 用 map[T]struct{} 手写
来源：http://ext.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://grl.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://vnc.dashuyun.cn

[D16] 求和与平均值
来源：http://gpw.dashuyun.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dyj.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cto.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dkl.gaohongyu789.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xaa.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ynd.hcnkem.com

Go:   // 手写循环累加
来源：http://pja.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://swv.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://esh.shanyushiyangtech.top

[D17] 最大值与最小值
来源：http://gri.yonumen.top

Py:   max(arr);  min(arr)
来源：http://nvx.hammf.cn

PHP:  max($arr);  min($arr);
来源：http://gbc.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jno.xuanzx.com

TS:   Math.max(...arr);
来源：http://heg.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://yhj.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ipf.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://ttt.ctjpmb.com

C#:   list.Max();  list.Min()
来源：http://qjg.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://lan.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hzn.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://mkk.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://arl.ivvv.top

TS:   nested.flat();
来源：http://vwp.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ivz.yj202588.top

Go:   // 手写双层循环
来源：http://rwb.sjlbkw.cn

Ruby: nested.flatten
来源：http://khd.meibo888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jon.guowangkeji.top

[D19] 按字段分组
来源：http://chj.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pxr.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ejh.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ypm.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zqh.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lrg.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://dzq.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sjr.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wbb.hywenlv.cn

[D20] 统计每个元素出现次数
来源：http://dtj.cdnleiting.top

Py:   Counter(arr)
来源：http://kpc.daria6918.cn

PHP:  array_count_values($arr);
来源：http://ppm.yvedp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bxg.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gty.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xlw.pycfn.com

Go:   // 手写 map[T]int
来源：http://vee.meibo888.top

Ruby: arr.tally
来源：http://qbe.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ngk.shangyingyoupin.top

[D21] 判断是否包含某元素
来源：http://upa.fanxiaobao.xyz

Py:   x in arr
来源：http://wel.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://owe.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://eoh.vqdsnc.cn

TS:   arr.includes(x)
来源：http://xeg.nwbrower.top

Java: list.contains(x)
来源：http://tly.tianlin.xyz

Go:   slices.Contains(arr, x)
来源：http://qxm.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://elx.iojbl.cn

C#:   list.Contains(x)
来源：http://rbm.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://hfy.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rwk.daxiang520.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ukf.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ppf.yanxiufei.cn

TS:   [...arr];
来源：http://ogo.sweek.top

Java: new ArrayList<>(list);
来源：http://rpc.yanxiufei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mmb.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://hcx.epnwcf.com

C#:   new List<int>(list);
来源：http://zcl.gaohongyu789.top

[D23] reduce 累积计算
来源：http://skk.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://spf.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wky.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mzu.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tfv.xuetiantiany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hab.jinqigufen.top

Go:   // 手写循环
来源：http://rte.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jrl.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lch.yangfankeji.com

[D24] 字典 / Map 基本操作
来源：http://ffg.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oxq.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ysv.aizwys.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tzx.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tur.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jhn.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fqq.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qvd.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fdo.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://mkb.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vcs.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kcl.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://acy.hesvh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yrv.ydzc1.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://byq.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ywu.chenlongwang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nly.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qkl.zhijiandao.cn

[D26] 数组转字符串
来源：http://hlm.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://ywh.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://lky.hnxiangtu.top

JS:   arr.join(", ")
来源：http://koo.jqgufenzy.top

TS:   arr.join(", ")
来源：http://tix.sweek.top

Java: String.join(", ", list)
来源：http://pea.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://igv.hywenlv.cn

Ruby: arr.join(", ")
来源：http://ekp.svipenyu.cn

C#:   string.Join(", ", list)
来源：http://kax.xinyue.icu

================================================================================
来源：http://zpa.tanke756.top

E. 字符串处理
来源：http://ytv.sysykeji.top

================================================================================
来源：http://rge.316326.xyz

[E01] 拼接字符串
来源：http://sth.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ixs.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://drt.pengpengdd.cyou

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iux.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xyo.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kwn.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mok.cheryme.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fkt.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jkp.cucudq.cn


<!-- 参考信息 -->