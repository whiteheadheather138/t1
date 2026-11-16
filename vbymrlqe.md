代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://elj.yj20258.top

[C15] 解构 / 展开参数
来源：http://org.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jqc.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://zfx.ehwqpu.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://awp.nanxuanxn.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bdv.havefunace.top

Java: // 无解构
来源：http://duh.chenzaomai.com

Go:   // 无解构
来源：http://smk.xuetiantiany.cn

Ruby: a, b = pair
来源：http://znc.vehdjk.com

C#:   var (a, b) = pair;
来源：http://djd.yuxming.cn

[C16] 函数 / 方法重载
来源：http://zbi.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bpl.zhengqikj.top

PHP:  // 无重载
来源：http://itv.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qll.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://cmk.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ejr.gogol.net.cn

Go:   // 无重载：用不同函数名
来源：http://yik.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://jib.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kyw.tarul.cn

================================================================================
来源：http://suj.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://esu.cdnleiting.top

================================================================================
来源：http://qcx.bjfxy.top

[D01] 创建数组 / 列表
来源：http://vng.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://anw.sxryk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yev.cqqwz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zmg.guannengcc.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mdm.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zfg.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://ptn.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://tum.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xgr.yj202588.top

[D02] 追加元素到末尾
来源：http://qpw.nwbrower.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ova.hywenlv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ajx.zhongyouzk.top

JS:   arr.push(4);
来源：http://pim.chenzaomai.com

TS:   arr.push(4);
来源：http://ztm.pengpengdd.cyou

Java: list.add(4);
来源：http://jhk.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://cnc.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://yik.guannengcc.top

C#:   list.Add(4);
来源：http://xne.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://ora.aizwys.cn

Py:   arr.insert(0, 0)
来源：http://bek.hysaishi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rov.hammf.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dlx.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://rxw.guowangkeji.top

Java: list.add(0, 0);
来源：http://ifu.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://ymg.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yem.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://acr.epnwcf.com

[D04] 删除元素
来源：http://gnc.hywenlv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uxp.ydjk.org.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ltf.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://imn.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://zkh.wangshuangyany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dkt.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xci.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://diy.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vnt.jqgfzy.top

[D05] 访问与修改元素
来源：http://wco.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wbc.shuidangran.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xir.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kvq.zhijiandao.cn

TS:   arr[0]; arr.at(-1);
来源：http://tgp.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://coj.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://vtx.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://app.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ert.zhaomingkeji.xyz

[D06] 数组长度
来源：http://arp.fktsv.cn

Py:   len(arr)
来源：http://mfx.vehdjk.com

PHP:  count($arr);
来源：http://uqv.vehdjk.com

JS:   arr.length
来源：http://ist.meibo888.top

TS:   arr.length
来源：http://prn.shuidangran.top

Java: list.size();
来源：http://qkk.hammf.cn

Go:   len(arr)
来源：http://ypn.zhoulong.xyz

Ruby: arr.length; arr.size
来源：http://fbb.sjlbkw.cn

C#:   list.Count;
来源：http://czo.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://rsn.hysaishi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jxu.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://bas.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://jfv.vehdjk.com

TS:   arr.slice(1, 4);
来源：http://ceg.andypj.xyz

Java: list.subList(1, 4);
来源：http://gyp.cqqwz.cn

Go:   arr[1:4]
来源：http://rry.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://agl.sweek.top

C#:   list.GetRange(1, 3);
来源：http://dbc.guannengcc.top

[D08] 合并两个数组
来源：http://ejv.daxiang520.top

Py:   a + b;  a.extend(b)
来源：http://gby.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://fvn.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://quv.snrcjt.cn

TS:   [...a, ...b];
来源：http://xpd.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qes.cdnleiting.top

Go:   append(a, b...)
来源：http://rbs.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://lwy.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://enx.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://prl.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://ppe.zhixingplan.top

PHP:  sort($arr);
来源：http://rry.daria6918.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pjz.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uou.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zjf.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://opi.pycfn.com

Ruby: arr.sort
来源：http://bdp.ehwqpu.com

C#:   list.Sort();
来源：http://qcz.tarul.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nxo.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://slu.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cnw.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iui.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://shb.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wnf.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vrp.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://peh.jyoumei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://scn.vehdjk.com

[D11] 反转数组
来源：http://krj.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://caw.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://qyk.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rqe.snrcjt.cn

TS:   [...arr].reverse();
来源：http://olk.nwbrower.top

Java: Collections.reverse(list);
来源：http://hgd.fzhhl.top

Go:   slices.Reverse(arr)
来源：http://dji.jinqigfzy.top

Ruby: arr.reverse
来源：http://obv.fehbvm.com

C#:   list.Reverse();
来源：http://sjp.ivvv.top

[D12] 查找元素下标
来源：http://spb.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://pho.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hyg.hfpthk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pdw.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vqq.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nrr.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://ohw.zhengqikj.top

Ruby: arr.index(x)
来源：http://hig.yangfankeji.com

C#:   list.IndexOf(x);
来源：http://uwt.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://rww.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qqy.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://duh.ydjk.org.cn

JS:   arr.filter(x => x > 3)
来源：http://tpz.yj202588.top

TS:   arr.filter(x => x > 3)
来源：http://ewx.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hvx.cucudq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wft.yueranfly.top

Ruby: arr.select { |x| x > 3 }
来源：http://hgi.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://buu.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://qex.ehwqpu.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lyz.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ouo.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://wyb.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://wml.tianlin.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://ejd.kuanghao11.cn

Go:   // 手写循环
来源：http://rvs.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://fio.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iml.52xcode.cn

[D15] 去重
来源：http://lmo.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tvf.cdnleiting.top

PHP:  array_unique($arr);
来源：http://tsx.xziqi.cn

JS:   [...new Set(arr)]
来源：http://ozq.cucudq.cn

TS:   [...new Set(arr)]
来源：http://jdr.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gjs.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://gtu.gzhubu.top

Ruby: arr.uniq
来源：http://azc.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://nns.xuetiantiany.cn

[D16] 求和与平均值
来源：http://itt.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iqn.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://prq.jqgfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gfp.cdnleiting.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nqq.havefunace.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ztm.jqgufenzy.top

Go:   // 手写循环累加
来源：http://vcp.andypj.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://clv.daxiang520.top

C#:   list.Sum();  list.Average()
来源：http://uzq.nwbrower.top

[D17] 最大值与最小值
来源：http://jwp.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://bsz.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://afx.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://imq.tanke756.top

TS:   Math.max(...arr);
来源：http://sln.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zeu.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cit.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://wqh.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://kxt.birdmap.top

[D18] 扁平化嵌套数组
来源：http://rpr.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://icx.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://vzm.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xjb.yueranfly.top

TS:   nested.flat();
来源：http://yac.nanxuanxn.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://afi.cucudq.cn

Go:   // 手写双层循环
来源：http://jlm.yuanzhike.top

Ruby: nested.flatten
来源：http://viv.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://xnz.jinqigfzy.top

[D19] 按字段分组
来源：http://mos.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aig.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tir.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kvn.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://vdd.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lnb.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://eje.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://otu.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mph.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://ail.nwbrower.top

Py:   Counter(arr)
来源：http://xda.vehdjk.com

PHP:  array_count_values($arr);
来源：http://tro.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://edu.hcnkem.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eph.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vps.havefunace.top

Go:   // 手写 map[T]int
来源：http://fgi.gogol.net.cn

Ruby: arr.tally
来源：http://zgx.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aep.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://ohz.xuetiantiany.cn

Py:   x in arr
来源：http://tjt.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://ryu.snrcjt.cn

JS:   arr.includes(x)
来源：http://jry.kuanghao11.cn

TS:   arr.includes(x)
来源：http://vjd.52xcode.cn

Java: list.contains(x)
来源：http://xvk.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://zba.fzhhl.top

Ruby: arr.include?(x)
来源：http://tfi.hammf.cn

C#:   list.Contains(x)
来源：http://ibc.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://exm.bbcook.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jhw.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kqg.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ark.uphjek.com

TS:   [...arr];
来源：http://bfk.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://sjb.sweek.top

Go:   copied := append([]int(nil), arr...)
来源：http://yva.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://jpg.hfpthk.cn

C#:   new List<int>(list);
来源：http://gqt.hesvh.cn

[D23] reduce 累积计算
来源：http://lgm.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cjb.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vff.zhongyouzk.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://czr.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nig.chenlongwang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rop.hammf.cn

Go:   // 手写循环
来源：http://jvq.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nps.hammf.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fyt.tianlin.xyz

[D24] 字典 / Map 基本操作
来源：http://dsv.daria6918.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pqz.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xjd.jqgufenzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lwh.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bxn.daria6918.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qav.epnwcf.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://abi.jinqigfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xzf.jinqigufen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bxt.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://fsa.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bsk.shzxlz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hhy.gotoacloud.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vbc.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tru.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bnu.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oth.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ran.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rkt.nwbrower.top

[D26] 数组转字符串
来源：http://jwb.zdqjudy.top

Py:   ", ".join(map(str, arr))
来源：http://tfz.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://adb.hcnkem.com

JS:   arr.join(", ")
来源：http://oka.smart0.xyz

TS:   arr.join(", ")
来源：http://ozf.jinqigufen.top

Java: String.join(", ", list)
来源：http://zye.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://kxy.nwbrower.top

Ruby: arr.join(", ")
来源：http://qpv.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://iqp.hfpthk.cn

================================================================================
来源：http://run.hnqzz.top

E. 字符串处理
来源：http://uwv.sxryk.cn

================================================================================
来源：http://pdp.yuxming.cn

[E01] 拼接字符串
来源：http://nkt.cheryme.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wzm.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uht.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://knv.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mso.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vyn.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ymz.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bbp.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xee.chenjidiqi.icu

[E02] 重复字符串
来源：http://qoa.cashguo.top

Py:   "ab" * 3
来源：http://duo.nwbrower.top

PHP:  str_repeat("ab", 3);
来源：http://ias.jqgufenzy.top

JS:   "ab".repeat(3)
来源：http://yos.fktsv.cn

TS:   "ab".repeat(3)
来源：http://crn.chenzaomai.com

Java: "ab".repeat(3)
来源：http://ukp.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://dbf.jianghu66.top

Ruby: "ab" * 3
来源：http://luy.cdnleiting.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qsn.kuanghao11.cn

[E03] 截取子串
来源：http://kfd.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rgs.yongpay.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oxq.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zkh.shanyushiyangtech.top

TS:   s.slice(1, 4)
来源：http://orq.zycfv.cn

Java: s.substring(1, 4)
来源：http://vha.jinyuanbaomall.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aqw.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://omv.gotoacloud.top

C#:   s.Substring(1, 3)
来源：http://kdw.fehbvm.com

[E04] 查找子串位置
来源：http://qbm.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://doi.hcnkem.com

PHP:  strpos($s, "x");
来源：http://kfe.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tqy.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://fzy.iojbl.cn

Java: s.indexOf("x")
来源：http://did.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://goq.jqgfzy.top

Ruby: s.index("x")
来源：http://tzi.zdqjudy.top

C#:   s.IndexOf("x")
来源：http://bij.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://heb.birdmap.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xyu.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nvo.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ewo.hfpthk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oia.svipenyu.cn


<!-- 参考信息 -->