代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hnl.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ngj.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uet.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fpu.redwolf501.top

Java: int add(int a, int b) { return a + b; }
来源：http://vfv.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://ayo.sxryk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hmb.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://sxs.nanxinkj.top

[C14] 泛型函数
来源：http://acw.mhx1999.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zej.yongpay.top

PHP:  // 无泛型
来源：http://pkq.nanxinkj.top

JS:   // 无泛型
来源：http://jwm.jinqigfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nve.jianghu66.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vzh.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nbk.gaohongyu789.top

Ruby: # 无泛型
来源：http://lwj.nanxinkj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sxk.tanke756.top

[C15] 解构 / 展开参数
来源：http://pia.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zpl.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://asq.0kj1m.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dfr.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aee.yuanzhike.top

Java: // 无解构
来源：http://fga.hywenlv.cn

Go:   // 无解构
来源：http://mdm.xuanzx.com

Ruby: a, b = pair
来源：http://ura.xylfe.cn

C#:   var (a, b) = pair;
来源：http://zxl.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://qfl.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rzk.hfpthk.cn

PHP:  // 无重载
来源：http://xto.9152youxi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wah.zycfv.cn

TS:   // 用联合类型或重载签名声明
来源：http://uoq.zhoulong.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://ufi.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://wfg.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://yrm.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://zxu.xziqi.cn

================================================================================
来源：http://qgb.yongpay.top

D. 数组 / 列表 / 集合
来源：http://vpm.hnqzz.top

================================================================================
来源：http://qkw.jinqigfzy.top

[D01] 创建数组 / 列表
来源：http://qkb.zhengqikj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uqr.cqqwz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wcl.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wmw.sysykeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ael.yj20258.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dnu.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://zcl.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://kog.daria6918.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xkj.gaohongyu789.top

[D02] 追加元素到末尾
来源：http://jug.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ghe.ivvv.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qrc.zhengqikj.top

JS:   arr.push(4);
来源：http://vre.ydzc1.top

TS:   arr.push(4);
来源：http://nkj.hywenlv.cn

Java: list.add(4);
来源：http://mks.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://cqx.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://owr.jlsjyb.cn

C#:   list.Add(4);
来源：http://ygy.fzhhl.top

[D03] 在指定位置插入元素
来源：http://eos.zhixingplan.top

Py:   arr.insert(0, 0)
来源：http://haa.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ezs.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sbz.cqqwz.cn

TS:   arr.splice(0, 0, 0);
来源：http://rvk.redwolf501.top

Java: list.add(0, 0);
来源：http://avh.ctjpmb.com

Go:   arr = append([]int{0}, arr...)
来源：http://aog.nwbrower.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hxu.sysykeji.top

C#:   list.Insert(0, 0);
来源：http://ovd.fktsv.cn

[D04] 删除元素
来源：http://gxv.gzhubu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cmu.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qmc.yj20258888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://swj.zhengqikj.top

TS:   arr.splice(0, 1);
来源：http://yts.316326.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nen.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rug.zycfv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://voo.birdmap.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fid.gzhubu.top

[D05] 访问与修改元素
来源：http://lha.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://osh.hcnkem.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xzb.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kaa.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://eld.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://qsl.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://rrq.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rga.jinqigufen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hau.jlsjyb.cn

[D06] 数组长度
来源：http://smd.xinyue.icu

Py:   len(arr)
来源：http://slf.cqqwz.cn

PHP:  count($arr);
来源：http://whq.pengpengdd.cyou

JS:   arr.length
来源：http://faz.c1oappe.top

TS:   arr.length
来源：http://vmn.fehbvm.com

Java: list.size();
来源：http://nyd.vqdsnc.cn

Go:   len(arr)
来源：http://sai.zhijiandao.cn

Ruby: arr.length; arr.size
来源：http://lba.jiagoushi.top

C#:   list.Count;
来源：http://wxv.cashguo.top

[D07] 切片 / 取子数组
来源：http://bzo.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qhn.jinghuilouyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fwp.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://nln.hnxiangtu.top

TS:   arr.slice(1, 4);
来源：http://upp.wangdashe.top

Java: list.subList(1, 4);
来源：http://qjr.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://cjt.yongpay.top

Ruby: arr[1, 3]
来源：http://lxk.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://ehl.nanxinkj.top

[D08] 合并两个数组
来源：http://hib.chenzaomai.com

Py:   a + b;  a.extend(b)
来源：http://vso.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://mzl.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wqv.chenlongwang.top

TS:   [...a, ...b];
来源：http://nok.hcnkem.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://inl.316326.xyz

Go:   append(a, b...)
来源：http://ioi.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://pgi.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://qik.jianghu66.top

[D09] 排序（升序）
来源：http://wqk.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://knj.zhoulong.xyz

PHP:  sort($arr);
来源：http://msl.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dfo.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xhb.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hkf.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vzv.jqgufenzy.top

Ruby: arr.sort
来源：http://tln.zhixingplan.top

C#:   list.Sort();
来源：http://itk.hnqzz.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pgi.shuidangran.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ppc.chenlongwang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lzz.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://imy.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://knj.zhongyouzk.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xxm.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ynw.hesvh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kat.cheryme.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zku.tianlin.xyz

[D11] 反转数组
来源：http://ouw.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://oyu.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://qwu.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zcb.sxryk.cn

TS:   [...arr].reverse();
来源：http://fft.yvedp.cn

Java: Collections.reverse(list);
来源：http://zab.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://abj.zycfv.cn

Ruby: arr.reverse
来源：http://krs.jqgfzy.top

C#:   list.Reverse();
来源：http://tax.hnqzz.top

[D12] 查找元素下标
来源：http://fzu.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://pfy.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://igg.jinghuilouyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vta.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iba.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://dqx.svipenyu.cn

Ruby: arr.index(x)
来源：http://qmu.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://kin.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://hoh.hammf.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://feb.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jgr.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://lpr.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://cbl.nanxuanxn.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uax.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gsi.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://ysd.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://szo.cucudq.cn

[D14] 映射转换（每个元素变形）
来源：http://jdg.yuxming.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rdv.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qjz.yanxiufei.cn

JS:   arr.map(x => x * 2)
来源：http://soo.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://apn.zhoulong.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://gjo.guannengcc.top

Go:   // 手写循环
来源：http://yds.yueranfly.top

Ruby: arr.map { |x| x * 2 }
来源：http://kbv.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pxp.yj20258888.top

[D15] 去重
来源：http://gzj.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jno.svipenyu.cn

PHP:  array_unique($arr);
来源：http://kpj.yonumen.top

JS:   [...new Set(arr)]
来源：http://cru.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://dci.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://egr.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://ghq.hongshengwenyu.top

Ruby: arr.uniq
来源：http://ixs.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://azu.zhixingplan.top

[D16] 求和与平均值
来源：http://ecr.guowangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://avb.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cqx.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hvk.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hsd.fktsv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nxh.chenzaomai.com

Go:   // 手写循环累加
来源：http://fuy.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hdo.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://otm.epnwcf.com

[D17] 最大值与最小值
来源：http://pah.shangyingyoupin.top

Py:   max(arr);  min(arr)
来源：http://qld.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://bgp.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://akh.wangdashe.top

TS:   Math.max(...arr);
来源：http://hcd.jinyuanbaomall.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ssu.hcnkem.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://udq.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://bvb.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://hbx.yuxming.cn

[D18] 扁平化嵌套数组
来源：http://yeh.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mex.wangdashe.top

PHP:  array_merge(...$nested);
来源：http://xgx.zhaomingkeji.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fhx.jinqigfzy.top

TS:   nested.flat();
来源：http://wne.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zgd.nwbrower.top

Go:   // 手写双层循环
来源：http://kzw.ctjpmb.com

Ruby: nested.flatten
来源：http://gwp.sjlbkw.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rgo.nanxinkj.top

[D19] 按字段分组
来源：http://uds.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qal.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://frk.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eee.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ytg.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gif.snrcjt.cn

Go:   // 手写 map[string][]T
来源：http://qwv.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mzd.wangdashe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dxc.sjlbkw.cn

[D20] 统计每个元素出现次数
来源：http://qqk.hesvh.cn

Py:   Counter(arr)
来源：http://jke.yj20258888.top

PHP:  array_count_values($arr);
来源：http://zgq.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ggy.tarul.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://naf.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ktq.dashuyun.cn

Go:   // 手写 map[T]int
来源：http://vgu.fanxiaobao.xyz

Ruby: arr.tally
来源：http://bqo.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xrj.hywenlv.cn

[D21] 判断是否包含某元素
来源：http://wee.zhaomingkeji.xyz

Py:   x in arr
来源：http://uxk.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://ovn.zhongyouzk.top

JS:   arr.includes(x)
来源：http://pbd.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://eya.jianghu66.top

Java: list.contains(x)
来源：http://twc.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://ulw.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://col.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://lns.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://zvf.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xdi.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ujl.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jos.zdqjudy.top

TS:   [...arr];
来源：http://gez.dianchejie.cn

Java: new ArrayList<>(list);
来源：http://vnl.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://gfb.ivvv.top

Ruby: arr.dup;  arr.clone
来源：http://drl.havefunace.top

C#:   new List<int>(list);
来源：http://lou.vehdjk.com

[D23] reduce 累积计算
来源：http://jyi.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ghj.uphjek.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wkn.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ppg.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ykv.nanxinkj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zpv.yuxming.cn

Go:   // 手写循环
来源：http://lpe.jinyuanbaomall.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fkg.wangshuangyany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fxp.tarul.cn

[D24] 字典 / Map 基本操作
来源：http://bnf.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ccb.jinyuanbaomall.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aob.yj20258888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qkx.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cbz.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kjo.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kps.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fha.havefunace.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dgj.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://tbz.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rbu.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://luq.pengpengdd.cyou

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xtn.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zad.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ony.wangshuangyany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://evo.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vhh.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bci.guannengcc.top

[D26] 数组转字符串
来源：http://fiv.mhx1999.top

Py:   ", ".join(map(str, arr))
来源：http://bxi.uphjek.com

PHP:  implode(", ", $arr);
来源：http://fwy.hfpthk.cn

JS:   arr.join(", ")
来源：http://nir.ydzc1.top

TS:   arr.join(", ")
来源：http://aas.yj20258888.top

Java: String.join(", ", list)
来源：http://urh.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://mfh.ppjwa.cn

Ruby: arr.join(", ")
来源：http://ltn.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://kig.ydjk.org.cn

================================================================================
来源：http://rwt.uphjek.com

E. 字符串处理
来源：http://iqd.yueranfly.top

================================================================================
来源：http://pue.xuanzx.com

[E01] 拼接字符串
来源：http://lnu.chenjidiqi.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://afw.xuetiantiany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kgy.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://upr.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bfo.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lio.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lmj.hywenlv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://emu.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nhr.redwolf501.top

[E02] 重复字符串
来源：http://cya.yongpay.top

Py:   "ab" * 3
来源：http://tft.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://std.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://tyn.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://xfr.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://ocn.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://tsr.cdnleiting.top

Ruby: "ab" * 3
来源：http://xff.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dwy.cdnleiting.top

[E03] 截取子串
来源：http://lbe.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wbi.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zui.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://veb.tian-w.cn

TS:   s.slice(1, 4)
来源：http://rxk.birdmap.top

Java: s.substring(1, 4)
来源：http://awq.cheryme.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fxq.aizwys.cn


<!-- 参考信息 -->