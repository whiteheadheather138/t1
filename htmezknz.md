代发 wailian999

Java: list.size();
来源：http://dpg.zycfv.cn

Go:   len(arr)
来源：http://mpz.zycfv.cn

Ruby: arr.length; arr.size
来源：http://vzf.wangshuangyany.cn

C#:   list.Count;
来源：http://jie.hcnkem.com

[D07] 切片 / 取子数组
来源：http://hag.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wwy.yueranfly.top

PHP:  array_slice($arr, 1, 3);
来源：http://ndv.cheryme.top

JS:   arr.slice(1, 4);
来源：http://hhn.yuxming.cn

TS:   arr.slice(1, 4);
来源：http://kjc.yangfankeji.com

Java: list.subList(1, 4);
来源：http://zey.sjlbkw.cn

Go:   arr[1:4]
来源：http://rsm.gzhubu.top

Ruby: arr[1, 3]
来源：http://kbv.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://ege.yfazqb.com

[D08] 合并两个数组
来源：http://lnp.redwolf501.top

Py:   a + b;  a.extend(b)
来源：http://gdv.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://dav.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dsq.cqqwz.cn

TS:   [...a, ...b];
来源：http://bqd.fehbvm.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cnw.hongshengwenyu.top

Go:   append(a, b...)
来源：http://ehq.guannengcc.top

Ruby: a + b;  a.concat(b)
来源：http://aaf.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://kfq.gzhubu.top

[D09] 排序（升序）
来源：http://jqo.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://zkz.kuanghao11.cn

PHP:  sort($arr);
来源：http://utr.feifeiyinyue.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ovh.svipenyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jpc.zycfv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tfl.cqqwz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://czo.sjlbkw.cn

Ruby: arr.sort
来源：http://eca.mhx1999.top

C#:   list.Sort();
来源：http://tlx.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vpe.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vwe.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jew.chenzaomai.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fus.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://enr.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bpx.jinqigfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hsq.cashguo.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vhy.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pyl.yj20258.top

[D11] 反转数组
来源：http://kin.xuetiantiany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wsj.sxryk.cn

PHP:  array_reverse($arr);
来源：http://chn.pengpengdd.cyou

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dnj.fzhhl.top

TS:   [...arr].reverse();
来源：http://oyc.smart0.xyz

Java: Collections.reverse(list);
来源：http://zhn.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://hyq.yj20258.top

Ruby: arr.reverse
来源：http://cch.mhx1999.top

C#:   list.Reverse();
来源：http://brt.316326.xyz

[D12] 查找元素下标
来源：http://gci.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://dpj.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://axr.xuetiantiany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iwu.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zhc.guowangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lox.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://idb.kuanghao11.cn

Ruby: arr.index(x)
来源：http://xxz.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://utr.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://qvk.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qsc.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ywm.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://wdb.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://ruv.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rne.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://svs.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://kap.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://tqg.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://val.hysaishi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qel.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ger.yfazqb.com

JS:   arr.map(x => x * 2)
来源：http://nza.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://osw.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lqw.shzxlz.cn

Go:   // 手写循环
来源：http://wam.daxiang520.top

Ruby: arr.map { |x| x * 2 }
来源：http://qph.mhx1999.top

C#:   list.Select(x => x * 2).ToList()
来源：http://aep.yfazqb.com

[D15] 去重
来源：http://gsp.sweek.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yfp.guowangkeji.top

PHP:  array_unique($arr);
来源：http://hxi.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://qyz.tian-w.cn

TS:   [...new Set(arr)]
来源：http://wvl.shuidangran.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jdm.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://yzo.tian-w.cn

Ruby: arr.uniq
来源：http://odm.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://nyo.yvedp.cn

[D16] 求和与平均值
来源：http://ton.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rhp.zdbjq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://opi.birdmap.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xfd.ydzc1.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mvd.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://csh.zycfv.cn

Go:   // 手写循环累加
来源：http://aue.hywenlv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iap.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://trd.9152youxi.cn

[D17] 最大值与最小值
来源：http://ntp.meibo888.top

Py:   max(arr);  min(arr)
来源：http://efj.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://rro.svipenyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yxt.nanxinkj.top

TS:   Math.max(...arr);
来源：http://jgt.wangdashe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gmd.tianlin.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cws.52xcode.cn

Ruby: arr.max;  arr.min
来源：http://erc.cashguo.top

C#:   list.Max();  list.Min()
来源：http://isp.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://yrn.sweek.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hyc.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://vqd.tian-w.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jlo.daria6918.cn

TS:   nested.flat();
来源：http://rsx.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://avy.yj20258888.top

Go:   // 手写双层循环
来源：http://aae.cucudq.cn

Ruby: nested.flatten
来源：http://inw.hnxiangtu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uij.bjfxy.top

[D19] 按字段分组
来源：http://feo.gaohongyu789.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://euf.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xnv.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://svr.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ukg.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fct.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://miq.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rzp.sjlbkw.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lug.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://hzj.sysykeji.top

Py:   Counter(arr)
来源：http://xay.xziqi.cn

PHP:  array_count_values($arr);
来源：http://fts.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nxg.sysykeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://flu.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vud.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://pgy.zhijiandao.cn

Ruby: arr.tally
来源：http://ovx.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sgd.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://pcc.sxryk.cn

Py:   x in arr
来源：http://tze.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://ubs.pycfn.com

JS:   arr.includes(x)
来源：http://xfu.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://qbh.havefunace.top

Java: list.contains(x)
来源：http://gwq.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://mzc.bjfxy.top

Ruby: arr.include?(x)
来源：http://btv.aibaodan.cn

C#:   list.Contains(x)
来源：http://xtd.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://uqc.zycfv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hre.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yze.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kkr.gotoacloud.top

TS:   [...arr];
来源：http://oxr.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://kti.yuxming.cn

Go:   copied := append([]int(nil), arr...)
来源：http://byq.hywenlv.cn

Ruby: arr.dup;  arr.clone
来源：http://wez.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://vob.wangdashe.top

[D23] reduce 累积计算
来源：http://kcb.guannengcc.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://knl.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lit.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zcf.sjlbkw.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://txs.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yxk.jqgfzy.top

Go:   // 手写循环
来源：http://uej.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xxb.fanxiaobao.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sqb.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://zkb.yj202588.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kgu.wangshuangyany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dpz.smart0.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tps.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dky.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kfn.uphjek.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pcc.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tns.haohaochexian.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://thn.cucudq.cn

[D25] Set 集合去重与交并差
来源：http://gtx.c1oappe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rsv.hysaishi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ker.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rdn.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dxl.tarul.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vrg.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fhr.xuanzx.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vua.jinqigfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ezr.cucudq.cn

[D26] 数组转字符串
来源：http://buj.xingfuxueyuan.xyz

Py:   ", ".join(map(str, arr))
来源：http://plm.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://avr.zycfv.cn

JS:   arr.join(", ")
来源：http://jxi.hcnkem.com

TS:   arr.join(", ")
来源：http://txy.jinqigufen.top

Java: String.join(", ", list)
来源：http://dbc.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://sfk.xuanzx.com

Ruby: arr.join(", ")
来源：http://fvo.pycfn.com

C#:   string.Join(", ", list)
来源：http://jmy.chenlongwang.top

================================================================================
来源：http://wld.snrcjt.cn

E. 字符串处理
来源：http://kwn.shuidangran.top

================================================================================
来源：http://clr.tanke756.top

[E01] 拼接字符串
来源：http://snb.zhengqikj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xwn.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://djn.snrcjt.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iyl.pengpengdd.cyou

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zla.yj20258888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lxg.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tew.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ipv.birdmap.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tig.jinqigfzy.top

[E02] 重复字符串
来源：http://npu.zhiwuduotai.top

Py:   "ab" * 3
来源：http://fur.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://ttx.feifeiyinyue.top

JS:   "ab".repeat(3)
来源：http://omy.ivvv.top

TS:   "ab".repeat(3)
来源：http://cve.0kj1m.cn

Java: "ab".repeat(3)
来源：http://gyk.zhixingplan.top

Go:   strings.Repeat("ab", 3)
来源：http://yfr.yangfankeji.com

Ruby: "ab" * 3
来源：http://dwt.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ptb.xinyue.icu

[E03] 截取子串
来源：http://gkq.dashuyun.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ums.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rig.vqdsnc.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qnw.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://bge.yvedp.cn

Java: s.substring(1, 4)
来源：http://nsu.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zla.daxiang520.top

Ruby: s[1, 3];  s[1..3]
来源：http://yfd.hesvh.cn

C#:   s.Substring(1, 3)
来源：http://mzv.ivvv.top

[E04] 查找子串位置
来源：http://nyl.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://niu.aibaodan.cn

PHP:  strpos($s, "x");
来源：http://frm.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wsq.zhixingplan.top

TS:   s.indexOf("x")
来源：http://zpt.yvedp.cn

Java: s.indexOf("x")
来源：http://nkv.yuxming.cn

Go:   strings.Index(s, "x")
来源：http://wdm.daxiang520.top

Ruby: s.index("x")
来源：http://jxk.bbcook.cn

C#:   s.IndexOf("x")
来源：http://gio.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://sos.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://igr.hammf.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lpg.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bnf.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zvr.hongshengwenyu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qtz.sufxvd.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rom.sjlbkw.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hkg.yuanzhike.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bbn.birdmap.top

[E06] 替换子串
来源：http://ikj.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kul.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://uls.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lxm.meibo888.top

TS:   s.replaceAll("a", "b")
来源：http://sat.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mbr.xuanzx.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gbn.xylfe.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qlm.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://hcy.vqdsnc.cn

[E07] 按分隔符拆分
来源：http://gxh.ehwqpu.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vpk.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ocp.ydjk.org.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://onn.cheryme.top

TS:   s.split(",")
来源：http://zdt.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://zju.bjfxy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ggu.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://aaw.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zwj.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://yhb.wangshuangyany.cn

Py:   ",".join(items)
来源：http://dch.zhengqikj.top

PHP:  implode(",", $items);
来源：http://bgh.fzhhl.top

JS:   items.join(",")
来源：http://xns.jianghu66.top

TS:   items.join(",")
来源：http://mja.hysaishi.cn

Java: String.join(",", items)
来源：http://cub.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://hbh.ydjk.org.cn

Ruby: items.join(",")
来源：http://lxy.bjfxy.top

C#:   string.Join(",", items)
来源：http://and.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://vkl.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xor.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mrr.c1oappe.top

JS:   s.replace(/\s+/g, "")
来源：http://ijb.yonumen.top

TS:   s.replace(/\s+/g, "")
来源：http://bvn.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://hah.nanxinkj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://eeu.quarkkingdee.top

Ruby: s.gsub(/\s+/, "")
来源：http://pls.fzhhl.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hml.hysaishi.cn

[E10] 左侧补零 / 定长填充
来源：http://rth.chenjidiqi.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ghb.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://glc.bjfxy.top

JS:   "7".padStart(3, "0")
来源：http://lec.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://kmc.jinghuilouyu.cn

Java: String.format("%03d", 7)
来源：http://afk.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iha.yanxiufei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://djl.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sqd.xziqi.cn

[E11] 反转字符串
来源：http://dwb.jianghu66.top

Py:   s[::-1]
来源：http://lei.tianlin.xyz

PHP:  strrev($s);
来源：http://xwh.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://gfg.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://onb.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qgg.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gnq.sweek.top

Ruby: s.reverse
来源：http://rbc.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ehc.yanxiufei.cn

[E12] 统计某字符出现次数
来源：http://wmx.hesvh.cn

Py:   s.count("a")
来源：http://qyr.xingfuxueyuan.xyz

PHP:  substr_count($s, "a");
来源：http://rrg.yuxming.cn

JS:   s.split("a").length - 1
来源：http://jea.dashuyun.cn

TS:   s.split("a").length - 1
来源：http://sfp.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fjf.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://ear.ivvv.top

Ruby: s.count("a")
来源：http://hvt.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://trt.hammf.cn

[E13] 逐字符遍历
来源：http://tmr.zhijiandao.cn

Py:   for ch in s: print(ch)
来源：http://gxr.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rjx.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ood.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://otl.snrcjt.cn


<!-- 参考信息 -->