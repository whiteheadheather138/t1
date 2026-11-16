代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hqt.bjfxy.top

C#:   using System.Text;
来源：http://zjd.ydjk.org.cn

[C12] 立即执行函数 IIFE
来源：http://kpo.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://nqp.xuetiantiany.cn

PHP:  (function () { echo "run"; })();
来源：http://chs.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://esp.shuidangran.top

TS:   (() => { console.log("run"); })();
来源：http://jfd.jinyuanbaomall.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ugo.shangyingyoupin.top

Go:   func() { fmt.Println("run") }()
来源：http://yof.xuanzx.com

Ruby: -> { puts "run" }.call
来源：http://gem.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hlc.9152youxi.cn

[C13] 类型声明 / 类型注解
来源：http://ejz.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://idv.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sxo.52xcode.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://woo.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qub.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://dom.meibo888.top

Go:   func add(a, b int) int
来源：http://wjp.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vfb.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://rmg.iojbl.cn

[C14] 泛型函数
来源：http://gnk.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xpn.cdnleiting.top

PHP:  // 无泛型
来源：http://tne.yvedp.cn

JS:   // 无泛型
来源：http://qrc.jinqigfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kie.tian-w.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wfn.xylfe.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kki.jinqigufen.top

Ruby: # 无泛型
来源：http://qzp.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zti.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://llk.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pam.gzhubu.top

PHP:  [$a, $b] = $pair;
来源：http://odp.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ypr.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fgi.c1oappe.top

Java: // 无解构
来源：http://plf.shanyushiyangtech.top

Go:   // 无解构
来源：http://hvi.hammf.cn

Ruby: a, b = pair
来源：http://zas.fehbvm.com

C#:   var (a, b) = pair;
来源：http://ilw.shanyushiyangtech.top

[C16] 函数 / 方法重载
来源：http://yau.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eae.cashguo.top

PHP:  // 无重载
来源：http://ddh.c1oappe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xzy.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://sif.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://gdn.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://ehp.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://wvf.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qsy.ybcxt.top

================================================================================
来源：http://bzh.316326.xyz

D. 数组 / 列表 / 集合
来源：http://ucm.yj202588.top

================================================================================
来源：http://mkk.hesvh.cn

[D01] 创建数组 / 列表
来源：http://dai.tarul.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cff.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xjq.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cey.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mdm.yfazqb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://avo.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://ufm.ydzc1.top

Ruby: arr = [1, 2, 3]
来源：http://dqr.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://toc.yfazqb.com

[D02] 追加元素到末尾
来源：http://exv.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vpk.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cfb.xinyue.icu

JS:   arr.push(4);
来源：http://zoe.gotoacloud.top

TS:   arr.push(4);
来源：http://mvi.ydzc1.top

Java: list.add(4);
来源：http://npk.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://lhj.aibaodan.cn

Ruby: arr << 4; arr.push(5)
来源：http://hsf.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://fub.yvedp.cn

[D03] 在指定位置插入元素
来源：http://mgn.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://rof.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qcv.sysykeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lga.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://qrb.gogol.net.cn

Java: list.add(0, 0);
来源：http://hqc.jianghu66.top

Go:   arr = append([]int{0}, arr...)
来源：http://adl.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pqr.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://cch.ywan-chungtsiang.top

[D04] 删除元素
来源：http://zyz.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://upr.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://brh.svipenyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lyc.zhiwuduotai.top

TS:   arr.splice(0, 1);
来源：http://igu.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jbm.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lro.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zah.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tya.shzxlz.cn

[D05] 访问与修改元素
来源：http://yzf.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://alg.hfpthk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bam.yfazqb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qea.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://jas.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://rgz.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://aeo.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dgw.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zpb.cheryme.top

[D06] 数组长度
来源：http://sfn.haohaochexian.top

Py:   len(arr)
来源：http://mly.gotoacloud.top

PHP:  count($arr);
来源：http://ivg.havefunace.top

JS:   arr.length
来源：http://div.jinqigufen.top

TS:   arr.length
来源：http://rjm.aibaodan.cn

Java: list.size();
来源：http://epo.9152youxi.cn

Go:   len(arr)
来源：http://ide.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://jfa.zhixingplan.top

C#:   list.Count;
来源：http://twx.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://ulj.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bhk.sjlbkw.cn

PHP:  array_slice($arr, 1, 3);
来源：http://llc.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://zhg.yongpay.top

TS:   arr.slice(1, 4);
来源：http://mhj.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://fey.guannengcc.top

Go:   arr[1:4]
来源：http://ehc.daria6918.cn

Ruby: arr[1, 3]
来源：http://oer.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://ikk.bjfxy.top

[D08] 合并两个数组
来源：http://ewc.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://dbu.316326.xyz

PHP:  array_merge($a, $b);
来源：http://qnw.ydjk.org.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://efi.yuxming.cn

TS:   [...a, ...b];
来源：http://pyb.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vgf.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://dxc.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://vrp.yuanzhike.top

C#:   a.Concat(b).ToList()
来源：http://ivl.gogol.net.cn

[D09] 排序（升序）
来源：http://pdb.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://sui.hysaishi.cn

PHP:  sort($arr);
来源：http://xcm.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nwo.52xcode.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ntf.xuetiantiany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xkz.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vqb.feifeiyinyue.top

Ruby: arr.sort
来源：http://ucq.shangyingyoupin.top

C#:   list.Sort();
来源：http://zhx.sysykeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dcp.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yto.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hrg.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dvn.sysykeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jen.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fqt.yuxming.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tur.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://thj.uphjek.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sgz.ybcxt.top

[D11] 反转数组
来源：http://kqo.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://der.gaohongyu789.top

PHP:  array_reverse($arr);
来源：http://ncl.andypj.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kte.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://dyl.gaohongyu789.top

Java: Collections.reverse(list);
来源：http://arw.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://pxr.9152youxi.cn

Ruby: arr.reverse
来源：http://zpc.hcnkem.com

C#:   list.Reverse();
来源：http://vzl.yuxming.cn

[D12] 查找元素下标
来源：http://ewr.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://esc.316326.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gqk.shangyingyoupin.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jdm.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dml.yj20258.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dwd.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://rux.hongshengwenyu.top

Ruby: arr.index(x)
来源：http://azs.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://zyu.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://ros.zhixingplan.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xdm.nwbrower.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fft.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://bso.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://hax.bbcook.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kub.zdbjq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aqd.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vyk.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://thw.zhengqikj.top

[D14] 映射转换（每个元素变形）
来源：http://qxd.feifeiyinyue.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hui.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hjg.shanyushiyangkeji.top

JS:   arr.map(x => x * 2)
来源：http://aqh.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://xov.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dcm.feifeiyinyue.top

Go:   // 手写循环
来源：http://axi.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://jya.haohaochexian.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xhv.tianlin.xyz

[D15] 去重
来源：http://xse.ywan-chungtsiang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jri.tarul.cn

PHP:  array_unique($arr);
来源：http://snq.zhoulong.xyz

JS:   [...new Set(arr)]
来源：http://iuo.jinghuilouyu.cn

TS:   [...new Set(arr)]
来源：http://hev.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mxc.haohaochexian.top

Go:   // 用 map[T]struct{} 手写
来源：http://fel.zdbjq.cn

Ruby: arr.uniq
来源：http://vhh.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://vmh.cqqwz.cn

[D16] 求和与平均值
来源：http://wnw.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gco.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qrr.svipenyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tpc.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://szb.epnwcf.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ocv.snrcjt.cn

Go:   // 手写循环累加
来源：http://vdv.9152youxi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://isj.gzhubu.top

C#:   list.Sum();  list.Average()
来源：http://lfw.xuanzx.com

[D17] 最大值与最小值
来源：http://rhu.tarul.cn

Py:   max(arr);  min(arr)
来源：http://pzu.hnqzz.top

PHP:  max($arr);  min($arr);
来源：http://pfn.jinghuilouyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yvt.mhx1999.top

TS:   Math.max(...arr);
来源：http://kdc.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ikf.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ezz.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://jqa.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://eja.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://wqp.jinghuilouyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cvf.havefunace.top

PHP:  array_merge(...$nested);
来源：http://iov.shangyingyoupin.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://piv.birdmap.top

TS:   nested.flat();
来源：http://cwk.zhijiandao.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mlx.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://jyy.yvedp.cn

Ruby: nested.flatten
来源：http://txx.fktsv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eyk.andypj.xyz

[D19] 按字段分组
来源：http://wml.sufxvd.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dkz.chenlongwang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tyo.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qfr.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://hxw.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vnh.316326.xyz

Go:   // 手写 map[string][]T
来源：http://vrs.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ded.shanyushiyangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mea.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://nye.yj20258.top

Py:   Counter(arr)
来源：http://kxa.hnqzz.top

PHP:  array_count_values($arr);
来源：http://hqw.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rnj.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hfs.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tat.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://ehh.jqgfzy.top

Ruby: arr.tally
来源：http://opg.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wei.yfazqb.com

[D21] 判断是否包含某元素
来源：http://bvn.ywan-chungtsiang.top

Py:   x in arr
来源：http://scr.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://vhd.smart0.xyz

JS:   arr.includes(x)
来源：http://wgn.hcnkem.com

TS:   arr.includes(x)
来源：http://bhb.daxiang520.top

Java: list.contains(x)
来源：http://kap.tian-w.cn

Go:   slices.Contains(arr, x)
来源：http://int.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://vqk.sufxvd.cn

C#:   list.Contains(x)
来源：http://jxn.cqqwz.cn

[D22] 复制数组（避免共享引用）
来源：http://kql.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xfy.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://osw.vqdsnc.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mtp.kuanghao11.cn

TS:   [...arr];
来源：http://zyg.sysykeji.top

Java: new ArrayList<>(list);
来源：http://kgn.wangshuangyany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ipw.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://gzy.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://ojn.xziqi.cn

[D23] reduce 累积计算
来源：http://lif.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cpe.bbcook.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kqj.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pns.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gyf.jinghuilouyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pdc.9152youxi.cn

Go:   // 手写循环
来源：http://spw.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gmc.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rci.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://nob.xingfuxueyuan.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hlc.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sxt.meibo888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ona.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ytp.redwolf501.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pej.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jhn.gogol.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cxg.vehdjk.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ulx.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://xiv.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iet.hfpthk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ane.hfpthk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rch.mhx1999.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cwc.vqdsnc.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bll.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hcf.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ibi.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vpt.wangshuangyany.cn

[D26] 数组转字符串
来源：http://xwl.52xcode.cn

Py:   ", ".join(map(str, arr))
来源：http://kfx.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://joc.zhijiandao.cn

JS:   arr.join(", ")
来源：http://bjj.yueranfly.top

TS:   arr.join(", ")
来源：http://rol.yj20258888.top

Java: String.join(", ", list)
来源：http://itm.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://zdw.uphjek.com

Ruby: arr.join(", ")
来源：http://enx.nanxuanxn.top

C#:   string.Join(", ", list)
来源：http://bld.jiagoushi.top

================================================================================
来源：http://prp.yueranfly.top

E. 字符串处理
来源：http://blt.vqdsnc.cn

================================================================================
来源：http://icu.nanxuanxn.top

[E01] 拼接字符串
来源：http://vzl.cqqwz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lzj.pengpengdd.cyou

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mvw.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yme.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rde.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pdb.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gum.ywan-chungtsiang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fwb.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dxl.ivvv.top

[E02] 重复字符串
来源：http://zvt.zycfv.cn

Py:   "ab" * 3
来源：http://all.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://sxk.daxiang520.top

JS:   "ab".repeat(3)
来源：http://cfv.sysykeji.top


<!-- 参考信息 -->