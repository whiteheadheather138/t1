代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://err.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jbf.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kcf.zhengqikj.top

[D06] 数组长度
来源：http://awq.pycfn.com

Py:   len(arr)
来源：http://wiq.yj202588.top

PHP:  count($arr);
来源：http://gqm.c1oappe.top

JS:   arr.length
来源：http://glx.nanxuanxn.top

TS:   arr.length
来源：http://bqg.hesvh.cn

Java: list.size();
来源：http://pby.zdbjq.cn

Go:   len(arr)
来源：http://xcp.tanke756.top

Ruby: arr.length; arr.size
来源：http://qxl.jlsjyb.cn

C#:   list.Count;
来源：http://arx.hnxiangtu.top

[D07] 切片 / 取子数组
来源：http://uim.zhixingplan.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nby.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lda.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://nsd.zhiwuduotai.top

TS:   arr.slice(1, 4);
来源：http://vof.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://ged.zycfv.cn

Go:   arr[1:4]
来源：http://glc.jinqigufen.top

Ruby: arr[1, 3]
来源：http://zuo.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://she.jinqigfzy.top

[D08] 合并两个数组
来源：http://kxl.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://duz.nanxuanxn.top

PHP:  array_merge($a, $b);
来源：http://bdn.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cjn.sufxvd.cn

TS:   [...a, ...b];
来源：http://kfg.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lea.nwbrower.top

Go:   append(a, b...)
来源：http://dec.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://rfi.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://mfj.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://xfl.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://kur.hongshengwenyu.top

PHP:  sort($arr);
来源：http://gco.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rmk.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lrr.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://pxc.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gho.c1oappe.top

Ruby: arr.sort
来源：http://flk.bbcook.cn

C#:   list.Sort();
来源：http://aog.yanxiufei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lhu.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bor.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mwx.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bpv.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eer.uphjek.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ysb.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hbu.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kgq.iojbl.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zln.zhijiandao.cn

[D11] 反转数组
来源：http://smb.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fbu.yj202588.top

PHP:  array_reverse($arr);
来源：http://wxd.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ued.wangdashe.top

TS:   [...arr].reverse();
来源：http://hka.dashuyun.cn

Java: Collections.reverse(list);
来源：http://pdf.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://jnl.yongpay.top

Ruby: arr.reverse
来源：http://zja.tanke756.top

C#:   list.Reverse();
来源：http://jqp.fzhhl.top

[D12] 查找元素下标
来源：http://myi.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://lap.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rxt.ydzc1.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jnw.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cnh.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kjn.tarul.cn

Go:   slices.Index(arr, x)
来源：http://rqq.svipenyu.cn

Ruby: arr.index(x)
来源：http://gzp.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://rwp.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://shi.shanyushiyangtech.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xlk.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://crn.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://gaj.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://clw.redwolf501.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pba.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zhu.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pmv.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pvy.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://fyb.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mfh.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dly.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://nsa.zhoulong.xyz

TS:   arr.map(x => x * 2)
来源：http://tsv.zhiwuduotai.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://piq.guannengcc.top

Go:   // 手写循环
来源：http://nyc.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iuw.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sfv.dianchejie.cn

[D15] 去重
来源：http://xbt.snrcjt.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jfx.bbcook.cn

PHP:  array_unique($arr);
来源：http://ypm.xinyue.icu

JS:   [...new Set(arr)]
来源：http://fgh.yonumen.top

TS:   [...new Set(arr)]
来源：http://zhz.sysykeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rry.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pmn.jqgufenzy.top

Ruby: arr.uniq
来源：http://gca.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://jse.chenjidiqi.icu

[D16] 求和与平均值
来源：http://jre.fehbvm.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qtd.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xhw.zhoulong.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lcb.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jfm.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dgw.zdqjudy.top

Go:   // 手写循环累加
来源：http://itt.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ibq.sweek.top

C#:   list.Sum();  list.Average()
来源：http://scy.zhongyouzk.top

[D17] 最大值与最小值
来源：http://jne.zycfv.cn

Py:   max(arr);  min(arr)
来源：http://uhd.vqdsnc.cn

PHP:  max($arr);  min($arr);
来源：http://tns.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mrz.tanke756.top

TS:   Math.max(...arr);
来源：http://nfd.ivvv.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dro.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pyp.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://nbt.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://ezw.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://unk.hfpthk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jeo.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://cqg.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ibt.feifeiyinyue.top

TS:   nested.flat();
来源：http://asj.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tja.pycfn.com

Go:   // 手写双层循环
来源：http://nxh.andypj.xyz

Ruby: nested.flatten
来源：http://mvv.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sgl.xziqi.cn

[D19] 按字段分组
来源：http://czn.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ntg.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rup.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://orn.bbcook.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wib.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dha.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://cpq.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zwa.gotoacloud.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hnj.bbcook.cn

[D20] 统计每个元素出现次数
来源：http://zmm.shanyushiyangkeji.top

Py:   Counter(arr)
来源：http://ozv.vehdjk.com

PHP:  array_count_values($arr);
来源：http://fcm.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ijq.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://abd.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bgd.0kj1m.cn

Go:   // 手写 map[T]int
来源：http://mka.sjlbkw.cn

Ruby: arr.tally
来源：http://ofd.yj20258.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://txz.fengsongda.top

[D21] 判断是否包含某元素
来源：http://umg.snrcjt.cn

Py:   x in arr
来源：http://zqe.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://xkr.ywan-chungtsiang.top

JS:   arr.includes(x)
来源：http://xzy.fehbvm.com

TS:   arr.includes(x)
来源：http://ash.gzhubu.top

Java: list.contains(x)
来源：http://lmc.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://nop.fzhhl.top

Ruby: arr.include?(x)
来源：http://azh.tian-w.cn

C#:   list.Contains(x)
来源：http://hwq.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://dts.zycfv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jjk.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yjx.ydjk.org.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://foh.jinqigfzy.top

TS:   [...arr];
来源：http://rrg.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://gsn.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://edl.guannengcc.top

Ruby: arr.dup;  arr.clone
来源：http://swt.aizwys.cn

C#:   new List<int>(list);
来源：http://cwv.cheryme.top

[D23] reduce 累积计算
来源：http://faf.chenzaomai.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ccb.jyoumei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hab.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yco.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nkd.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bbu.hammf.cn

Go:   // 手写循环
来源：http://pgq.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lbn.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://svn.c1oappe.top

[D24] 字典 / Map 基本操作
来源：http://mns.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://maj.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jnk.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iqs.ivvv.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ypw.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lmt.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://owl.zhixingplan.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tnp.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zie.svipenyu.cn

[D25] Set 集合去重与交并差
来源：http://ykd.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sxh.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blm.fanxiaobao.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sky.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://anm.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tnv.zhoulong.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pml.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kbl.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rvo.hysaishi.cn

[D26] 数组转字符串
来源：http://efz.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://adm.guannengcc.top

PHP:  implode(", ", $arr);
来源：http://qxt.fehbvm.com

JS:   arr.join(", ")
来源：http://ygu.tanke756.top

TS:   arr.join(", ")
来源：http://oik.yongpay.top

Java: String.join(", ", list)
来源：http://gvi.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://ieh.zhengqikj.top

Ruby: arr.join(", ")
来源：http://wkm.sweek.top

C#:   string.Join(", ", list)
来源：http://czw.gaohongyu789.top

================================================================================
来源：http://akk.yueranfly.top

E. 字符串处理
来源：http://rat.xingfuxueyuan.xyz

================================================================================
来源：http://bsz.hammf.cn

[E01] 拼接字符串
来源：http://vqo.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hsk.tarul.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ava.cucudq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qxc.9152youxi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zrl.yj20258.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pff.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://csb.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pds.zhijiandao.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pbg.dianchejie.cn

[E02] 重复字符串
来源：http://irp.mhx1999.top

Py:   "ab" * 3
来源：http://mde.andypj.xyz

PHP:  str_repeat("ab", 3);
来源：http://ffx.chenjidiqi.icu

JS:   "ab".repeat(3)
来源：http://rjs.ppjwa.cn

TS:   "ab".repeat(3)
来源：http://xpe.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://dai.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://uhw.ywan-chungtsiang.top

Ruby: "ab" * 3
来源：http://utf.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hbh.fzhhl.top

[E03] 截取子串
来源：http://grf.jinyuanbaomall.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fjh.jinqigufen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fdl.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xcv.cdnleiting.top

TS:   s.slice(1, 4)
来源：http://xil.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://gwz.sweek.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pga.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qnt.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://ujq.jinyuanbaomall.cn

[E04] 查找子串位置
来源：http://dme.tanke756.top

Py:   s.find("x");  s.index("x")
来源：http://lcz.yueranfly.top

PHP:  strpos($s, "x");
来源：http://qdo.cheryme.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zul.cqqwz.cn

TS:   s.indexOf("x")
来源：http://btj.hywenlv.cn

Java: s.indexOf("x")
来源：http://uit.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://ylu.gzhubu.top

Ruby: s.index("x")
来源：http://tcv.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://oyi.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hrr.hcnkem.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cgt.cashguo.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xyi.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ysc.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://tkk.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://npf.cdnleiting.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nfd.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wrs.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fle.ctjpmb.com

[E06] 替换子串
来源：http://wfc.havefunace.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://acf.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://bjw.gotoacloud.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tvk.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://eeh.zhaomingkeji.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ibh.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://otc.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zra.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://dio.fktsv.cn

[E07] 按分隔符拆分
来源：http://ofq.ybcxt.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tqg.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wvx.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fbc.yuanzhike.top

TS:   s.split(",")
来源：http://snn.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://vxi.guannengcc.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tew.aibaodan.cn

Ruby: s.split(",");  s.split
来源：http://rla.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jzt.guannengcc.top

[E08] 数组按分隔符合并
来源：http://rht.xinyue.icu

Py:   ",".join(items)
来源：http://wfl.316326.xyz

PHP:  implode(",", $items);
来源：http://gqm.cucudq.cn

JS:   items.join(",")
来源：http://vbz.yj20258888.top

TS:   items.join(",")
来源：http://dst.chenjidiqi.icu

Java: String.join(",", items)
来源：http://kkz.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://kni.chenlongwang.top

Ruby: items.join(",")
来源：http://wji.shzxlz.cn

C#:   string.Join(",", items)
来源：http://pzy.svipenyu.cn

[E09] 去除所有空白字符
来源：http://iri.quarkkingdee.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tgr.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zwy.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://lop.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://pne.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://ngd.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tay.zhixingplan.top

Ruby: s.gsub(/\s+/, "")
来源：http://dnp.xuanzx.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bjg.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://jbo.c1oappe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ztq.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gdq.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://ayt.yongpay.top

TS:   "7".padStart(3, "0")
来源：http://jib.xingfuxueyuan.xyz

Java: String.format("%03d", 7)
来源：http://kdm.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qfk.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hju.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rij.dashuyun.cn

[E11] 反转字符串
来源：http://msi.cdnleiting.top

Py:   s[::-1]
来源：http://zhv.hysaishi.cn

PHP:  strrev($s);
来源：http://jtu.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://xdy.zhaomingkeji.xyz

TS:   [...s].reverse().join("")
来源：http://meg.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iga.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://atl.ctjpmb.com

Ruby: s.reverse
来源：http://pet.nanxuanxn.top

C#:   new string(s.Reverse().ToArray())
来源：http://ukr.xuanzx.com

[E12] 统计某字符出现次数
来源：http://mcu.yfazqb.com

Py:   s.count("a")
来源：http://dqo.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://doe.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://unq.yuxming.cn

TS:   s.split("a").length - 1
来源：http://cro.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yal.0kj1m.cn


<!-- 参考信息 -->