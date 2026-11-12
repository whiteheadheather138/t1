代发 wailian999

Java: list.size();
来源：http://bkh.smart0.xyz

Go:   len(arr)
来源：http://igx.daria6918.cn

Ruby: arr.length; arr.size
来源：http://fgk.yuxming.cn

C#:   list.Count;
来源：http://sfr.yongpay.top

[D07] 切片 / 取子数组
来源：http://tcv.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aoz.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://ajs.wangshuangyany.cn

JS:   arr.slice(1, 4);
来源：http://ljz.havefunace.top

TS:   arr.slice(1, 4);
来源：http://pre.pycfn.com

Java: list.subList(1, 4);
来源：http://msy.c1oappe.top

Go:   arr[1:4]
来源：http://vrw.iojbl.cn

Ruby: arr[1, 3]
来源：http://yxg.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://itj.chenjidiqi.icu

[D08] 合并两个数组
来源：http://jhh.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://arz.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://awb.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://okr.ppjwa.cn

TS:   [...a, ...b];
来源：http://cfs.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rhl.zycfv.cn

Go:   append(a, b...)
来源：http://mjm.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://sgq.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://dtt.yongpay.top

[D09] 排序（升序）
来源：http://nxt.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://dhf.yj202588.top

PHP:  sort($arr);
来源：http://fxj.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wbq.bjfxy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://srf.tanke756.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nnt.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hfh.redwolf501.top

Ruby: arr.sort
来源：http://rck.nwbrower.top

C#:   list.Sort();
来源：http://fyc.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cqd.shuidangran.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nwb.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aqc.xingfuxueyuan.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tns.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hqw.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cqh.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ohx.yj202588.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dkq.hnqzz.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lqt.daxiang520.top

[D11] 反转数组
来源：http://edj.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://jfe.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://cyt.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nnm.cashguo.top

TS:   [...arr].reverse();
来源：http://ywx.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://cgy.shangyingyoupin.top

Go:   slices.Reverse(arr)
来源：http://ijb.feifeiyinyue.top

Ruby: arr.reverse
来源：http://ewa.jqgufenzy.top

C#:   list.Reverse();
来源：http://ffh.xziqi.cn

[D12] 查找元素下标
来源：http://hsk.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://unq.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kmb.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://whp.xuetiantiany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tla.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iuh.fehbvm.com

Go:   slices.Index(arr, x)
来源：http://pad.hcnkem.com

Ruby: arr.index(x)
来源：http://psr.bjfxy.top

C#:   list.IndexOf(x);
来源：http://ozu.zdqjudy.top

[D13] 过滤（保留满足条件的）
来源：http://koa.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pvn.jiagoushi.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cgj.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://gxc.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://lnb.iojbl.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dkl.cheryme.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ftr.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dbb.redwolf501.top

C#:   list.Where(x => x > 3).ToList()
来源：http://iou.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://vrh.jianghu66.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zsk.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jpv.hongshengwenyu.top

JS:   arr.map(x => x * 2)
来源：http://ctn.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://tlw.fzhhl.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://sat.hfpthk.cn

Go:   // 手写循环
来源：http://fhf.hnqzz.top

Ruby: arr.map { |x| x * 2 }
来源：http://mgj.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ljy.hywenlv.cn

[D15] 去重
来源：http://pog.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nua.fehbvm.com

PHP:  array_unique($arr);
来源：http://szn.yanxiufei.cn

JS:   [...new Set(arr)]
来源：http://wji.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://qol.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xwy.chenlongwang.top

Go:   // 用 map[T]struct{} 手写
来源：http://oyc.aizwys.cn

Ruby: arr.uniq
来源：http://jjh.epnwcf.com

C#:   list.Distinct().ToList()
来源：http://hse.chenzaomai.com

[D16] 求和与平均值
来源：http://yhw.52xcode.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nzy.xuetiantiany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qis.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kci.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yca.zhoulong.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://feb.hongshengwenyu.top

Go:   // 手写循环累加
来源：http://qdw.smart0.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pmz.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://zes.chenzaomai.com

[D17] 最大值与最小值
来源：http://uer.pycfn.com

Py:   max(arr);  min(arr)
来源：http://udz.yj20258.top

PHP:  max($arr);  min($arr);
来源：http://pys.yvedp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zqf.ppjwa.cn

TS:   Math.max(...arr);
来源：http://gth.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qnw.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pex.uphjek.com

Ruby: arr.max;  arr.min
来源：http://tml.yj20258.top

C#:   list.Max();  list.Min()
来源：http://ozq.guannengcc.top

[D18] 扁平化嵌套数组
来源：http://jpo.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pus.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://tcl.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://owg.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://tuq.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://plv.zhijiandao.cn

Go:   // 手写双层循环
来源：http://fbj.fengsongda.top

Ruby: nested.flatten
来源：http://uyo.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://ynf.daria6918.cn

[D19] 按字段分组
来源：http://vzz.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xvs.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gyq.birdmap.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://buj.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gbj.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dly.uphjek.com

Go:   // 手写 map[string][]T
来源：http://zsn.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dum.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jvb.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://nze.hammf.cn

Py:   Counter(arr)
来源：http://iqq.tian-w.cn

PHP:  array_count_values($arr);
来源：http://nqd.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xtd.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pqg.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nrh.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://ain.zhongyouzk.top

Ruby: arr.tally
来源：http://zkv.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aiq.daria6918.cn

[D21] 判断是否包含某元素
来源：http://jtt.hcnkem.com

Py:   x in arr
来源：http://rsm.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://bmw.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://mnt.pycfn.com

TS:   arr.includes(x)
来源：http://mpp.sysykeji.top

Java: list.contains(x)
来源：http://sqg.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://gbe.smart0.xyz

Ruby: arr.include?(x)
来源：http://wjs.jyoumei.cn

C#:   list.Contains(x)
来源：http://zwc.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://mkt.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cqr.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fhb.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bxj.chenjidiqi.icu

TS:   [...arr];
来源：http://nxc.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://boq.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qro.xingfuxueyuan.xyz

Ruby: arr.dup;  arr.clone
来源：http://zov.xylfe.cn

C#:   new List<int>(list);
来源：http://tqp.yvedp.cn

[D23] reduce 累积计算
来源：http://eqv.zhoulong.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cmy.yj20258.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mne.yj202588.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kgb.sufxvd.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://snr.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ksx.pengpengdd.cyou

Go:   // 手写循环
来源：http://wbq.hongshengwenyu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hjh.havefunace.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hsn.quarkkingdee.top

[D24] 字典 / Map 基本操作
来源：http://egl.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ifc.epnwcf.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zts.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kdy.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zby.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blm.jinghuilouyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zcc.zhijiandao.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ovr.kuanghao11.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yzz.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://nov.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kjd.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jbo.xingfuxueyuan.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pfz.tanke756.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jbm.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ijq.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hvq.jqgufenzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eoh.zhoulong.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://czl.shuidangran.top

[D26] 数组转字符串
来源：http://fxb.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://xww.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://ufw.yuxming.cn

JS:   arr.join(", ")
来源：http://foq.tianlin.xyz

TS:   arr.join(", ")
来源：http://pay.jlsjyb.cn

Java: String.join(", ", list)
来源：http://icg.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://dua.andypj.xyz

Ruby: arr.join(", ")
来源：http://ptg.hesvh.cn

C#:   string.Join(", ", list)
来源：http://wyf.xingfuxueyuan.xyz

================================================================================
来源：http://flq.mhx1999.top

E. 字符串处理
来源：http://rft.tianlin.xyz

================================================================================
来源：http://uqb.birdmap.top

[E01] 拼接字符串
来源：http://pmt.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lwm.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ogj.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://olu.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tzz.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://brr.daria6918.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dkh.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://thi.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rgu.cheryme.top

[E02] 重复字符串
来源：http://bln.jiagoushi.top

Py:   "ab" * 3
来源：http://sfk.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://fbg.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://lgc.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://ydk.yongpay.top

Java: "ab".repeat(3)
来源：http://ujw.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://bxy.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://dwt.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vrm.yj20258.top

[E03] 截取子串
来源：http://itw.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dqr.daxiang520.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dqp.nanxinkj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cmc.yvedp.cn

TS:   s.slice(1, 4)
来源：http://qpk.shanyushiyangkeji.top

Java: s.substring(1, 4)
来源：http://ecx.gogol.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tlg.chenlongwang.top

Ruby: s[1, 3];  s[1..3]
来源：http://pku.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://wer.andypj.xyz

[E04] 查找子串位置
来源：http://gxh.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://zku.ctjpmb.com

PHP:  strpos($s, "x");
来源：http://dap.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://enq.jiagoushi.top

TS:   s.indexOf("x")
来源：http://kci.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://pna.redwolf501.top

Go:   strings.Index(s, "x")
来源：http://gjm.meibo888.top

Ruby: s.index("x")
来源：http://zxx.ydzc1.top

C#:   s.IndexOf("x")
来源：http://wcn.uphjek.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://itk.birdmap.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://coh.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ydy.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ovp.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pmd.chenjidiqi.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tff.yvedp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wxf.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qmk.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hib.fanxiaobao.xyz

[E06] 替换子串
来源：http://uyy.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oub.tianlin.xyz

PHP:  str_replace("a", "b", $s);
来源：http://uxf.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pvz.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://mtf.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nsm.bjfxy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://njz.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://arb.sweek.top

C#:   s.Replace("a", "b")
来源：http://yej.haohaochexian.top

[E07] 按分隔符拆分
来源：http://mae.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pii.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://huh.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ayl.sjlbkw.cn

TS:   s.split(",")
来源：http://ild.jiagoushi.top

Java: s.split(",");  s.split("\\s+")
来源：http://wmb.ybcxt.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://usy.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://cto.uphjek.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mmh.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://bnw.redwolf501.top

Py:   ",".join(items)
来源：http://lwi.yfazqb.com

PHP:  implode(",", $items);
来源：http://rtz.jqgfzy.top

JS:   items.join(",")
来源：http://qms.zhixingplan.top

TS:   items.join(",")
来源：http://ssn.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://yzv.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://tam.xylfe.cn

Ruby: items.join(",")
来源：http://bdz.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://xsr.tarul.cn

[E09] 去除所有空白字符
来源：http://ngs.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wpu.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qdu.xinyue.icu

JS:   s.replace(/\s+/g, "")
来源：http://pox.jqgfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://vwt.zhixingplan.top

Java: s.replaceAll("\\s+", "")
来源：http://eup.chenzaomai.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://gue.kuanghao11.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mkz.jqgufenzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kqf.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://rjk.meibo888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ulq.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rkp.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://dsx.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://eqh.0kj1m.cn

Java: String.format("%03d", 7)
来源：http://hrx.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yht.yueranfly.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://adi.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://otk.hfpthk.cn

[E11] 反转字符串
来源：http://xqa.nanxinkj.top

Py:   s[::-1]
来源：http://npl.fktsv.cn

PHP:  strrev($s);
来源：http://nhb.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://avt.zdqjudy.top

TS:   [...s].reverse().join("")
来源：http://zcy.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xjp.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hej.c1oappe.top

Ruby: s.reverse
来源：http://ftd.vehdjk.com

C#:   new string(s.Reverse().ToArray())
来源：http://thj.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://wxk.hcnkem.com

Py:   s.count("a")
来源：http://szy.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://azg.xziqi.cn

JS:   s.split("a").length - 1
来源：http://dlc.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://vdk.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://afr.xuanzx.com

Go:   strings.Count(s, "a")
来源：http://vit.xylfe.cn

Ruby: s.count("a")
来源：http://xjy.ivvv.top

C#:   s.Count(c => c == 'a')
来源：http://mwq.cqqwz.cn

[E13] 逐字符遍历
来源：http://mug.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://gef.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://air.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jko.cheryme.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fgy.meibo888.top


<!-- 参考信息 -->