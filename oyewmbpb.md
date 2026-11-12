代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://duv.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iqp.ydzc1.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cmy.fzhhl.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://euc.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://spm.zhoulong.xyz

Ruby: arr = [1, 2, 3]
来源：http://qem.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fnc.jinqigufen.top

[D02] 追加元素到末尾
来源：http://pgg.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://add.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://puq.jlsjyb.cn

JS:   arr.push(4);
来源：http://bjv.shangyingyoupin.top

TS:   arr.push(4);
来源：http://ewo.xuetiantiany.cn

Java: list.add(4);
来源：http://oot.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://ezh.zhijiandao.cn

Ruby: arr << 4; arr.push(5)
来源：http://ubr.tanke756.top

C#:   list.Add(4);
来源：http://yzo.mhx1999.top

[D03] 在指定位置插入元素
来源：http://urz.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://ygb.sysykeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ttg.kuanghao11.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wwc.jqgfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://per.yuxming.cn

Java: list.add(0, 0);
来源：http://mdq.jianghu66.top

Go:   arr = append([]int{0}, arr...)
来源：http://zba.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://obh.tanke756.top

C#:   list.Insert(0, 0);
来源：http://cmx.shanyushiyangkeji.top

[D04] 删除元素
来源：http://cxk.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wue.xziqi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://txg.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ggh.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://crc.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xiv.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ugd.52xcode.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ukg.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bwz.chenlongwang.top

[D05] 访问与修改元素
来源：http://xhu.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sch.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iyp.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sva.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://lxd.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://hzs.wangdashe.top

Go:   arr[0]; arr[0] = 9
来源：http://ezv.fengsongda.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ysi.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mtu.shuidangran.top

[D06] 数组长度
来源：http://xic.zycfv.cn

Py:   len(arr)
来源：http://hrs.cheryme.top

PHP:  count($arr);
来源：http://gzy.zdqjudy.top

JS:   arr.length
来源：http://rog.jlsjyb.cn

TS:   arr.length
来源：http://ill.sysykeji.top

Java: list.size();
来源：http://crh.wangdashe.top

Go:   len(arr)
来源：http://wzz.yanxiufei.cn

Ruby: arr.length; arr.size
来源：http://sow.zhiwuduotai.top

C#:   list.Count;
来源：http://amp.zhoulong.xyz

[D07] 切片 / 取子数组
来源：http://cta.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mbn.ppjwa.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wtq.jinqigfzy.top

JS:   arr.slice(1, 4);
来源：http://wsi.feifeiyinyue.top

TS:   arr.slice(1, 4);
来源：http://odt.mhx1999.top

Java: list.subList(1, 4);
来源：http://amu.tarul.cn

Go:   arr[1:4]
来源：http://zbe.fzhhl.top

Ruby: arr[1, 3]
来源：http://vof.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://qhp.jlsjyb.cn

[D08] 合并两个数组
来源：http://spd.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://bsk.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://gof.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wea.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://eol.shanyushiyangtech.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dqt.yongpay.top

Go:   append(a, b...)
来源：http://jsi.xuanzx.com

Ruby: a + b;  a.concat(b)
来源：http://ufp.ywan-chungtsiang.top

C#:   a.Concat(b).ToList()
来源：http://khm.gotoacloud.top

[D09] 排序（升序）
来源：http://lnm.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://jgq.jianghu66.top

PHP:  sort($arr);
来源：http://lac.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bzc.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bsv.hcnkem.com

Java: Collections.sort(list);  list.sort(null);
来源：http://qfg.zdqjudy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://agx.yj202588.top

Ruby: arr.sort
来源：http://rbh.fanxiaobao.xyz

C#:   list.Sort();
来源：http://eve.hesvh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cuv.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iww.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qyx.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://edf.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mtx.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wcz.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://acv.pycfn.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zpb.cucudq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dhe.hnqzz.top

[D11] 反转数组
来源：http://gtr.ywan-chungtsiang.top

Py:   arr[::-1];  arr.reverse()
来源：http://ima.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://mwz.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cgx.kuanghao11.cn

TS:   [...arr].reverse();
来源：http://mkx.cucudq.cn

Java: Collections.reverse(list);
来源：http://zvt.smart0.xyz

Go:   slices.Reverse(arr)
来源：http://fag.jinqigfzy.top

Ruby: arr.reverse
来源：http://jzc.vehdjk.com

C#:   list.Reverse();
来源：http://ajz.aizwys.cn

[D12] 查找元素下标
来源：http://mqz.sweek.top

Py:   arr.index(x);  x in arr
来源：http://sdl.yuanzhike.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ldt.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vrj.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zfe.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lkd.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://rcu.fanxiaobao.xyz

Ruby: arr.index(x)
来源：http://mde.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://xjh.mhx1999.top

[D13] 过滤（保留满足条件的）
来源：http://xsi.wangdashe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://usk.c1oappe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://moe.sjlbkw.cn

JS:   arr.filter(x => x > 3)
来源：http://pnp.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://ltg.sysykeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://onr.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qlq.kuanghao11.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rkh.nanxinkj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nio.shangyingyoupin.top

[D14] 映射转换（每个元素变形）
来源：http://iud.hongshengwenyu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bna.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uyc.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://ubs.vehdjk.com

TS:   arr.map(x => x * 2)
来源：http://scv.yuxming.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bwe.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://csb.vehdjk.com

Ruby: arr.map { |x| x * 2 }
来源：http://hcv.chenzaomai.com

C#:   list.Select(x => x * 2).ToList()
来源：http://pmo.zhaomingkeji.xyz

[D15] 去重
来源：http://itz.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dgn.shuidangran.top

PHP:  array_unique($arr);
来源：http://ndy.mhx1999.top

JS:   [...new Set(arr)]
来源：http://jno.tanke756.top

TS:   [...new Set(arr)]
来源：http://nsq.jyoumei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fgk.yvedp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zjm.kuanghao11.cn

Ruby: arr.uniq
来源：http://kcr.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://guw.hnqzz.top

[D16] 求和与平均值
来源：http://eaq.ctjpmb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://epb.fanxiaobao.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ost.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://byz.nwbrower.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gkf.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://njr.zycfv.cn

Go:   // 手写循环累加
来源：http://exe.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mjy.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://rph.pycfn.com

[D17] 最大值与最小值
来源：http://cjd.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://fpj.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://mch.guowangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://epm.iojbl.cn

TS:   Math.max(...arr);
来源：http://vlu.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bai.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tyn.uphjek.com

Ruby: arr.max;  arr.min
来源：http://xhy.xuanzx.com

C#:   list.Max();  list.Min()
来源：http://qgy.yanxiufei.cn

[D18] 扁平化嵌套数组
来源：http://dqk.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rdi.ivvv.top

PHP:  array_merge(...$nested);
来源：http://qro.fengsongda.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nux.zhoulong.xyz

TS:   nested.flat();
来源：http://sej.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gyn.dashuyun.cn

Go:   // 手写双层循环
来源：http://qus.hfpthk.cn

Ruby: nested.flatten
来源：http://gfb.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fmp.hammf.cn

[D19] 按字段分组
来源：http://ril.sysykeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zvs.tanke756.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eda.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qjv.chenjidiqi.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://vnl.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ono.xylfe.cn

Go:   // 手写 map[string][]T
来源：http://tyd.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://eqf.yonumen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://grr.ctjpmb.com

[D20] 统计每个元素出现次数
来源：http://mui.ppjwa.cn

Py:   Counter(arr)
来源：http://ybr.meibo888.top

PHP:  array_count_values($arr);
来源：http://eaq.nanxinkj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ugw.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hrf.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vrk.redwolf501.top

Go:   // 手写 map[T]int
来源：http://dre.vehdjk.com

Ruby: arr.tally
来源：http://nan.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rat.cqqwz.cn

[D21] 判断是否包含某元素
来源：http://tmh.zhaomingkeji.xyz

Py:   x in arr
来源：http://xlp.zdqjudy.top

PHP:  in_array($x, $arr, true);
来源：http://nyo.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://wxv.tianlin.xyz

TS:   arr.includes(x)
来源：http://kst.yj20258.top

Java: list.contains(x)
来源：http://tgz.yj20258888.top

Go:   slices.Contains(arr, x)
来源：http://koi.nwbrower.top

Ruby: arr.include?(x)
来源：http://rxd.aibaodan.cn

C#:   list.Contains(x)
来源：http://pgr.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://qth.yj20258.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ofj.shuidangran.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://shy.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sox.ehwqpu.com

TS:   [...arr];
来源：http://kvp.xuanzx.com

Java: new ArrayList<>(list);
来源：http://ekj.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://zeo.meibo888.top

Ruby: arr.dup;  arr.clone
来源：http://bku.sufxvd.cn

C#:   new List<int>(list);
来源：http://bmv.sysykeji.top

[D23] reduce 累积计算
来源：http://htm.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://elk.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hxo.fehbvm.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kfn.sufxvd.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wxz.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hee.jyoumei.cn

Go:   // 手写循环
来源：http://lku.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fkn.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qtk.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://lcb.redwolf501.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lio.zhongyouzk.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kfg.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iao.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xui.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fzm.yj20258.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nai.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uwr.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yim.pycfn.com

[D25] Set 集合去重与交并差
来源：http://hhs.xziqi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nte.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rwj.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fgc.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qnh.xinyue.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://def.kuanghao11.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vnr.hesvh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xar.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ewx.c1oappe.top

[D26] 数组转字符串
来源：http://yzg.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://ohu.316326.xyz

PHP:  implode(", ", $arr);
来源：http://zwt.zdqjudy.top

JS:   arr.join(", ")
来源：http://wzf.ctjpmb.com

TS:   arr.join(", ")
来源：http://rks.dashuyun.cn

Java: String.join(", ", list)
来源：http://xmt.wangshuangyany.cn

Go:   strings.Join(strs, ", ")
来源：http://iyq.yvedp.cn

Ruby: arr.join(", ")
来源：http://psg.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://vlh.yuxming.cn

================================================================================
来源：http://rjg.c1oappe.top

E. 字符串处理
来源：http://ogk.guowangkeji.top

================================================================================
来源：http://kfp.sxryk.cn

[E01] 拼接字符串
来源：http://izv.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pkc.quarkkingdee.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hgz.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ohq.vqdsnc.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://scm.cashguo.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://los.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://llq.pengpengdd.cyou

Ruby: "a" + "b";  ["a", "b"].join
来源：http://icr.shzxlz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bzd.fanxiaobao.xyz

[E02] 重复字符串
来源：http://uef.yangfankeji.com

Py:   "ab" * 3
来源：http://mic.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://ahd.kuanghao11.cn

JS:   "ab".repeat(3)
来源：http://eyg.sweek.top

TS:   "ab".repeat(3)
来源：http://nns.andypj.xyz

Java: "ab".repeat(3)
来源：http://olp.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://lhd.fehbvm.com

Ruby: "ab" * 3
来源：http://jry.zhengqikj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lrl.sjlbkw.cn

[E03] 截取子串
来源：http://ffz.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bbk.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uol.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://keo.fengsongda.top

TS:   s.slice(1, 4)
来源：http://uim.vehdjk.com

Java: s.substring(1, 4)
来源：http://cjz.meibo888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kjr.bbcook.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tet.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://qbo.yj20258.top

[E04] 查找子串位置
来源：http://nyt.gogol.net.cn

Py:   s.find("x");  s.index("x")
来源：http://flh.ydzc1.top

PHP:  strpos($s, "x");
来源：http://zdv.snrcjt.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wam.dashuyun.cn

TS:   s.indexOf("x")
来源：http://hdk.c1oappe.top

Java: s.indexOf("x")
来源：http://siv.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://zlr.gogol.net.cn

Ruby: s.index("x")
来源：http://rki.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://ady.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://vff.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pqf.ydjk.org.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ute.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uqt.zhengqikj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ocg.yj20258888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xzj.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://icy.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://klx.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ykz.svipenyu.cn

[E06] 替换子串
来源：http://mgu.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mix.nwbrower.top

PHP:  str_replace("a", "b", $s);
来源：http://yrn.yuanzhike.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vaj.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://kuf.jyoumei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gko.sufxvd.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://etx.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://odl.yvedp.cn

C#:   s.Replace("a", "b")
来源：http://vdj.nanxinkj.top

[E07] 按分隔符拆分
来源：http://uyj.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rrx.fzhhl.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dnm.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://igw.aibaodan.cn

TS:   s.split(",")
来源：http://znx.nanxinkj.top

Java: s.split(",");  s.split("\\s+")
来源：http://dxf.chenjidiqi.icu

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hps.tanke756.top

Ruby: s.split(",");  s.split
来源：http://ubd.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nsj.redwolf501.top

[E08] 数组按分隔符合并
来源：http://qey.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://pof.birdmap.top


<!-- 参考信息 -->