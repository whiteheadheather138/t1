代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://opn.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://shd.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aeh.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jmt.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://rqs.fktsv.cn

Go:   func add(a, b int) int
来源：http://boe.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://syn.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://uhq.gaohongyu789.top

[C14] 泛型函数
来源：http://pyz.xuetiantiany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tpd.yj20258.top

PHP:  // 无泛型
来源：http://gtt.xuanzx.com

JS:   // 无泛型
来源：http://bmr.redwolf501.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://okv.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://png.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ige.yj202588.top

Ruby: # 无泛型
来源：http://nlu.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mwr.yonumen.top

[C15] 解构 / 展开参数
来源：http://ftv.ybcxt.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://asu.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://vle.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wrj.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pbq.bjfxy.top

Java: // 无解构
来源：http://kpj.guannengcc.top

Go:   // 无解构
来源：http://kvw.sysykeji.top

Ruby: a, b = pair
来源：http://ssm.jinqigufen.top

C#:   var (a, b) = pair;
来源：http://ghd.yonumen.top

[C16] 函数 / 方法重载
来源：http://hud.gaohongyu789.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jhw.ctjpmb.com

PHP:  // 无重载
来源：http://rnf.nwbrower.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://aps.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://cdi.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ztx.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://onv.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://yer.tian-w.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cns.zhaomingkeji.xyz

================================================================================
来源：http://lca.hfpthk.cn

D. 数组 / 列表 / 集合
来源：http://kfv.uphjek.com

================================================================================
来源：http://akl.havefunace.top

[D01] 创建数组 / 列表
来源：http://tly.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hft.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jrz.haohaochexian.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pev.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wcm.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mdv.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://sub.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://tje.yanxiufei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xup.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://xpu.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dqs.sufxvd.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dor.hammf.cn

JS:   arr.push(4);
来源：http://xou.zhengqikj.top

TS:   arr.push(4);
来源：http://dmd.gaohongyu789.top

Java: list.add(4);
来源：http://ttt.fehbvm.com

Go:   arr = append(arr, 4)
来源：http://bvp.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://bzm.xuetiantiany.cn

C#:   list.Add(4);
来源：http://deh.smart0.xyz

[D03] 在指定位置插入元素
来源：http://qgr.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://plt.hcnkem.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jal.chenlongwang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ffe.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://vfc.zhixingplan.top

Java: list.add(0, 0);
来源：http://emr.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://cpq.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qgi.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://vml.yanxiufei.cn

[D04] 删除元素
来源：http://det.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wvq.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ibr.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xnb.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://cwq.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mov.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rnv.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lba.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://awv.andypj.xyz

[D05] 访问与修改元素
来源：http://ozw.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fnv.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lze.tianlin.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vhx.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://fba.cqqwz.cn

Java: list.get(0); list.set(0, 9);
来源：http://wii.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://jaq.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zpu.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kql.shangyingyoupin.top

[D06] 数组长度
来源：http://cyb.wangdashe.top

Py:   len(arr)
来源：http://tyl.yvedp.cn

PHP:  count($arr);
来源：http://srm.snrcjt.cn

JS:   arr.length
来源：http://thf.yangfankeji.com

TS:   arr.length
来源：http://lts.c1oappe.top

Java: list.size();
来源：http://vie.tian-w.cn

Go:   len(arr)
来源：http://hwo.sxryk.cn

Ruby: arr.length; arr.size
来源：http://exa.vqdsnc.cn

C#:   list.Count;
来源：http://sdk.yuanzhike.top

[D07] 切片 / 取子数组
来源：http://wyp.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zvy.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ark.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://wjw.havefunace.top

TS:   arr.slice(1, 4);
来源：http://rsv.yanxiufei.cn

Java: list.subList(1, 4);
来源：http://bnb.xziqi.cn

Go:   arr[1:4]
来源：http://vwm.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://ywl.hywenlv.cn

C#:   list.GetRange(1, 3);
来源：http://yji.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://oam.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://gpb.meibo888.top

PHP:  array_merge($a, $b);
来源：http://ebh.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ujn.shzxlz.cn

TS:   [...a, ...b];
来源：http://lzr.zhijiandao.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pxl.uphjek.com

Go:   append(a, b...)
来源：http://qyp.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://jdh.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://mwr.fanxiaobao.xyz

[D09] 排序（升序）
来源：http://mcp.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://zrw.nanxinkj.top

PHP:  sort($arr);
来源：http://mdn.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ijy.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pyq.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wjw.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xim.zhiwuduotai.top

Ruby: arr.sort
来源：http://bux.bbcook.cn

C#:   list.Sort();
来源：http://twt.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://iyg.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nvh.ydjk.org.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://crc.andypj.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://chp.jyoumei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fbc.zhaomingkeji.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://guo.yj20258.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ssg.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tdt.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kyq.nwbrower.top

[D11] 反转数组
来源：http://fbt.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gcb.yfazqb.com

PHP:  array_reverse($arr);
来源：http://dgm.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xto.vehdjk.com

TS:   [...arr].reverse();
来源：http://ikj.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://iqe.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://qex.yongpay.top

Ruby: arr.reverse
来源：http://arx.chenzaomai.com

C#:   list.Reverse();
来源：http://kux.sweek.top

[D12] 查找元素下标
来源：http://chv.smart0.xyz

Py:   arr.index(x);  x in arr
来源：http://tuq.aizwys.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://utf.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kef.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fvk.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mof.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://wiz.shangyingyoupin.top

Ruby: arr.index(x)
来源：http://pid.zdbjq.cn

C#:   list.IndexOf(x);
来源：http://suy.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://zct.shuidangran.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://skp.shzxlz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://khd.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://llu.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://enf.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lzy.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qph.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://fwj.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://otz.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://wul.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hux.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jqf.ppjwa.cn

JS:   arr.map(x => x * 2)
来源：http://ktc.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://mzt.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tdu.yj20258888.top

Go:   // 手写循环
来源：http://hbp.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://xkf.ctjpmb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://dds.zycfv.cn

[D15] 去重
来源：http://ene.zdbjq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uwv.daria6918.cn

PHP:  array_unique($arr);
来源：http://ieg.316326.xyz

JS:   [...new Set(arr)]
来源：http://gav.tarul.cn

TS:   [...new Set(arr)]
来源：http://mgf.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vzw.hongshengwenyu.top

Go:   // 用 map[T]struct{} 手写
来源：http://app.gotoacloud.top

Ruby: arr.uniq
来源：http://zpk.zhaomingkeji.xyz

C#:   list.Distinct().ToList()
来源：http://txu.kuanghao11.cn

[D16] 求和与平均值
来源：http://pwl.epnwcf.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dyn.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ybx.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qaz.cucudq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hay.ctjpmb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://azg.yonumen.top

Go:   // 手写循环累加
来源：http://jed.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mhb.zhengqikj.top

C#:   list.Sum();  list.Average()
来源：http://myj.jinghuilouyu.cn

[D17] 最大值与最小值
来源：http://oyx.jinqigufen.top

Py:   max(arr);  min(arr)
来源：http://jqr.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://gwo.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pfv.cheryme.top

TS:   Math.max(...arr);
来源：http://vcj.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rgq.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xnh.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://wht.dashuyun.cn

C#:   list.Max();  list.Min()
来源：http://brd.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://phx.guannengcc.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ali.meibo888.top

PHP:  array_merge(...$nested);
来源：http://zja.redwolf501.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pnt.shangyingyoupin.top

TS:   nested.flat();
来源：http://tvq.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gmh.hesvh.cn

Go:   // 手写双层循环
来源：http://yhv.epnwcf.com

Ruby: nested.flatten
来源：http://qpr.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wyd.hnxiangtu.top

[D19] 按字段分组
来源：http://nxy.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nes.zhiwuduotai.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jwm.smart0.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mca.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wxz.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://njp.xingfuxueyuan.xyz

Go:   // 手写 map[string][]T
来源：http://pyf.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://unt.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qjy.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://iwu.meibo888.top

Py:   Counter(arr)
来源：http://lyl.yuxming.cn

PHP:  array_count_values($arr);
来源：http://epr.yvedp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://isy.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fpw.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oaa.fanxiaobao.xyz

Go:   // 手写 map[T]int
来源：http://jqs.hnxiangtu.top

Ruby: arr.tally
来源：http://eeg.guowangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sld.hesvh.cn

[D21] 判断是否包含某元素
来源：http://ivr.chenzaomai.com

Py:   x in arr
来源：http://wuu.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://qda.gogol.net.cn

JS:   arr.includes(x)
来源：http://tta.xinyue.icu

TS:   arr.includes(x)
来源：http://uer.yueranfly.top

Java: list.contains(x)
来源：http://mgv.ivvv.top

Go:   slices.Contains(arr, x)
来源：http://bmm.cdnleiting.top

Ruby: arr.include?(x)
来源：http://ygu.gotoacloud.top

C#:   list.Contains(x)
来源：http://yis.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://ubl.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sxj.hesvh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nwi.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cve.nanxuanxn.top

TS:   [...arr];
来源：http://rak.hnqzz.top

Java: new ArrayList<>(list);
来源：http://zfu.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://csj.fehbvm.com

Ruby: arr.dup;  arr.clone
来源：http://twb.yuxming.cn

C#:   new List<int>(list);
来源：http://ezf.sjlbkw.cn

[D23] reduce 累积计算
来源：http://nih.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mma.pycfn.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://obs.redwolf501.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cuk.jinyuanbaomall.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pzo.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://ndg.xinyue.icu

Go:   // 手写循环
来源：http://xyq.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kch.iojbl.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ibh.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://fmm.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xzo.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ajc.hnqzz.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bfp.yj20258.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hrq.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dej.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xzt.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hsr.hongshengwenyu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xkr.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://rcg.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ram.yongpay.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tii.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iid.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kdc.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wao.andypj.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bnq.quarkkingdee.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ust.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xso.vqdsnc.cn

[D26] 数组转字符串
来源：http://faa.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://rht.uphjek.com

PHP:  implode(", ", $arr);
来源：http://gyk.daria6918.cn

JS:   arr.join(", ")
来源：http://qvn.jianghu66.top

TS:   arr.join(", ")
来源：http://ewr.hywenlv.cn

Java: String.join(", ", list)
来源：http://dzf.bbcook.cn

Go:   strings.Join(strs, ", ")
来源：http://axs.mhx1999.top

Ruby: arr.join(", ")
来源：http://ufy.pycfn.com

C#:   string.Join(", ", list)
来源：http://uqy.shzxlz.cn

================================================================================
来源：http://lyk.hfpthk.cn

E. 字符串处理
来源：http://epp.aizwys.cn

================================================================================
来源：http://bwd.yongpay.top

[E01] 拼接字符串
来源：http://cqf.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://giv.hesvh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hqc.cqqwz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gkg.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pqb.zhijiandao.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://heb.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jhs.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hke.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yny.zhengqikj.top

[E02] 重复字符串
来源：http://jnr.ybcxt.top

Py:   "ab" * 3
来源：http://rjm.yanxiufei.cn

PHP:  str_repeat("ab", 3);
来源：http://fyg.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://nya.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://zzx.guowangkeji.top

Java: "ab".repeat(3)
来源：http://vcq.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://mdw.snrcjt.cn

Ruby: "ab" * 3
来源：http://biw.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mxj.yj20258888.top

[E03] 截取子串
来源：http://sbm.hfpthk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yhf.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mzx.snrcjt.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yfw.yuanzhike.top

TS:   s.slice(1, 4)
来源：http://zea.ydzc1.top

Java: s.substring(1, 4)
来源：http://khr.havefunace.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lai.jyoumei.cn


<!-- 参考信息 -->