代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://vnd.ctjpmb.com

Java: list.add(0, 0);
来源：http://gdo.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://blx.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xfj.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://lqt.tian-w.cn

[D04] 删除元素
来源：http://npj.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://amg.sufxvd.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gik.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iuj.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://oht.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mwf.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zky.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lgn.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://luk.zhixingplan.top

[D05] 访问与修改元素
来源：http://hba.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://use.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mxf.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gaw.guannengcc.top

TS:   arr[0]; arr.at(-1);
来源：http://ynb.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://pap.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://aqi.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sxp.chenjidiqi.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fgt.bbcook.cn

[D06] 数组长度
来源：http://wbp.zhiwuduotai.top

Py:   len(arr)
来源：http://ata.yanxiufei.cn

PHP:  count($arr);
来源：http://zct.gaohongyu789.top

JS:   arr.length
来源：http://qdx.hongshengwenyu.top

TS:   arr.length
来源：http://oqy.zhiwuduotai.top

Java: list.size();
来源：http://orx.daxiang520.top

Go:   len(arr)
来源：http://wdr.fzhhl.top

Ruby: arr.length; arr.size
来源：http://zyt.bjfxy.top

C#:   list.Count;
来源：http://qkj.birdmap.top

[D07] 切片 / 取子数组
来源：http://jvj.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vpo.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://gtu.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://cow.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://cxc.pycfn.com

Java: list.subList(1, 4);
来源：http://fng.daria6918.cn

Go:   arr[1:4]
来源：http://rdl.uphjek.com

Ruby: arr[1, 3]
来源：http://ykf.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://toh.xinyue.icu

[D08] 合并两个数组
来源：http://kxe.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://yyp.shzxlz.cn

PHP:  array_merge($a, $b);
来源：http://ftk.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yfw.nanxuanxn.top

TS:   [...a, ...b];
来源：http://jyj.epnwcf.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yry.nanxinkj.top

Go:   append(a, b...)
来源：http://qeq.vehdjk.com

Ruby: a + b;  a.concat(b)
来源：http://wcd.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://fff.cheryme.top

[D09] 排序（升序）
来源：http://rah.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://wza.c1oappe.top

PHP:  sort($arr);
来源：http://ddp.jianghu66.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://onc.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nul.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cbf.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dha.cqqwz.cn

Ruby: arr.sort
来源：http://xyj.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://jcj.ivvv.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zqw.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qlh.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fay.yj20258.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zys.ctjpmb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gsk.ybcxt.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vrd.316326.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qhq.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oeo.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://chq.hongshengwenyu.top

[D11] 反转数组
来源：http://urb.mhx1999.top

Py:   arr[::-1];  arr.reverse()
来源：http://wia.sxryk.cn

PHP:  array_reverse($arr);
来源：http://vat.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pmk.fktsv.cn

TS:   [...arr].reverse();
来源：http://ojw.jqgfzy.top

Java: Collections.reverse(list);
来源：http://jdv.ywan-chungtsiang.top

Go:   slices.Reverse(arr)
来源：http://jiw.hfpthk.cn

Ruby: arr.reverse
来源：http://sod.zhongyouzk.top

C#:   list.Reverse();
来源：http://wwo.yvedp.cn

[D12] 查找元素下标
来源：http://ivm.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://iem.yangfankeji.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mtu.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://swr.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hdf.dianchejie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vgd.cheryme.top

Go:   slices.Index(arr, x)
来源：http://itx.jyoumei.cn

Ruby: arr.index(x)
来源：http://zrh.zhixingplan.top

C#:   list.IndexOf(x);
来源：http://bbm.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://owi.xziqi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pkz.mhx1999.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jdt.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://uzl.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://fyx.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tfz.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iiw.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://acg.shanyushiyangtech.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zqh.aibaodan.cn

[D14] 映射转换（每个元素变形）
来源：http://fwm.epnwcf.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eix.ydjk.org.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dtq.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://iwu.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://wrz.sysykeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qlg.guowangkeji.top

Go:   // 手写循环
来源：http://adu.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://lgm.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ztr.pengpengdd.cyou

[D15] 去重
来源：http://aci.yuanzhike.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://twb.pycfn.com

PHP:  array_unique($arr);
来源：http://imi.ybcxt.top

JS:   [...new Set(arr)]
来源：http://aun.meibo888.top

TS:   [...new Set(arr)]
来源：http://uav.pycfn.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xhl.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://jrp.xziqi.cn

Ruby: arr.uniq
来源：http://gwq.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://uhj.ydzc1.top

[D16] 求和与平均值
来源：http://npv.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zvk.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pra.0kj1m.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kum.jinqigufen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dul.shzxlz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sum.xuetiantiany.cn

Go:   // 手写循环累加
来源：http://ibr.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mkj.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://hwh.cdnleiting.top

[D17] 最大值与最小值
来源：http://vak.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://toe.jinyuanbaomall.cn

PHP:  max($arr);  min($arr);
来源：http://moh.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oyl.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://boi.meibo888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fav.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zug.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://bzr.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://xiu.nanxuanxn.top

[D18] 扁平化嵌套数组
来源：http://too.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xzx.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://eio.shzxlz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qbm.yangfankeji.com

TS:   nested.flat();
来源：http://mzz.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eed.sysykeji.top

Go:   // 手写双层循环
来源：http://cka.yongpay.top

Ruby: nested.flatten
来源：http://kqx.guowangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qnl.zdqjudy.top

[D19] 按字段分组
来源：http://iwu.yanxiufei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zac.c1oappe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ueo.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iov.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cnw.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ygi.snrcjt.cn

Go:   // 手写 map[string][]T
来源：http://pxj.ydjk.org.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://snn.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jgr.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://hpe.hfpthk.cn

Py:   Counter(arr)
来源：http://prw.sxryk.cn

PHP:  array_count_values($arr);
来源：http://kwm.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zgg.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hcq.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jyn.feifeiyinyue.top

Go:   // 手写 map[T]int
来源：http://gkj.dianchejie.cn

Ruby: arr.tally
来源：http://rdg.sjlbkw.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://axg.yj202588.top

[D21] 判断是否包含某元素
来源：http://jhx.smart0.xyz

Py:   x in arr
来源：http://wlj.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://otj.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://gay.yuxming.cn

TS:   arr.includes(x)
来源：http://joh.sweek.top

Java: list.contains(x)
来源：http://cxv.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://gxm.hnqzz.top

Ruby: arr.include?(x)
来源：http://kws.jqgfzy.top

C#:   list.Contains(x)
来源：http://vxm.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://bsm.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yuk.hnqzz.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dgp.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qot.fanxiaobao.xyz

TS:   [...arr];
来源：http://akf.wangshuangyany.cn

Java: new ArrayList<>(list);
来源：http://jhq.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ngv.yj20258.top

Ruby: arr.dup;  arr.clone
来源：http://zkd.nwbrower.top

C#:   new List<int>(list);
来源：http://zda.yj20258888.top

[D23] reduce 累积计算
来源：http://fub.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kaa.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ufb.jinghuilouyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://job.aibaodan.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nom.hnxiangtu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rmq.gaohongyu789.top

Go:   // 手写循环
来源：http://gnb.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cwr.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gug.zhengqikj.top

[D24] 字典 / Map 基本操作
来源：http://vuq.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yqb.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://koj.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fyp.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qdp.cucudq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://enh.yj20258.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sng.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qcc.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qsx.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://wub.ydjk.org.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cuw.yfazqb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rna.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ehi.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ppd.daxiang520.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://erb.jianghu66.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zha.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://udv.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vak.sufxvd.cn

[D26] 数组转字符串
来源：http://iej.ywan-chungtsiang.top

Py:   ", ".join(map(str, arr))
来源：http://ubn.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://kxy.andypj.xyz

JS:   arr.join(", ")
来源：http://ver.hywenlv.cn

TS:   arr.join(", ")
来源：http://gjd.fanxiaobao.xyz

Java: String.join(", ", list)
来源：http://tsi.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://nhr.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://nxz.yj20258.top

C#:   string.Join(", ", list)
来源：http://zoj.zhengqikj.top

================================================================================
来源：http://egj.kuanghao11.cn

E. 字符串处理
来源：http://hzz.hnxiangtu.top

================================================================================
来源：http://kmc.chenjidiqi.icu

[E01] 拼接字符串
来源：http://hwc.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cti.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iwj.jinyuanbaomall.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://htw.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jds.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eah.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oea.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bvn.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vhi.sjlbkw.cn

[E02] 重复字符串
来源：http://kha.chenzaomai.com

Py:   "ab" * 3
来源：http://kho.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://csx.cashguo.top

JS:   "ab".repeat(3)
来源：http://dzn.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://ynh.xinyue.icu

Java: "ab".repeat(3)
来源：http://flp.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://bsv.birdmap.top

Ruby: "ab" * 3
来源：http://sfd.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sfj.redwolf501.top

[E03] 截取子串
来源：http://rov.fengsongda.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wcg.hesvh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nqc.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zfy.andypj.xyz

TS:   s.slice(1, 4)
来源：http://gnz.cheryme.top

Java: s.substring(1, 4)
来源：http://kyl.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cda.aibaodan.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wep.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://gqn.shuidangran.top

[E04] 查找子串位置
来源：http://bts.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://gjj.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://ggd.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dbm.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://bbx.yuanzhike.top

Java: s.indexOf("x")
来源：http://prk.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://xhx.yfazqb.com

Ruby: s.index("x")
来源：http://cpp.jqgfzy.top

C#:   s.IndexOf("x")
来源：http://eku.mhx1999.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gec.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://avn.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://utz.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zcg.guowangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://adj.jiagoushi.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fod.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lcd.0kj1m.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cqg.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://azf.zhongyouzk.top

[E06] 替换子串
来源：http://bcr.zycfv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hqw.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://ahf.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hqe.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://skr.fehbvm.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gqm.cqqwz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pfa.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pcs.tianlin.xyz

C#:   s.Replace("a", "b")
来源：http://nje.iojbl.cn

[E07] 按分隔符拆分
来源：http://pye.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yss.snrcjt.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jjy.hywenlv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rxp.smart0.xyz

TS:   s.split(",")
来源：http://icm.9152youxi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://imu.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gut.birdmap.top

Ruby: s.split(",");  s.split
来源：http://mms.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tyn.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://njk.ivvv.top

Py:   ",".join(items)
来源：http://dhp.mhx1999.top

PHP:  implode(",", $items);
来源：http://rdb.xziqi.cn

JS:   items.join(",")
来源：http://iar.fehbvm.com

TS:   items.join(",")
来源：http://jwh.dashuyun.cn

Java: String.join(",", items)
来源：http://ykw.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://kuv.hcnkem.com

Ruby: items.join(",")
来源：http://ibd.yuxming.cn

C#:   string.Join(",", items)
来源：http://hak.yj20258888.top

[E09] 去除所有空白字符
来源：http://fry.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bry.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dzm.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://vkv.daxiang520.top

TS:   s.replace(/\s+/g, "")
来源：http://jfk.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://dld.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dxv.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://mvb.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gvn.feifeiyinyue.top

[E10] 左侧补零 / 定长填充
来源：http://miw.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kgg.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ohy.daxiang520.top

JS:   "7".padStart(3, "0")
来源：http://mbk.bjfxy.top


<!-- 参考信息 -->