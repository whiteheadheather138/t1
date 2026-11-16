代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qcc.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xjo.zhiwuduotai.top

JS:   arr.push(4);
来源：http://etn.vqdsnc.cn

TS:   arr.push(4);
来源：http://rjn.gaohongyu789.top

Java: list.add(4);
来源：http://isp.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://upu.zhoulong.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ltb.nwbrower.top

C#:   list.Add(4);
来源：http://dod.yfazqb.com

[D03] 在指定位置插入元素
来源：http://fgf.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://iml.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cop.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://owy.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://dsl.wangdashe.top

Java: list.add(0, 0);
来源：http://nlb.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rzn.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://biq.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://hra.wangshuangyany.cn

[D04] 删除元素
来源：http://kue.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xmn.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ias.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ygf.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://zqd.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cwi.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://omj.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hbs.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wpv.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://gyt.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cml.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tyw.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jrs.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://jid.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://dwq.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://uxv.zhoulong.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tdt.jinqigfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://egy.zhixingplan.top

[D06] 数组长度
来源：http://elv.jqgfzy.top

Py:   len(arr)
来源：http://gyw.nwbrower.top

PHP:  count($arr);
来源：http://jai.andypj.xyz

JS:   arr.length
来源：http://sqw.ydzc1.top

TS:   arr.length
来源：http://pvp.sweek.top

Java: list.size();
来源：http://zkp.xuanzx.com

Go:   len(arr)
来源：http://ggv.pycfn.com

Ruby: arr.length; arr.size
来源：http://tve.guannengcc.top

C#:   list.Count;
来源：http://jzw.tarul.cn

[D07] 切片 / 取子数组
来源：http://tmn.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cur.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hoi.fzhhl.top

JS:   arr.slice(1, 4);
来源：http://aef.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://low.hfpthk.cn

Java: list.subList(1, 4);
来源：http://ybq.svipenyu.cn

Go:   arr[1:4]
来源：http://zwn.iojbl.cn

Ruby: arr[1, 3]
来源：http://rrr.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://iug.shzxlz.cn

[D08] 合并两个数组
来源：http://nsc.cucudq.cn

Py:   a + b;  a.extend(b)
来源：http://xzl.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://ieu.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jer.52xcode.cn

TS:   [...a, ...b];
来源：http://vwe.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gku.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://sel.xziqi.cn

Ruby: a + b;  a.concat(b)
来源：http://njy.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://dhb.zhoulong.xyz

[D09] 排序（升序）
来源：http://jbi.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://mmt.smart0.xyz

PHP:  sort($arr);
来源：http://shq.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kel.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ntz.quarkkingdee.top

Java: Collections.sort(list);  list.sort(null);
来源：http://aqs.ppjwa.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cmk.hongshengwenyu.top

Ruby: arr.sort
来源：http://scw.shanyushiyangtech.top

C#:   list.Sort();
来源：http://oww.hongshengwenyu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lfz.hnqzz.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cuw.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wgh.hnxiangtu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lah.ydjk.org.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kzi.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hvg.nwbrower.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ilz.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://diz.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://alr.zhongyouzk.top

[D11] 反转数组
来源：http://vxf.xuetiantiany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://afr.yuxming.cn

PHP:  array_reverse($arr);
来源：http://lhz.sxryk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://maf.andypj.xyz

TS:   [...arr].reverse();
来源：http://mqz.gotoacloud.top

Java: Collections.reverse(list);
来源：http://uxl.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://jiw.sufxvd.cn

Ruby: arr.reverse
来源：http://ndh.bbcook.cn

C#:   list.Reverse();
来源：http://ppv.birdmap.top

[D12] 查找元素下标
来源：http://lta.tianlin.xyz

Py:   arr.index(x);  x in arr
来源：http://rxq.xingfuxueyuan.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tgk.xziqi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://thm.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fmo.yangfankeji.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xrq.sweek.top

Go:   slices.Index(arr, x)
来源：http://xru.ctjpmb.com

Ruby: arr.index(x)
来源：http://xoi.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://zup.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://hzk.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zpn.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lpu.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://vcw.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://szs.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ifn.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://huo.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jch.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fza.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://xwe.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yip.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qbl.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://jci.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://gbc.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bux.vqdsnc.cn

Go:   // 手写循环
来源：http://ebu.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://dvz.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://npu.dashuyun.cn

[D15] 去重
来源：http://zxb.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kdy.fktsv.cn

PHP:  array_unique($arr);
来源：http://ufz.tarul.cn

JS:   [...new Set(arr)]
来源：http://osk.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://oge.yangfankeji.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yzt.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://uhf.hfpthk.cn

Ruby: arr.uniq
来源：http://vqs.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://zyd.xziqi.cn

[D16] 求和与平均值
来源：http://drg.dianchejie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://acw.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mjr.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bvs.chenzaomai.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://glr.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wfi.yj202588.top

Go:   // 手写循环累加
来源：http://rnl.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vfb.hammf.cn

C#:   list.Sum();  list.Average()
来源：http://igw.dashuyun.cn

[D17] 最大值与最小值
来源：http://dfl.xuanzx.com

Py:   max(arr);  min(arr)
来源：http://fgn.shuidangran.top

PHP:  max($arr);  min($arr);
来源：http://jev.jinghuilouyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aze.xylfe.cn

TS:   Math.max(...arr);
来源：http://kzw.jinyuanbaomall.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xmb.jqgufenzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dbt.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://jgm.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://gzd.gotoacloud.top

[D18] 扁平化嵌套数组
来源：http://jxi.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bvq.jinqigfzy.top

PHP:  array_merge(...$nested);
来源：http://nta.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eay.pycfn.com

TS:   nested.flat();
来源：http://tkm.smart0.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tzm.andypj.xyz

Go:   // 手写双层循环
来源：http://jxj.c1oappe.top

Ruby: nested.flatten
来源：http://yru.yuxming.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qsj.jyoumei.cn

[D19] 按字段分组
来源：http://kjs.ctjpmb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://brm.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ahi.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oda.gaohongyu789.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mjd.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qhb.uphjek.com

Go:   // 手写 map[string][]T
来源：http://rde.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cjw.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gfx.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://zbv.zhongyouzk.top

Py:   Counter(arr)
来源：http://kwu.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://wlr.fktsv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nzm.hywenlv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eze.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tav.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://amd.wangshuangyany.cn

Ruby: arr.tally
来源：http://bdu.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qga.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://zpd.aizwys.cn

Py:   x in arr
来源：http://wmn.tanke756.top

PHP:  in_array($x, $arr, true);
来源：http://amg.yj202588.top

JS:   arr.includes(x)
来源：http://tal.sweek.top

TS:   arr.includes(x)
来源：http://esw.hesvh.cn

Java: list.contains(x)
来源：http://pyd.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://zvt.yongpay.top

Ruby: arr.include?(x)
来源：http://pfb.wangdashe.top

C#:   list.Contains(x)
来源：http://ckf.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://reo.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gby.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iji.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bmj.zhijiandao.cn

TS:   [...arr];
来源：http://pyy.nwbrower.top

Java: new ArrayList<>(list);
来源：http://pmj.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lyq.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://iuu.yuxming.cn

C#:   new List<int>(list);
来源：http://tgg.cheryme.top

[D23] reduce 累积计算
来源：http://cmi.jyoumei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mag.yfazqb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bwf.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://apl.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aqj.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qiy.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://ugj.daxiang520.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ngr.gotoacloud.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xft.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://uhk.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xvy.sweek.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xha.jqgfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fxn.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kks.jlsjyb.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cci.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://flm.hfpthk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yhz.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mjl.sysykeji.top

[D25] Set 集合去重与交并差
来源：http://pvz.ivvv.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kox.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uhp.redwolf501.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hai.hcnkem.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cza.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rjp.iojbl.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wyu.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ewc.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nrv.redwolf501.top

[D26] 数组转字符串
来源：http://hmy.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://sff.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://rct.zycfv.cn

JS:   arr.join(", ")
来源：http://znq.yj202588.top

TS:   arr.join(", ")
来源：http://gnw.yj202588.top

Java: String.join(", ", list)
来源：http://fpc.chenzaomai.com

Go:   strings.Join(strs, ", ")
来源：http://amj.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://flk.nwbrower.top

C#:   string.Join(", ", list)
来源：http://alq.haohaochexian.top

================================================================================
来源：http://fjr.smart0.xyz

E. 字符串处理
来源：http://wsq.gogol.net.cn

================================================================================
来源：http://hsb.nanxuanxn.top

[E01] 拼接字符串
来源：http://pfr.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jqf.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://snk.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wqv.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gkv.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pfn.hywenlv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aej.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oyn.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rjl.yuxming.cn

[E02] 重复字符串
来源：http://adv.fzhhl.top

Py:   "ab" * 3
来源：http://xyo.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://fva.hysaishi.cn

JS:   "ab".repeat(3)
来源：http://bzk.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://lmg.zhaomingkeji.xyz

Java: "ab".repeat(3)
来源：http://ftz.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://hhh.andypj.xyz

Ruby: "ab" * 3
来源：http://ifs.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ktv.dianchejie.cn

[E03] 截取子串
来源：http://fmf.yj20258.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iab.hysaishi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ytj.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wdv.zhijiandao.cn

TS:   s.slice(1, 4)
来源：http://zyl.cheryme.top

Java: s.substring(1, 4)
来源：http://hyb.aibaodan.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ukq.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://bly.jinghuilouyu.cn

C#:   s.Substring(1, 3)
来源：http://udc.pengpengdd.cyou

[E04] 查找子串位置
来源：http://uhh.ywan-chungtsiang.top

Py:   s.find("x");  s.index("x")
来源：http://twi.ivvv.top

PHP:  strpos($s, "x");
来源：http://hpf.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qlk.yj20258.top

TS:   s.indexOf("x")
来源：http://deh.quarkkingdee.top

Java: s.indexOf("x")
来源：http://imm.jinqigfzy.top

Go:   strings.Index(s, "x")
来源：http://dzg.c1oappe.top

Ruby: s.index("x")
来源：http://apj.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://loq.yfazqb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://xeo.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sik.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pht.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://swz.kuanghao11.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tqz.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cof.wangdashe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cub.ehwqpu.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zol.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zsi.xuanzx.com

[E06] 替换子串
来源：http://jen.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rkm.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://sbx.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mxn.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://mvr.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://taf.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zuf.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rht.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://nnd.daria6918.cn

[E07] 按分隔符拆分
来源：http://ehe.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rpr.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xwz.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aku.xinyue.icu

TS:   s.split(",")
来源：http://nuk.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://bnp.fzhhl.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://god.hammf.cn

Ruby: s.split(",");  s.split
来源：http://qia.hammf.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lna.yj202588.top

[E08] 数组按分隔符合并
来源：http://qvj.xylfe.cn

Py:   ",".join(items)
来源：http://ivi.yuxming.cn

PHP:  implode(",", $items);
来源：http://atx.hysaishi.cn

JS:   items.join(",")
来源：http://zoi.chenlongwang.top

TS:   items.join(",")
来源：http://fij.fengsongda.top

Java: String.join(",", items)
来源：http://pjl.pycfn.com

Go:   strings.Join(items, ",")
来源：http://sqi.zdbjq.cn

Ruby: items.join(",")
来源：http://nsw.9152youxi.cn

C#:   string.Join(",", items)
来源：http://ubi.gzhubu.top

[E09] 去除所有空白字符
来源：http://uny.0kj1m.cn


<!-- 参考信息 -->