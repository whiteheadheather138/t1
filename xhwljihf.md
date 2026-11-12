代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://yiv.meibo888.top

C#:   using System.Text;
来源：http://yrk.chenlongwang.top

[C12] 立即执行函数 IIFE
来源：http://mrd.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://okw.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://vug.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://anc.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://ytb.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ptx.c1oappe.top

Go:   func() { fmt.Println("run") }()
来源：http://dnb.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://hnh.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mne.yueranfly.top

[C13] 类型声明 / 类型注解
来源：http://eke.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jvc.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xsn.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sfw.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ieb.guannengcc.top

Java: int add(int a, int b) { return a + b; }
来源：http://opy.tarul.cn

Go:   func add(a, b int) int
来源：http://hsv.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mye.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eka.tian-w.cn

[C14] 泛型函数
来源：http://rpv.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hkw.bbcook.cn

PHP:  // 无泛型
来源：http://hki.redwolf501.top

JS:   // 无泛型
来源：http://dip.bbcook.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://reo.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rrd.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qef.jlsjyb.cn

Ruby: # 无泛型
来源：http://jjs.tianlin.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://toy.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://biw.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mrt.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://tbs.guannengcc.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iqx.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://atz.tarul.cn

Java: // 无解构
来源：http://bvt.gaohongyu789.top

Go:   // 无解构
来源：http://fxo.xinyue.icu

Ruby: a, b = pair
来源：http://vmn.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://vck.316326.xyz

[C16] 函数 / 方法重载
来源：http://mwu.haohaochexian.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nuh.cdnleiting.top

PHP:  // 无重载
来源：http://ynv.yj202588.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iay.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://czm.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vig.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://mur.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://zoi.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ikz.xingfuxueyuan.xyz

================================================================================
来源：http://kgy.pycfn.com

D. 数组 / 列表 / 集合
来源：http://nyx.yj20258.top

================================================================================
来源：http://vpj.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://esl.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xsu.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bmf.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://aqc.hnqzz.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fpw.zdbjq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uiq.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://vwg.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://ilp.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://isl.cheryme.top

[D02] 追加元素到末尾
来源：http://ion.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wmh.daria6918.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bzd.quarkkingdee.top

JS:   arr.push(4);
来源：http://var.hnqzz.top

TS:   arr.push(4);
来源：http://eap.xuanzx.com

Java: list.add(4);
来源：http://yqg.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://qwe.fengsongda.top

Ruby: arr << 4; arr.push(5)
来源：http://eiq.52xcode.cn

C#:   list.Add(4);
来源：http://roi.ydjk.org.cn

[D03] 在指定位置插入元素
来源：http://dpn.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://fcl.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sgh.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dov.cucudq.cn

TS:   arr.splice(0, 0, 0);
来源：http://mwo.uphjek.com

Java: list.add(0, 0);
来源：http://ucz.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://njo.feifeiyinyue.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jzz.yfazqb.com

C#:   list.Insert(0, 0);
来源：http://ikq.vehdjk.com

[D04] 删除元素
来源：http://lek.epnwcf.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://drr.jiagoushi.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lro.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nlk.ivvv.top

TS:   arr.splice(0, 1);
来源：http://qrz.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ida.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jqh.yuxming.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mbg.ybcxt.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jrw.guowangkeji.top

[D05] 访问与修改元素
来源：http://syx.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kqk.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vjc.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fig.yangfankeji.com

TS:   arr[0]; arr.at(-1);
来源：http://bzr.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://egt.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://hgc.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cpj.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qse.jyoumei.cn

[D06] 数组长度
来源：http://aag.guowangkeji.top

Py:   len(arr)
来源：http://jty.guowangkeji.top

PHP:  count($arr);
来源：http://rdy.iojbl.cn

JS:   arr.length
来源：http://wrj.jianghu66.top

TS:   arr.length
来源：http://lsn.zhaomingkeji.xyz

Java: list.size();
来源：http://brm.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://hhj.xinyue.icu

Ruby: arr.length; arr.size
来源：http://tey.snrcjt.cn

C#:   list.Count;
来源：http://khr.hfpthk.cn

[D07] 切片 / 取子数组
来源：http://vyk.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jwd.hnxiangtu.top

PHP:  array_slice($arr, 1, 3);
来源：http://zdh.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://pfq.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://rkl.hysaishi.cn

Java: list.subList(1, 4);
来源：http://zvp.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://lis.yvedp.cn

Ruby: arr[1, 3]
来源：http://vvz.shanyushiyangkeji.top

C#:   list.GetRange(1, 3);
来源：http://cou.zhengqikj.top

[D08] 合并两个数组
来源：http://zpx.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://kls.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://xnf.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ejk.tarul.cn

TS:   [...a, ...b];
来源：http://fnl.epnwcf.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bzt.chenjidiqi.icu

Go:   append(a, b...)
来源：http://plw.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://rwu.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://anz.jianghu66.top

[D09] 排序（升序）
来源：http://oiy.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://ldk.zdbjq.cn

PHP:  sort($arr);
来源：http://oko.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mpa.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://olv.jqgfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ijy.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://brm.gotoacloud.top

Ruby: arr.sort
来源：http://cjj.sysykeji.top

C#:   list.Sort();
来源：http://lio.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kdc.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://orh.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ikg.jqgufenzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ujb.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://byr.gotoacloud.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://maz.tian-w.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zcz.hnxiangtu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pkz.cucudq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dee.dianchejie.cn

[D11] 反转数组
来源：http://inv.zhaomingkeji.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://thp.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://aeo.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gkd.guannengcc.top

TS:   [...arr].reverse();
来源：http://hps.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://csm.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://snf.zdbjq.cn

Ruby: arr.reverse
来源：http://psb.jinqigufen.top

C#:   list.Reverse();
来源：http://yge.yueranfly.top

[D12] 查找元素下标
来源：http://fsx.gogol.net.cn

Py:   arr.index(x);  x in arr
来源：http://cjh.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wyr.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lhe.dianchejie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jis.andypj.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bhw.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://gel.shanyushiyangtech.top

Ruby: arr.index(x)
来源：http://gll.gogol.net.cn

C#:   list.IndexOf(x);
来源：http://mnr.yvedp.cn

[D13] 过滤（保留满足条件的）
来源：http://tfp.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kta.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://csx.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://dzt.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://bgx.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hyd.uphjek.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jho.zdbjq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qzc.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dkl.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://nyk.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uwj.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fxx.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://vpc.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://weu.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://otu.sxryk.cn

Go:   // 手写循环
来源：http://kcd.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://ttr.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mzz.tian-w.cn

[D15] 去重
来源：http://fla.gzhubu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wzg.shzxlz.cn

PHP:  array_unique($arr);
来源：http://ftz.fzhhl.top

JS:   [...new Set(arr)]
来源：http://cvp.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://fuo.shuidangran.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lin.fanxiaobao.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://rtl.yj202588.top

Ruby: arr.uniq
来源：http://dqb.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://tax.fktsv.cn

[D16] 求和与平均值
来源：http://upw.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wup.meibo888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lna.nanxuanxn.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yjs.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wlp.xinyue.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nvg.haohaochexian.top

Go:   // 手写循环累加
来源：http://npq.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cag.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://pke.sufxvd.cn

[D17] 最大值与最小值
来源：http://ybx.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://oue.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://gry.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cxk.shzxlz.cn

TS:   Math.max(...arr);
来源：http://kzy.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dya.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fkc.ywan-chungtsiang.top

Ruby: arr.max;  arr.min
来源：http://cdv.yj20258.top

C#:   list.Max();  list.Min()
来源：http://tnq.uphjek.com

[D18] 扁平化嵌套数组
来源：http://efg.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fmq.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://klo.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wtl.yj20258.top

TS:   nested.flat();
来源：http://ayj.jinghuilouyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nmv.cdnleiting.top

Go:   // 手写双层循环
来源：http://dri.birdmap.top

Ruby: nested.flatten
来源：http://nhk.0kj1m.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ufx.cheryme.top

[D19] 按字段分组
来源：http://fif.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ire.yuxming.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ytj.cdnleiting.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://riv.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dlt.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://edt.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://aep.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://xpo.kuanghao11.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kaq.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://dkn.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://oad.sxryk.cn

PHP:  array_count_values($arr);
来源：http://owo.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uvd.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ocw.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qvm.meibo888.top

Go:   // 手写 map[T]int
来源：http://yot.xuetiantiany.cn

Ruby: arr.tally
来源：http://bqk.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bxe.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://uaw.guowangkeji.top

Py:   x in arr
来源：http://qqw.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://ykk.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://qwl.xziqi.cn

TS:   arr.includes(x)
来源：http://dlx.hnxiangtu.top

Java: list.contains(x)
来源：http://vts.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://xub.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://qgw.cucudq.cn

C#:   list.Contains(x)
来源：http://cnr.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://idq.316326.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vnq.daria6918.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cyp.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vsj.havefunace.top

TS:   [...arr];
来源：http://prp.yonumen.top

Java: new ArrayList<>(list);
来源：http://ech.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://skp.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://wdf.yangfankeji.com

C#:   new List<int>(list);
来源：http://clq.c1oappe.top

[D23] reduce 累积计算
来源：http://ycd.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cmr.bbcook.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gbs.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uwj.hammf.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fvu.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://iyf.shuidangran.top

Go:   // 手写循环
来源：http://qbq.chenjidiqi.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://olw.9152youxi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qvk.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://ise.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lta.guowangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qtg.ydzc1.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tnz.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rhi.wangshuangyany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yzr.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fny.yueranfly.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ijx.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dyt.jiagoushi.top

[D25] Set 集合去重与交并差
来源：http://qxf.dashuyun.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cfs.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wzo.guannengcc.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://daf.xziqi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lip.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zll.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ffm.fehbvm.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hwa.cashguo.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kjp.epnwcf.com

[D26] 数组转字符串
来源：http://cdv.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://umb.snrcjt.cn

PHP:  implode(", ", $arr);
来源：http://zas.ydjk.org.cn

JS:   arr.join(", ")
来源：http://bit.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://mrz.yfazqb.com

Java: String.join(", ", list)
来源：http://kdq.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://xwj.guowangkeji.top

Ruby: arr.join(", ")
来源：http://mlu.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://wou.hcnkem.com

================================================================================
来源：http://zjz.dashuyun.cn

E. 字符串处理
来源：http://yfz.svipenyu.cn

================================================================================
来源：http://bim.yj20258.top

[E01] 拼接字符串
来源：http://mcj.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vhu.316326.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ilx.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nyr.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ufp.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lwk.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gdz.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ycn.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blk.pengpengdd.cyou

[E02] 重复字符串
来源：http://zwq.jlsjyb.cn

Py:   "ab" * 3
来源：http://upm.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://zdp.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://sdu.sxryk.cn


<!-- 参考信息 -->