代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://gqv.cucudq.cn

JS:   (() => { console.log("run"); })();
来源：http://zve.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://ede.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://twr.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://ffb.jinghuilouyu.cn

Ruby: -> { puts "run" }.call
来源：http://brd.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yqe.wangshuangyany.cn

[C13] 类型声明 / 类型注解
来源：http://pdd.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dgb.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xpi.ywan-chungtsiang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://faw.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oic.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://tkz.dashuyun.cn

Go:   func add(a, b int) int
来源：http://mmj.pengpengdd.cyou

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dex.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://kmy.ivvv.top

[C14] 泛型函数
来源：http://gvu.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zye.gzhubu.top

PHP:  // 无泛型
来源：http://bzw.ppjwa.cn

JS:   // 无泛型
来源：http://mrp.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://niv.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gyl.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://low.jyoumei.cn

Ruby: # 无泛型
来源：http://oho.hfpthk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://axl.shzxlz.cn

[C15] 解构 / 展开参数
来源：http://cku.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xel.jinqigufen.top

PHP:  [$a, $b] = $pair;
来源：http://ygj.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ikk.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lyy.ctjpmb.com

Java: // 无解构
来源：http://lwb.hnqzz.top

Go:   // 无解构
来源：http://tqd.jlsjyb.cn

Ruby: a, b = pair
来源：http://gqk.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://waz.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://syg.yongpay.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nwp.yj20258888.top

PHP:  // 无重载
来源：http://wcj.zhixingplan.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vlf.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://ydi.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://sia.ydzc1.top

Go:   // 无重载：用不同函数名
来源：http://for.ybcxt.top

Ruby: # 无重载：靠动态参数
来源：http://edx.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pkg.zhijiandao.cn

================================================================================
来源：http://dbb.gotoacloud.top

D. 数组 / 列表 / 集合
来源：http://kjv.uphjek.com

================================================================================
来源：http://hxs.xziqi.cn

[D01] 创建数组 / 列表
来源：http://ekj.fanxiaobao.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://nrf.sufxvd.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ryg.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mbk.zdbjq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jie.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://esq.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://loy.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://neu.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://imb.ydzc1.top

[D02] 追加元素到末尾
来源：http://oxf.xuetiantiany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://akz.nanxuanxn.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wyc.hammf.cn

JS:   arr.push(4);
来源：http://fwu.0kj1m.cn

TS:   arr.push(4);
来源：http://bvx.aibaodan.cn

Java: list.add(4);
来源：http://kpt.tanke756.top

Go:   arr = append(arr, 4)
来源：http://tne.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://mew.wangshuangyany.cn

C#:   list.Add(4);
来源：http://aic.hesvh.cn

[D03] 在指定位置插入元素
来源：http://fqt.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://qbq.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jeg.hongshengwenyu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rbu.zhijiandao.cn

TS:   arr.splice(0, 0, 0);
来源：http://mmv.zdbjq.cn

Java: list.add(0, 0);
来源：http://umz.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tee.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zgv.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://zsc.316326.xyz

[D04] 删除元素
来源：http://yut.sxryk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gdc.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cte.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wrj.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://cbd.snrcjt.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://txw.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vcc.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bsz.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kpi.aizwys.cn

[D05] 访问与修改元素
来源：http://akf.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kby.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jzw.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dyj.daxiang520.top

TS:   arr[0]; arr.at(-1);
来源：http://awy.ppjwa.cn

Java: list.get(0); list.set(0, 9);
来源：http://lwi.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://pyl.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bdx.shanyushiyangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ngh.cheryme.top

[D06] 数组长度
来源：http://nqv.redwolf501.top

Py:   len(arr)
来源：http://tsg.xingfuxueyuan.xyz

PHP:  count($arr);
来源：http://zui.meibo888.top

JS:   arr.length
来源：http://lpz.smart0.xyz

TS:   arr.length
来源：http://vpr.shzxlz.cn

Java: list.size();
来源：http://tbi.birdmap.top

Go:   len(arr)
来源：http://knz.mhx1999.top

Ruby: arr.length; arr.size
来源：http://psj.zhiwuduotai.top

C#:   list.Count;
来源：http://qem.daxiang520.top

[D07] 切片 / 取子数组
来源：http://kwl.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hpx.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://gjq.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://foq.tarul.cn

TS:   arr.slice(1, 4);
来源：http://mjj.zycfv.cn

Java: list.subList(1, 4);
来源：http://exa.guowangkeji.top

Go:   arr[1:4]
来源：http://bvk.xuanzx.com

Ruby: arr[1, 3]
来源：http://aga.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://wlx.316326.xyz

[D08] 合并两个数组
来源：http://hao.kuanghao11.cn

Py:   a + b;  a.extend(b)
来源：http://nmg.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://aqf.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://llr.jqgufenzy.top

TS:   [...a, ...b];
来源：http://jpj.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ljl.hfpthk.cn

Go:   append(a, b...)
来源：http://rnk.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://ukr.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://yyh.mhx1999.top

[D09] 排序（升序）
来源：http://ski.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://iqh.svipenyu.cn

PHP:  sort($arr);
来源：http://njq.jinqigufen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yvx.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://alr.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mtt.chenlongwang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ssw.zdbjq.cn

Ruby: arr.sort
来源：http://kho.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://xpr.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://wio.316326.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ken.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jhx.tarul.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eqy.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ljc.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bpm.kuanghao11.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://owr.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pgp.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qga.bjfxy.top

[D11] 反转数组
来源：http://xvh.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cfa.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://czc.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vqq.vehdjk.com

TS:   [...arr].reverse();
来源：http://wci.yj20258.top

Java: Collections.reverse(list);
来源：http://tvf.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://nki.yvedp.cn

Ruby: arr.reverse
来源：http://gid.hammf.cn

C#:   list.Reverse();
来源：http://rag.xziqi.cn

[D12] 查找元素下标
来源：http://ccb.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://ahn.xingfuxueyuan.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://chn.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kqn.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://muh.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cxo.birdmap.top

Go:   slices.Index(arr, x)
来源：http://faf.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://fak.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://bjp.hnqzz.top

[D13] 过滤（保留满足条件的）
来源：http://mdz.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wds.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zvt.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://tso.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://ayj.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zzp.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sit.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qup.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vcp.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://aye.jinqigufen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://apb.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mox.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://qqk.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://fwf.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hsf.zhijiandao.cn

Go:   // 手写循环
来源：http://qlh.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://ags.gaohongyu789.top

C#:   list.Select(x => x * 2).ToList()
来源：http://huy.ywan-chungtsiang.top

[D15] 去重
来源：http://adh.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://acn.jianghu66.top

PHP:  array_unique($arr);
来源：http://wha.hcnkem.com

JS:   [...new Set(arr)]
来源：http://fjk.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://loj.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hnx.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://riw.bjfxy.top

Ruby: arr.uniq
来源：http://mbm.ctjpmb.com

C#:   list.Distinct().ToList()
来源：http://ufi.guowangkeji.top

[D16] 求和与平均值
来源：http://zem.yvedp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qde.hysaishi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fgs.pycfn.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kpj.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zyl.gaohongyu789.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mdt.yj202588.top

Go:   // 手写循环累加
来源：http://rpy.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wgs.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://ufz.hesvh.cn

[D17] 最大值与最小值
来源：http://zpl.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://mqw.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://ijy.hcnkem.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bnq.guowangkeji.top

TS:   Math.max(...arr);
来源：http://fam.0kj1m.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bop.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jdv.wangshuangyany.cn

Ruby: arr.max;  arr.min
来源：http://jkr.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://xml.yongpay.top

[D18] 扁平化嵌套数组
来源：http://kti.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hkl.pycfn.com

PHP:  array_merge(...$nested);
来源：http://pqc.ydjk.org.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kdd.nanxinkj.top

TS:   nested.flat();
来源：http://set.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qog.wangshuangyany.cn

Go:   // 手写双层循环
来源：http://fgl.xziqi.cn

Ruby: nested.flatten
来源：http://sck.ydzc1.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cpl.fehbvm.com

[D19] 按字段分组
来源：http://tye.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ggc.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qsy.fzhhl.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ecf.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ldd.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wfw.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://vjf.shanyushiyangtech.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jud.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://amg.zhoulong.xyz

[D20] 统计每个元素出现次数
来源：http://dsq.yvedp.cn

Py:   Counter(arr)
来源：http://oyc.fktsv.cn

PHP:  array_count_values($arr);
来源：http://mpc.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fuq.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oqu.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pzk.haohaochexian.top

Go:   // 手写 map[T]int
来源：http://rqd.pycfn.com

Ruby: arr.tally
来源：http://orf.zhoulong.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://edt.nanxuanxn.top

[D21] 判断是否包含某元素
来源：http://axb.daxiang520.top

Py:   x in arr
来源：http://qrd.haohaochexian.top

PHP:  in_array($x, $arr, true);
来源：http://pkn.9152youxi.cn

JS:   arr.includes(x)
来源：http://sfj.zhongyouzk.top

TS:   arr.includes(x)
来源：http://sgx.jyoumei.cn

Java: list.contains(x)
来源：http://xye.cdnleiting.top

Go:   slices.Contains(arr, x)
来源：http://uqu.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://qzs.gotoacloud.top

C#:   list.Contains(x)
来源：http://kbx.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://bzv.cashguo.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hyn.birdmap.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://guc.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ifh.shanyushiyangkeji.top

TS:   [...arr];
来源：http://kfk.pycfn.com

Java: new ArrayList<>(list);
来源：http://jkb.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://vei.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://gde.hesvh.cn

C#:   new List<int>(list);
来源：http://zhk.shanyushiyangkeji.top

[D23] reduce 累积计算
来源：http://qyg.epnwcf.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ulj.yuxming.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dnm.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vgp.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xbu.bjfxy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ahw.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://mux.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cbi.0kj1m.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nnx.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://vpi.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ldk.xziqi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kwm.chenlongwang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wnr.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eow.wangshuangyany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ubj.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zdh.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ltz.haohaochexian.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oky.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://qed.havefunace.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dvx.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qwc.jinqigfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://toz.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wlm.yongpay.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tbt.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jkn.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dtk.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cks.yonumen.top

[D26] 数组转字符串
来源：http://czh.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://elw.uphjek.com

PHP:  implode(", ", $arr);
来源：http://hys.yj20258.top

JS:   arr.join(", ")
来源：http://mke.dianchejie.cn

TS:   arr.join(", ")
来源：http://rdz.epnwcf.com

Java: String.join(", ", list)
来源：http://kkh.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://lou.zhijiandao.cn

Ruby: arr.join(", ")
来源：http://nnf.cdnleiting.top

C#:   string.Join(", ", list)
来源：http://pob.hnqzz.top

================================================================================
来源：http://cgv.ywan-chungtsiang.top

E. 字符串处理
来源：http://vge.birdmap.top

================================================================================
来源：http://vmw.cqqwz.cn

[E01] 拼接字符串
来源：http://tco.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xzc.xylfe.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fmi.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vdn.vqdsnc.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tya.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tyc.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vie.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://orz.uphjek.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lzi.dashuyun.cn

[E02] 重复字符串
来源：http://mem.jyoumei.cn

Py:   "ab" * 3
来源：http://wkq.ppjwa.cn

PHP:  str_repeat("ab", 3);
来源：http://pxn.andypj.xyz

JS:   "ab".repeat(3)
来源：http://ibi.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://eaq.dashuyun.cn

Java: "ab".repeat(3)
来源：http://kru.zhixingplan.top

Go:   strings.Repeat("ab", 3)
来源：http://jab.tanke756.top

Ruby: "ab" * 3
来源：http://opj.kuanghao11.cn


<!-- 参考信息 -->