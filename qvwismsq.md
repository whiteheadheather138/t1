代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wsi.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vlh.aizwys.cn

JS:   arr.push(4);
来源：http://xhp.yj20258.top

TS:   arr.push(4);
来源：http://zvk.havefunace.top

Java: list.add(4);
来源：http://uyc.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://uau.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://mpx.cashguo.top

C#:   list.Add(4);
来源：http://hev.fehbvm.com

[D03] 在指定位置插入元素
来源：http://jja.vehdjk.com

Py:   arr.insert(0, 0)
来源：http://bpx.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gxb.yj20258.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kag.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://unl.hesvh.cn

Java: list.add(0, 0);
来源：http://pia.cheryme.top

Go:   arr = append([]int{0}, arr...)
来源：http://ibn.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jtp.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://ihq.ybcxt.top

[D04] 删除元素
来源：http://arr.ydjk.org.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vnu.havefunace.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://njw.gogol.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zjt.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://hke.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nlk.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qfa.hesvh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iex.jiagoushi.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cqm.cqqwz.cn

[D05] 访问与修改元素
来源：http://dws.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qun.gogol.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bzu.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://smp.xuetiantiany.cn

TS:   arr[0]; arr.at(-1);
来源：http://jke.shanyushiyangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://qia.zhoulong.xyz

Go:   arr[0]; arr[0] = 9
来源：http://bbp.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qzn.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kvu.pycfn.com

[D06] 数组长度
来源：http://azd.nanxuanxn.top

Py:   len(arr)
来源：http://kdw.52xcode.cn

PHP:  count($arr);
来源：http://cef.guowangkeji.top

JS:   arr.length
来源：http://yor.iojbl.cn

TS:   arr.length
来源：http://gne.sufxvd.cn

Java: list.size();
来源：http://shy.ydzc1.top

Go:   len(arr)
来源：http://hcb.aizwys.cn

Ruby: arr.length; arr.size
来源：http://rtj.zhixingplan.top

C#:   list.Count;
来源：http://jfd.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://bpq.ydjk.org.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yvr.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://bsw.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://sxm.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://pal.0kj1m.cn

Java: list.subList(1, 4);
来源：http://biy.0kj1m.cn

Go:   arr[1:4]
来源：http://luw.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://pla.vehdjk.com

C#:   list.GetRange(1, 3);
来源：http://cko.jinyuanbaomall.cn

[D08] 合并两个数组
来源：http://ywc.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://xqh.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://rpb.zycfv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ezd.pycfn.com

TS:   [...a, ...b];
来源：http://oxb.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sls.tianlin.xyz

Go:   append(a, b...)
来源：http://ozb.vehdjk.com

Ruby: a + b;  a.concat(b)
来源：http://tkv.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://lha.zhixingplan.top

[D09] 排序（升序）
来源：http://spx.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://ioo.jyoumei.cn

PHP:  sort($arr);
来源：http://fuq.chenlongwang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zac.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xwr.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://fsb.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vrz.dashuyun.cn

Ruby: arr.sort
来源：http://tvg.hcnkem.com

C#:   list.Sort();
来源：http://xkd.sjlbkw.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tmd.sxryk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://own.zhiwuduotai.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://guq.jinqigufen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dky.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pif.yj202588.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qpm.cdnleiting.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://buz.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qnx.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://duh.zhongyouzk.top

[D11] 反转数组
来源：http://nrn.sufxvd.cn

Py:   arr[::-1];  arr.reverse()
来源：http://clu.mhx1999.top

PHP:  array_reverse($arr);
来源：http://lku.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yzr.sxryk.cn

TS:   [...arr].reverse();
来源：http://lom.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://swl.redwolf501.top

Go:   slices.Reverse(arr)
来源：http://rbl.chenjidiqi.icu

Ruby: arr.reverse
来源：http://dqy.xuetiantiany.cn

C#:   list.Reverse();
来源：http://ltw.daxiang520.top

[D12] 查找元素下标
来源：http://mdn.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://vtq.ywan-chungtsiang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://had.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mxu.xinyue.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fjo.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wpq.fehbvm.com

Go:   slices.Index(arr, x)
来源：http://kiv.jiagoushi.top

Ruby: arr.index(x)
来源：http://qck.cheryme.top

C#:   list.IndexOf(x);
来源：http://gdz.quarkkingdee.top

[D13] 过滤（保留满足条件的）
来源：http://kfv.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vnl.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zfv.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://cjh.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://gaz.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vgu.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://daq.bbcook.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gdd.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kov.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://mpm.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bjy.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mgn.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://alq.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://ipg.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://elk.hysaishi.cn

Go:   // 手写循环
来源：http://ink.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://kex.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://nwc.xuetiantiany.cn

[D15] 去重
来源：http://xgg.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hmd.316326.xyz

PHP:  array_unique($arr);
来源：http://wzr.daxiang520.top

JS:   [...new Set(arr)]
来源：http://bkp.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://duc.hfpthk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pcx.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://nee.9152youxi.cn

Ruby: arr.uniq
来源：http://puq.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://pbp.uphjek.com

[D16] 求和与平均值
来源：http://esn.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://upz.bjfxy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://itl.birdmap.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qcs.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cyg.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ufy.ivvv.top

Go:   // 手写循环累加
来源：http://yam.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lag.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://vxc.yj202588.top

[D17] 最大值与最小值
来源：http://ria.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://rtk.zdbjq.cn

PHP:  max($arr);  min($arr);
来源：http://ypo.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xzj.zhaomingkeji.xyz

TS:   Math.max(...arr);
来源：http://rdd.ivvv.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mpq.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rnx.xziqi.cn

Ruby: arr.max;  arr.min
来源：http://bdl.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://tly.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://vzo.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dnl.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://seb.ctjpmb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://whp.sysykeji.top

TS:   nested.flat();
来源：http://hhk.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fny.xuanzx.com

Go:   // 手写双层循环
来源：http://pyu.yj202588.top

Ruby: nested.flatten
来源：http://twr.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vcy.pengpengdd.cyou

[D19] 按字段分组
来源：http://dmt.jqgfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hzt.hnxiangtu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nci.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bnr.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uxt.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xbu.hammf.cn

Go:   // 手写 map[string][]T
来源：http://ell.hysaishi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://scs.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gse.havefunace.top

[D20] 统计每个元素出现次数
来源：http://qew.0kj1m.cn

Py:   Counter(arr)
来源：http://bsj.shangyingyoupin.top

PHP:  array_count_values($arr);
来源：http://igv.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wyw.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://trr.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ggd.nanxinkj.top

Go:   // 手写 map[T]int
来源：http://wiz.redwolf501.top

Ruby: arr.tally
来源：http://hnj.yuxming.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cqo.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://gwl.bbcook.cn

Py:   x in arr
来源：http://mgg.ivvv.top

PHP:  in_array($x, $arr, true);
来源：http://pdq.ctjpmb.com

JS:   arr.includes(x)
来源：http://uje.gzhubu.top

TS:   arr.includes(x)
来源：http://qyj.xuanzx.com

Java: list.contains(x)
来源：http://hhc.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://yyh.meibo888.top

Ruby: arr.include?(x)
来源：http://tcc.xingfuxueyuan.xyz

C#:   list.Contains(x)
来源：http://lni.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://abv.zhixingplan.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ukb.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gsv.nwbrower.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xcd.smart0.xyz

TS:   [...arr];
来源：http://amc.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://tkf.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://phy.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://kkj.hywenlv.cn

C#:   new List<int>(list);
来源：http://wsg.bjfxy.top

[D23] reduce 累积计算
来源：http://iks.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://spt.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://irf.daria6918.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ffz.tarul.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nrh.smart0.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://sff.gaohongyu789.top

Go:   // 手写循环
来源：http://pzq.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bfn.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aca.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://bke.snrcjt.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lpv.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yfy.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zbt.yj20258888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://chi.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cms.vqdsnc.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hsi.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ldq.jinyuanbaomall.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cud.smart0.xyz

[D25] Set 集合去重与交并差
来源：http://xsl.sjlbkw.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gqp.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zgr.andypj.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://chs.cashguo.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://upu.andypj.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ewe.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sdt.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rdi.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jwi.yuxming.cn

[D26] 数组转字符串
来源：http://imf.chenzaomai.com

Py:   ", ".join(map(str, arr))
来源：http://hfz.meibo888.top

PHP:  implode(", ", $arr);
来源：http://dza.yj20258888.top

JS:   arr.join(", ")
来源：http://xig.nanxinkj.top

TS:   arr.join(", ")
来源：http://oox.jlsjyb.cn

Java: String.join(", ", list)
来源：http://rin.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://uph.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://vdt.xuanzx.com

C#:   string.Join(", ", list)
来源：http://zqx.zhoulong.xyz

================================================================================
来源：http://sgi.kuanghao11.cn

E. 字符串处理
来源：http://lpz.kuanghao11.cn

================================================================================
来源：http://iek.mhx1999.top

[E01] 拼接字符串
来源：http://avq.jiagoushi.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hyh.jinghuilouyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sbg.chenlongwang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rlz.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wqd.hesvh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ixl.vqdsnc.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vmq.xylfe.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://scx.jinqigufen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sql.daria6918.cn

[E02] 重复字符串
来源：http://fuz.meibo888.top

Py:   "ab" * 3
来源：http://msv.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://xhc.yueranfly.top

JS:   "ab".repeat(3)
来源：http://lrv.hfpthk.cn

TS:   "ab".repeat(3)
来源：http://ymv.yongpay.top

Java: "ab".repeat(3)
来源：http://aep.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://ioi.jqgfzy.top

Ruby: "ab" * 3
来源：http://dwm.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sez.cucudq.cn

[E03] 截取子串
来源：http://xfu.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ond.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ldt.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ohu.cdnleiting.top

TS:   s.slice(1, 4)
来源：http://cja.316326.xyz

Java: s.substring(1, 4)
来源：http://ppr.aibaodan.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fxv.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://qyr.yonumen.top

C#:   s.Substring(1, 3)
来源：http://uic.zhixingplan.top

[E04] 查找子串位置
来源：http://oiq.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://ekw.yvedp.cn

PHP:  strpos($s, "x");
来源：http://eha.hysaishi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ofq.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://vue.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://daj.hcnkem.com

Go:   strings.Index(s, "x")
来源：http://bee.birdmap.top

Ruby: s.index("x")
来源：http://xqb.zhongyouzk.top

C#:   s.IndexOf("x")
来源：http://tzf.shzxlz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://eyb.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ema.svipenyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ptc.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gvu.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ssn.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yen.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fxy.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://akb.snrcjt.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tsz.shangyingyoupin.top

[E06] 替换子串
来源：http://zlx.zhiwuduotai.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gpj.xingfuxueyuan.xyz

PHP:  str_replace("a", "b", $s);
来源：http://puy.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://knk.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://rqj.tian-w.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rfj.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tny.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kff.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://tcu.ppjwa.cn

[E07] 按分隔符拆分
来源：http://abz.daria6918.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sug.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hjq.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jjr.bbcook.cn

TS:   s.split(",")
来源：http://ciz.zhiwuduotai.top

Java: s.split(",");  s.split("\\s+")
来源：http://kpc.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://viv.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://zmd.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mcs.meibo888.top

[E08] 数组按分隔符合并
来源：http://phc.xuanzx.com

Py:   ",".join(items)
来源：http://sgo.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://hbl.yongpay.top

JS:   items.join(",")
来源：http://nes.cdnleiting.top

TS:   items.join(",")
来源：http://spn.fktsv.cn

Java: String.join(",", items)
来源：http://wbs.xinyue.icu

Go:   strings.Join(items, ",")
来源：http://tlx.hnxiangtu.top

Ruby: items.join(",")
来源：http://sqq.zdbjq.cn

C#:   string.Join(",", items)
来源：http://hrv.haohaochexian.top

[E09] 去除所有空白字符
来源：http://rba.nwbrower.top


<!-- 参考信息 -->