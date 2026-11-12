代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aws.iojbl.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ean.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://tdw.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pot.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://beh.bjfxy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tuv.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://jen.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://cph.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://ekk.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ypw.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xbk.xuanzx.com

[D06] 数组长度
来源：http://vuk.cheryme.top

Py:   len(arr)
来源：http://hxy.yongpay.top

PHP:  count($arr);
来源：http://jud.0kj1m.cn

JS:   arr.length
来源：http://psp.jqgfzy.top

TS:   arr.length
来源：http://ewb.fengsongda.top

Java: list.size();
来源：http://uaw.smart0.xyz

Go:   len(arr)
来源：http://yhr.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://hek.guannengcc.top

C#:   list.Count;
来源：http://ahe.cqqwz.cn

[D07] 切片 / 取子数组
来源：http://rmk.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fax.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://scx.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://sxx.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://qrk.hywenlv.cn

Java: list.subList(1, 4);
来源：http://nyt.bbcook.cn

Go:   arr[1:4]
来源：http://mkp.cashguo.top

Ruby: arr[1, 3]
来源：http://veq.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://iqj.xuanzx.com

[D08] 合并两个数组
来源：http://ftq.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://swz.dianchejie.cn

PHP:  array_merge($a, $b);
来源：http://iid.guannengcc.top

JS:   [...a, ...b];  a.concat(b);
来源：http://uzf.tanke756.top

TS:   [...a, ...b];
来源：http://oqs.yonumen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zhh.sysykeji.top

Go:   append(a, b...)
来源：http://mef.yanxiufei.cn

Ruby: a + b;  a.concat(b)
来源：http://pjr.jianghu66.top

C#:   a.Concat(b).ToList()
来源：http://wmx.feifeiyinyue.top

[D09] 排序（升序）
来源：http://gld.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://xfr.yanxiufei.cn

PHP:  sort($arr);
来源：http://zch.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cvd.haohaochexian.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uuo.tanke756.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qis.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vla.0kj1m.cn

Ruby: arr.sort
来源：http://mtn.hcnkem.com

C#:   list.Sort();
来源：http://ylb.sufxvd.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pkr.nanxinkj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nza.cheryme.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pht.feifeiyinyue.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ytc.gaohongyu789.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fqb.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aam.jinqigfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wdr.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bfg.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vxc.hnqzz.top

[D11] 反转数组
来源：http://klg.havefunace.top

Py:   arr[::-1];  arr.reverse()
来源：http://ooc.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://rgk.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rok.yueranfly.top

TS:   [...arr].reverse();
来源：http://ajb.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://vtp.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://zju.snrcjt.cn

Ruby: arr.reverse
来源：http://ecs.snrcjt.cn

C#:   list.Reverse();
来源：http://dke.shangyingyoupin.top

[D12] 查找元素下标
来源：http://ats.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://lyh.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rgy.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kdz.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ayw.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xpr.dashuyun.cn

Go:   slices.Index(arr, x)
来源：http://cih.yvedp.cn

Ruby: arr.index(x)
来源：http://wez.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://bvg.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://tww.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qdu.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cxs.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://arb.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://aia.gogol.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vun.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mgz.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://wos.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jsl.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://osl.zhijiandao.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jzt.bbcook.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ufk.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://bjv.yvedp.cn

TS:   arr.map(x => x * 2)
来源：http://qxa.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dgn.mhx1999.top

Go:   // 手写循环
来源：http://crv.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://arl.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tdr.cheryme.top

[D15] 去重
来源：http://nyt.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hzp.sweek.top

PHP:  array_unique($arr);
来源：http://pmj.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://bmo.jianghu66.top

TS:   [...new Set(arr)]
来源：http://xqq.shanyushiyangtech.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hes.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qvy.sxryk.cn

Ruby: arr.uniq
来源：http://bao.ydzc1.top

C#:   list.Distinct().ToList()
来源：http://rfj.zycfv.cn

[D16] 求和与平均值
来源：http://lbh.hywenlv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bob.vqdsnc.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fyh.cucudq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nvk.xingfuxueyuan.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rfm.gogol.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qzi.tanke756.top

Go:   // 手写循环累加
来源：http://soe.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mps.hywenlv.cn

C#:   list.Sum();  list.Average()
来源：http://skn.9152youxi.cn

[D17] 最大值与最小值
来源：http://gdr.sufxvd.cn

Py:   max(arr);  min(arr)
来源：http://xbw.316326.xyz

PHP:  max($arr);  min($arr);
来源：http://iij.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lgn.yueranfly.top

TS:   Math.max(...arr);
来源：http://cap.hywenlv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://egf.nwbrower.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ckd.tanke756.top

Ruby: arr.max;  arr.min
来源：http://ipf.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://dnl.hongshengwenyu.top

[D18] 扁平化嵌套数组
来源：http://qud.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ltd.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://sjq.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mdq.havefunace.top

TS:   nested.flat();
来源：http://ybx.meibo888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lnb.jinqigufen.top

Go:   // 手写双层循环
来源：http://zyu.uphjek.com

Ruby: nested.flatten
来源：http://hjh.hnxiangtu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mrg.tarul.cn

[D19] 按字段分组
来源：http://dtr.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jrn.shzxlz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vqf.zdbjq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ipr.9152youxi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qvd.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kka.cheryme.top

Go:   // 手写 map[string][]T
来源：http://fpw.shanyushiyangtech.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gxs.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uli.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://zly.jiagoushi.top

Py:   Counter(arr)
来源：http://hbz.andypj.xyz

PHP:  array_count_values($arr);
来源：http://zxs.gzhubu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ilv.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hik.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cuh.daria6918.cn

Go:   // 手写 map[T]int
来源：http://xpv.aizwys.cn

Ruby: arr.tally
来源：http://tux.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yih.tian-w.cn

[D21] 判断是否包含某元素
来源：http://vdw.zhaomingkeji.xyz

Py:   x in arr
来源：http://abi.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://eul.shzxlz.cn

JS:   arr.includes(x)
来源：http://ase.tian-w.cn

TS:   arr.includes(x)
来源：http://izs.redwolf501.top

Java: list.contains(x)
来源：http://nhf.yj20258888.top

Go:   slices.Contains(arr, x)
来源：http://sdk.hnqzz.top

Ruby: arr.include?(x)
来源：http://oyg.redwolf501.top

C#:   list.Contains(x)
来源：http://hnf.kuanghao11.cn

[D22] 复制数组（避免共享引用）
来源：http://pmn.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cvx.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uqf.daxiang520.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pqr.yongpay.top

TS:   [...arr];
来源：http://erc.zhoulong.xyz

Java: new ArrayList<>(list);
来源：http://gzb.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dml.mhx1999.top

Ruby: arr.dup;  arr.clone
来源：http://elz.jlsjyb.cn

C#:   new List<int>(list);
来源：http://pci.jyoumei.cn

[D23] reduce 累积计算
来源：http://sol.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tct.wangdashe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://idv.jyoumei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://han.hysaishi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://raz.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hvc.zhengqikj.top

Go:   // 手写循环
来源：http://xzw.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nlg.jinyuanbaomall.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mhk.daxiang520.top

[D24] 字典 / Map 基本操作
来源：http://gym.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qnv.shanyushiyangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ajl.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bpn.jianghu66.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nmz.sjlbkw.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qdz.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pyl.hnqzz.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rxs.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gox.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://ywt.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qsm.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hfv.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gjl.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ncn.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rwi.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tpm.yuxming.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aaq.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kbj.daria6918.cn

[D26] 数组转字符串
来源：http://vyi.sxryk.cn

Py:   ", ".join(map(str, arr))
来源：http://hed.zycfv.cn

PHP:  implode(", ", $arr);
来源：http://vmq.jinqigufen.top

JS:   arr.join(", ")
来源：http://nyq.zdbjq.cn

TS:   arr.join(", ")
来源：http://ozw.zhixingplan.top

Java: String.join(", ", list)
来源：http://pjf.xylfe.cn

Go:   strings.Join(strs, ", ")
来源：http://vfk.hesvh.cn

Ruby: arr.join(", ")
来源：http://kdk.tanke756.top

C#:   string.Join(", ", list)
来源：http://dxo.hnqzz.top

================================================================================
来源：http://vih.ehwqpu.com

E. 字符串处理
来源：http://tam.vehdjk.com

================================================================================
来源：http://plq.hammf.cn

[E01] 拼接字符串
来源：http://yap.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zqa.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kwl.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dmu.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lin.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ike.uphjek.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tqh.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://twf.daria6918.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gcc.yonumen.top

[E02] 重复字符串
来源：http://chm.birdmap.top

Py:   "ab" * 3
来源：http://ydx.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://rxz.fengsongda.top

JS:   "ab".repeat(3)
来源：http://ilx.xinyue.icu

TS:   "ab".repeat(3)
来源：http://hml.cqqwz.cn

Java: "ab".repeat(3)
来源：http://jnk.hnxiangtu.top

Go:   strings.Repeat("ab", 3)
来源：http://koi.dianchejie.cn

Ruby: "ab" * 3
来源：http://xaj.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://osj.cqqwz.cn

[E03] 截取子串
来源：http://oph.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://laa.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xri.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tzm.fzhhl.top

TS:   s.slice(1, 4)
来源：http://jkd.jinqigufen.top

Java: s.substring(1, 4)
来源：http://dku.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wne.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://enr.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://hag.gzhubu.top

[E04] 查找子串位置
来源：http://gfd.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://zqh.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://ufc.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ylu.fehbvm.com

TS:   s.indexOf("x")
来源：http://qyd.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://gpa.pycfn.com

Go:   strings.Index(s, "x")
来源：http://lzr.gaohongyu789.top

Ruby: s.index("x")
来源：http://kxf.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://ekq.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kip.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://icn.jiagoushi.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pgk.hcnkem.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wbh.guowangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gaz.zhongyouzk.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://avb.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pud.sjlbkw.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eoy.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pel.zycfv.cn

[E06] 替换子串
来源：http://syl.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ghv.yonumen.top

PHP:  str_replace("a", "b", $s);
来源：http://zig.xingfuxueyuan.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jps.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://ztz.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rad.ppjwa.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://unz.yangfankeji.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zsg.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://tuy.xinyue.icu

[E07] 按分隔符拆分
来源：http://meh.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://puu.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ids.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cop.hesvh.cn

TS:   s.split(",")
来源：http://pra.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://tqi.shanyushiyangtech.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dkb.hnqzz.top

Ruby: s.split(",");  s.split
来源：http://zbt.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sdu.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://ejt.haohaochexian.top

Py:   ",".join(items)
来源：http://yoq.dianchejie.cn

PHP:  implode(",", $items);
来源：http://ded.c1oappe.top

JS:   items.join(",")
来源：http://uvu.zhixingplan.top

TS:   items.join(",")
来源：http://krm.cqqwz.cn

Java: String.join(",", items)
来源：http://qrw.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://uen.yfazqb.com

Ruby: items.join(",")
来源：http://ppl.aibaodan.cn

C#:   string.Join(",", items)
来源：http://htz.zhixingplan.top

[E09] 去除所有空白字符
来源：http://ntd.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vdv.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://coz.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://srh.sysykeji.top

TS:   s.replace(/\s+/g, "")
来源：http://udu.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://oaj.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://msw.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://tnq.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yec.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://ekk.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gzw.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://snj.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://ddk.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://jbl.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://rwe.jianghu66.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://atv.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://urw.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cgd.tianlin.xyz

[E11] 反转字符串
来源：http://aqb.vehdjk.com

Py:   s[::-1]
来源：http://rfd.cucudq.cn

PHP:  strrev($s);
来源：http://abj.sjlbkw.cn

JS:   [...s].reverse().join("")
来源：http://olj.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://ktk.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bjg.epnwcf.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://xhi.cashguo.top


<!-- 参考信息 -->