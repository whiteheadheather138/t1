代发 wailian999

TS:   arr.slice(1, 4);
来源：http://opg.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://nhy.xinyue.icu

Go:   arr[1:4]
来源：http://chf.c1oappe.top

Ruby: arr[1, 3]
来源：http://sqe.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://euk.tianlin.xyz

[D08] 合并两个数组
来源：http://bwb.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://anv.redwolf501.top

PHP:  array_merge($a, $b);
来源：http://lpk.jianghu66.top

JS:   [...a, ...b];  a.concat(b);
来源：http://uhk.316326.xyz

TS:   [...a, ...b];
来源：http://vtt.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://leh.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://cof.zhaomingkeji.xyz

Ruby: a + b;  a.concat(b)
来源：http://frx.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://ttk.xuetiantiany.cn

[D09] 排序（升序）
来源：http://vtp.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://nmg.aizwys.cn

PHP:  sort($arr);
来源：http://hiz.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nwj.jinghuilouyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xls.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iff.tarul.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iya.xuetiantiany.cn

Ruby: arr.sort
来源：http://yhs.jiagoushi.top

C#:   list.Sort();
来源：http://adp.dashuyun.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jsh.tarul.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mtu.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jrc.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rjg.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fbn.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zsv.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://afq.shanyushiyangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zpb.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uat.vehdjk.com

[D11] 反转数组
来源：http://yod.meibo888.top

Py:   arr[::-1];  arr.reverse()
来源：http://snc.tian-w.cn

PHP:  array_reverse($arr);
来源：http://uzg.ybcxt.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xly.vqdsnc.cn

TS:   [...arr].reverse();
来源：http://oyg.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://oci.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://ibu.gzhubu.top

Ruby: arr.reverse
来源：http://sfp.zhongyouzk.top

C#:   list.Reverse();
来源：http://dmt.hcnkem.com

[D12] 查找元素下标
来源：http://fdn.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://wkl.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xom.ydjk.org.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hmo.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ehk.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rqk.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://wub.jqgfzy.top

Ruby: arr.index(x)
来源：http://eek.yongpay.top

C#:   list.IndexOf(x);
来源：http://qxh.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://nes.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qfe.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fyg.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://llk.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://hpb.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fyo.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://azr.ctjpmb.com

Ruby: arr.select { |x| x > 3 }
来源：http://jzc.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://akl.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://mic.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uva.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ito.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://xex.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://mlv.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iuy.vqdsnc.cn

Go:   // 手写循环
来源：http://uov.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://qkw.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xwg.9152youxi.cn

[D15] 去重
来源：http://qoo.sjlbkw.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sbq.ywan-chungtsiang.top

PHP:  array_unique($arr);
来源：http://goi.shuidangran.top

JS:   [...new Set(arr)]
来源：http://lij.wangdashe.top

TS:   [...new Set(arr)]
来源：http://gik.jianghu66.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cag.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://oqf.hnxiangtu.top

Ruby: arr.uniq
来源：http://iob.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://ldu.fktsv.cn

[D16] 求和与平均值
来源：http://zfq.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fee.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xox.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fqx.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eur.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://etr.fzhhl.top

Go:   // 手写循环累加
来源：http://uwy.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iml.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://nnu.epnwcf.com

[D17] 最大值与最小值
来源：http://inr.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://ueq.gaohongyu789.top

PHP:  max($arr);  min($arr);
来源：http://jwx.gzhubu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ucn.zdbjq.cn

TS:   Math.max(...arr);
来源：http://fpa.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uow.ybcxt.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qqn.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://sbe.jinqigufen.top

C#:   list.Max();  list.Min()
来源：http://hzw.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://lty.yj202588.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fcw.guowangkeji.top

PHP:  array_merge(...$nested);
来源：http://jhb.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kng.yvedp.cn

TS:   nested.flat();
来源：http://ewp.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ptz.haohaochexian.top

Go:   // 手写双层循环
来源：http://amm.yj202588.top

Ruby: nested.flatten
来源：http://hsl.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gow.meibo888.top

[D19] 按字段分组
来源：http://mds.zhixingplan.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ckh.yonumen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wor.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://khz.shzxlz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fhw.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dmn.feifeiyinyue.top

Go:   // 手写 map[string][]T
来源：http://lxa.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://igr.mhx1999.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vop.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://dxb.epnwcf.com

Py:   Counter(arr)
来源：http://nsq.bbcook.cn

PHP:  array_count_values($arr);
来源：http://gdh.ywan-chungtsiang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vow.zhengqikj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nqn.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wuo.sysykeji.top

Go:   // 手写 map[T]int
来源：http://ycv.feifeiyinyue.top

Ruby: arr.tally
来源：http://odi.wangshuangyany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cem.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://mdg.birdmap.top

Py:   x in arr
来源：http://gbf.svipenyu.cn

PHP:  in_array($x, $arr, true);
来源：http://gpz.jinqigfzy.top

JS:   arr.includes(x)
来源：http://luc.aizwys.cn

TS:   arr.includes(x)
来源：http://rtn.hfpthk.cn

Java: list.contains(x)
来源：http://jjl.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://zic.cqqwz.cn

Ruby: arr.include?(x)
来源：http://tyr.fengsongda.top

C#:   list.Contains(x)
来源：http://enr.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://eme.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ezj.yj202588.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tbl.zycfv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wqw.guannengcc.top

TS:   [...arr];
来源：http://hic.gaohongyu789.top

Java: new ArrayList<>(list);
来源：http://iti.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hjo.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://xie.daxiang520.top

C#:   new List<int>(list);
来源：http://fdt.andypj.xyz

[D23] reduce 累积计算
来源：http://ojz.iojbl.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ypn.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yta.hfpthk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ldf.sysykeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tnj.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xid.jqgufenzy.top

Go:   // 手写循环
来源：http://bxt.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jcm.jinyuanbaomall.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xar.sysykeji.top

[D24] 字典 / Map 基本操作
来源：http://qvt.ydzc1.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uam.yueranfly.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://soq.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jaj.c1oappe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fpr.yongpay.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jbq.tanke756.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cvt.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sia.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cvc.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://vqb.hywenlv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lly.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ygn.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zsj.pycfn.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mye.fehbvm.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ofu.dianchejie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ssd.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://arn.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://byi.52xcode.cn

[D26] 数组转字符串
来源：http://ipg.jinqigufen.top

Py:   ", ".join(map(str, arr))
来源：http://pfk.sysykeji.top

PHP:  implode(", ", $arr);
来源：http://qrl.nwbrower.top

JS:   arr.join(", ")
来源：http://wgj.jinqigufen.top

TS:   arr.join(", ")
来源：http://yjd.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://wqf.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://hpg.smart0.xyz

Ruby: arr.join(", ")
来源：http://zbk.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://aih.zhaomingkeji.xyz

================================================================================
来源：http://ufn.xylfe.cn

E. 字符串处理
来源：http://cdh.xingfuxueyuan.xyz

================================================================================
来源：http://hmh.zhixingplan.top

[E01] 拼接字符串
来源：http://hrl.sxryk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ezp.sysykeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://puy.hnxiangtu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tuu.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zim.shanyushiyangtech.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vzm.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ffv.quarkkingdee.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kui.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pev.zhixingplan.top

[E02] 重复字符串
来源：http://vka.ybcxt.top

Py:   "ab" * 3
来源：http://zps.bjfxy.top

PHP:  str_repeat("ab", 3);
来源：http://nhc.pycfn.com

JS:   "ab".repeat(3)
来源：http://bhh.jqgufenzy.top

TS:   "ab".repeat(3)
来源：http://rqt.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://yhm.xziqi.cn

Go:   strings.Repeat("ab", 3)
来源：http://iri.pengpengdd.cyou

Ruby: "ab" * 3
来源：http://jrz.pengpengdd.cyou

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ehb.jyoumei.cn

[E03] 截取子串
来源：http://vws.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fpc.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nbk.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://krj.iojbl.cn

TS:   s.slice(1, 4)
来源：http://rzq.gogol.net.cn

Java: s.substring(1, 4)
来源：http://afk.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kma.ehwqpu.com

Ruby: s[1, 3];  s[1..3]
来源：http://xxj.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://usb.jinqigufen.top

[E04] 查找子串位置
来源：http://bhj.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://oee.fehbvm.com

PHP:  strpos($s, "x");
来源：http://eib.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mse.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://zhd.jiagoushi.top

Java: s.indexOf("x")
来源：http://xlp.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://nqc.jyoumei.cn

Ruby: s.index("x")
来源：http://kmj.sysykeji.top

C#:   s.IndexOf("x")
来源：http://eef.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vgg.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gpj.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sot.zhongyouzk.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rhr.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gpw.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://edl.birdmap.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dqa.dianchejie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pnd.tarul.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pyj.jinghuilouyu.cn

[E06] 替换子串
来源：http://vvz.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tli.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://aln.chenjidiqi.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cur.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://kgp.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kog.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wei.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sey.feifeiyinyue.top

C#:   s.Replace("a", "b")
来源：http://ypx.xziqi.cn

[E07] 按分隔符拆分
来源：http://knk.ydjk.org.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://shv.yonumen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vpf.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ebz.ydzc1.top

TS:   s.split(",")
来源：http://kgc.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://guh.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ugr.jinqigfzy.top

Ruby: s.split(",");  s.split
来源：http://voe.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lyj.yj202588.top

[E08] 数组按分隔符合并
来源：http://wcx.jqgufenzy.top

Py:   ",".join(items)
来源：http://eqo.chenlongwang.top

PHP:  implode(",", $items);
来源：http://hzr.xziqi.cn

JS:   items.join(",")
来源：http://rfh.cqqwz.cn

TS:   items.join(",")
来源：http://ixi.smart0.xyz

Java: String.join(",", items)
来源：http://aih.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://tzq.snrcjt.cn

Ruby: items.join(",")
来源：http://szd.andypj.xyz

C#:   string.Join(",", items)
来源：http://pxr.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://shv.chenjidiqi.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://idi.chenjidiqi.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vgn.xuetiantiany.cn

JS:   s.replace(/\s+/g, "")
来源：http://dwh.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://wby.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://sxh.gzhubu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mhx.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kvi.wangshuangyany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mxl.yj20258888.top

[E10] 左侧补零 / 定长填充
来源：http://ioe.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hdv.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hrh.gogol.net.cn

JS:   "7".padStart(3, "0")
来源：http://bib.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://sil.xuanzx.com

Java: String.format("%03d", 7)
来源：http://djm.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://uvz.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://arp.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hvp.shanyushiyangtech.top

[E11] 反转字符串
来源：http://rnd.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://bjz.nanxuanxn.top

PHP:  strrev($s);
来源：http://hjz.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://jhs.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://grc.fktsv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://atw.iojbl.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qgp.redwolf501.top

Ruby: s.reverse
来源：http://rkb.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://gdz.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://dek.jiagoushi.top

Py:   s.count("a")
来源：http://lgj.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://dyx.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://okh.yj20258888.top

TS:   s.split("a").length - 1
来源：http://qyb.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://npk.nanxinkj.top

Go:   strings.Count(s, "a")
来源：http://usa.hcnkem.com

Ruby: s.count("a")
来源：http://tke.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://eyz.gzhubu.top

[E13] 逐字符遍历
来源：http://cvo.havefunace.top

Py:   for ch in s: print(ch)
来源：http://ufs.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hgs.fzhhl.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://olw.bjfxy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xan.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iac.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hyo.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gtn.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mjf.gogol.net.cn

[E14] URL 编码与 Base64
来源：http://jmt.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yfi.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://czb.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://chx.chenlongwang.top


<!-- 参考信息 -->