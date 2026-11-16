代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://cmc.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xjd.yuanzhike.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ztu.chenzaomai.com

[D06] 数组长度
来源：http://hbm.nwbrower.top

Py:   len(arr)
来源：http://edj.gogol.net.cn

PHP:  count($arr);
来源：http://hkj.zhengqikj.top

JS:   arr.length
来源：http://avt.9152youxi.cn

TS:   arr.length
来源：http://mzx.cdnleiting.top

Java: list.size();
来源：http://ghk.dashuyun.cn

Go:   len(arr)
来源：http://non.andypj.xyz

Ruby: arr.length; arr.size
来源：http://dob.zhaomingkeji.xyz

C#:   list.Count;
来源：http://lis.jinqigufen.top

[D07] 切片 / 取子数组
来源：http://pvw.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eeg.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://tku.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://mzj.meibo888.top

TS:   arr.slice(1, 4);
来源：http://wnu.jinyuanbaomall.cn

Java: list.subList(1, 4);
来源：http://imy.shangyingyoupin.top

Go:   arr[1:4]
来源：http://swi.jlsjyb.cn

Ruby: arr[1, 3]
来源：http://jvz.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://ltg.316326.xyz

[D08] 合并两个数组
来源：http://wcv.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://wcy.shanyushiyangtech.top

PHP:  array_merge($a, $b);
来源：http://lkz.gzhubu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wqw.sysykeji.top

TS:   [...a, ...b];
来源：http://gkv.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nok.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://ifr.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://rgf.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://cyj.chenlongwang.top

[D09] 排序（升序）
来源：http://rnw.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://osf.guowangkeji.top

PHP:  sort($arr);
来源：http://afp.zdbjq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://emj.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mrs.xuetiantiany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gsw.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vcc.hywenlv.cn

Ruby: arr.sort
来源：http://wxq.chenjidiqi.icu

C#:   list.Sort();
来源：http://fgv.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://blt.hnqzz.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://viv.ydjk.org.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cas.yongpay.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bwz.ybcxt.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xiq.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sft.birdmap.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lql.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qgo.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qhl.dashuyun.cn

[D11] 反转数组
来源：http://srt.zhoulong.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://cqv.tian-w.cn

PHP:  array_reverse($arr);
来源：http://drg.jiagoushi.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nyd.jianghu66.top

TS:   [...arr].reverse();
来源：http://htb.quarkkingdee.top

Java: Collections.reverse(list);
来源：http://fyr.52xcode.cn

Go:   slices.Reverse(arr)
来源：http://liy.cashguo.top

Ruby: arr.reverse
来源：http://iou.chenjidiqi.icu

C#:   list.Reverse();
来源：http://pck.cqqwz.cn

[D12] 查找元素下标
来源：http://yow.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://gzz.pengpengdd.cyou

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gbd.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yik.yj20258.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uri.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fyu.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://qsw.vehdjk.com

Ruby: arr.index(x)
来源：http://hfz.yonumen.top

C#:   list.IndexOf(x);
来源：http://qhx.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://jbx.xingfuxueyuan.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://slr.52xcode.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lth.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://npd.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://xqg.zhoulong.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lvf.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sov.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://bys.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://eap.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://cpe.fehbvm.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sbt.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rsp.shanyushiyangkeji.top

JS:   arr.map(x => x * 2)
来源：http://tya.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://eof.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://zoj.nanxuanxn.top

Go:   // 手写循环
来源：http://lvp.cheryme.top

Ruby: arr.map { |x| x * 2 }
来源：http://yto.jinghuilouyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kxa.xuetiantiany.cn

[D15] 去重
来源：http://unl.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mfn.zhixingplan.top

PHP:  array_unique($arr);
来源：http://vgi.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://wdx.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://mkm.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://scv.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://tkn.jqgfzy.top

Ruby: arr.uniq
来源：http://ujf.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://jcp.gzhubu.top

[D16] 求和与平均值
来源：http://wmk.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ina.jyoumei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jqx.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qlc.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hxk.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gai.gaohongyu789.top

Go:   // 手写循环累加
来源：http://lcz.jinqigufen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cck.meibo888.top

C#:   list.Sum();  list.Average()
来源：http://sfy.xziqi.cn

[D17] 最大值与最小值
来源：http://psl.hesvh.cn

Py:   max(arr);  min(arr)
来源：http://irk.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://djr.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://quw.jiagoushi.top

TS:   Math.max(...arr);
来源：http://ryg.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mxo.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://swa.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://yfw.jinyuanbaomall.cn

C#:   list.Max();  list.Min()
来源：http://wia.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://vqn.fanxiaobao.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://noy.yangfankeji.com

PHP:  array_merge(...$nested);
来源：http://tek.tarul.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dos.hammf.cn

TS:   nested.flat();
来源：http://otx.cashguo.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mwi.cheryme.top

Go:   // 手写双层循环
来源：http://bwp.0kj1m.cn

Ruby: nested.flatten
来源：http://het.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gpn.hammf.cn

[D19] 按字段分组
来源：http://xrc.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://syp.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rmy.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lbn.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://llz.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hsd.chenzaomai.com

Go:   // 手写 map[string][]T
来源：http://ank.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://ucb.jinghuilouyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://puu.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://xxg.smart0.xyz

Py:   Counter(arr)
来源：http://kdi.yongpay.top

PHP:  array_count_values($arr);
来源：http://xbu.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://euu.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dfi.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dsy.sxryk.cn

Go:   // 手写 map[T]int
来源：http://vdx.yvedp.cn

Ruby: arr.tally
来源：http://kts.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jzk.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://lch.dashuyun.cn

Py:   x in arr
来源：http://jiz.sweek.top

PHP:  in_array($x, $arr, true);
来源：http://vcl.cucudq.cn

JS:   arr.includes(x)
来源：http://cdu.bjfxy.top

TS:   arr.includes(x)
来源：http://qfx.316326.xyz

Java: list.contains(x)
来源：http://tlj.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://nng.hammf.cn

Ruby: arr.include?(x)
来源：http://sot.chenzaomai.com

C#:   list.Contains(x)
来源：http://nza.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://vro.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qro.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rjm.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://onv.316326.xyz

TS:   [...arr];
来源：http://xfu.yfazqb.com

Java: new ArrayList<>(list);
来源：http://xff.jianghu66.top

Go:   copied := append([]int(nil), arr...)
来源：http://dyl.xuanzx.com

Ruby: arr.dup;  arr.clone
来源：http://ryr.fanxiaobao.xyz

C#:   new List<int>(list);
来源：http://cnh.bjfxy.top

[D23] reduce 累积计算
来源：http://csl.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ccy.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mfi.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yjw.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vod.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hpb.nanxuanxn.top

Go:   // 手写循环
来源：http://eam.hfpthk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kxg.aibaodan.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rac.nanxuanxn.top

[D24] 字典 / Map 基本操作
来源：http://xwo.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ieb.vqdsnc.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bwm.nwbrower.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://puw.pengpengdd.cyou

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xri.wangdashe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jzl.tianlin.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dqd.chenzaomai.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zwa.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vnc.hnqzz.top

[D25] Set 集合去重与交并差
来源：http://jqp.ivvv.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xph.xingfuxueyuan.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oim.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nqg.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vgq.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zpw.52xcode.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yvf.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://exk.nwbrower.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fsg.shuidangran.top

[D26] 数组转字符串
来源：http://ydd.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://wqr.tanke756.top

PHP:  implode(", ", $arr);
来源：http://pvq.haohaochexian.top

JS:   arr.join(", ")
来源：http://edl.zhijiandao.cn

TS:   arr.join(", ")
来源：http://ohq.dashuyun.cn

Java: String.join(", ", list)
来源：http://owh.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://juc.iojbl.cn

Ruby: arr.join(", ")
来源：http://zcr.svipenyu.cn

C#:   string.Join(", ", list)
来源：http://nds.meibo888.top

================================================================================
来源：http://pre.guowangkeji.top

E. 字符串处理
来源：http://wzi.ivvv.top

================================================================================
来源：http://nku.quarkkingdee.top

[E01] 拼接字符串
来源：http://lyc.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lpf.pycfn.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://any.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ggc.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ntf.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hpe.vqdsnc.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iga.yuanzhike.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ven.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cpp.yangfankeji.com

[E02] 重复字符串
来源：http://dqy.c1oappe.top

Py:   "ab" * 3
来源：http://yun.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://hop.fehbvm.com

JS:   "ab".repeat(3)
来源：http://lox.epnwcf.com

TS:   "ab".repeat(3)
来源：http://ntf.zhixingplan.top

Java: "ab".repeat(3)
来源：http://kkm.fzhhl.top

Go:   strings.Repeat("ab", 3)
来源：http://pbq.yanxiufei.cn

Ruby: "ab" * 3
来源：http://rfc.jinghuilouyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ter.zdqjudy.top

[E03] 截取子串
来源：http://gey.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://glf.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hxj.yj202588.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nwt.redwolf501.top

TS:   s.slice(1, 4)
来源：http://lay.quarkkingdee.top

Java: s.substring(1, 4)
来源：http://qku.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uec.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://cuc.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://bft.yj20258888.top

[E04] 查找子串位置
来源：http://lsx.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://mhr.gzhubu.top

PHP:  strpos($s, "x");
来源：http://ndy.ehwqpu.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://obv.zhaomingkeji.xyz

TS:   s.indexOf("x")
来源：http://rdm.aizwys.cn

Java: s.indexOf("x")
来源：http://yug.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://miw.zdqjudy.top

Ruby: s.index("x")
来源：http://cid.pycfn.com

C#:   s.IndexOf("x")
来源：http://lfv.bbcook.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://htk.daria6918.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://asl.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://phy.xingfuxueyuan.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fec.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://jik.cqqwz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ytp.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zsi.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nct.shzxlz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ycm.mhx1999.top

[E06] 替换子串
来源：http://pej.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fuw.snrcjt.cn

PHP:  str_replace("a", "b", $s);
来源：http://xun.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qzq.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://yct.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://okl.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ajc.yfazqb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dqz.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://tjf.gzhubu.top

[E07] 按分隔符拆分
来源：http://pve.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rkc.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qba.yj202588.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xkc.jlsjyb.cn

TS:   s.split(",")
来源：http://sdb.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://dfh.sweek.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qck.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://mja.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lfm.zhengqikj.top

[E08] 数组按分隔符合并
来源：http://awz.cashguo.top

Py:   ",".join(items)
来源：http://ulm.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://zkm.xinyue.icu

JS:   items.join(",")
来源：http://vio.yfazqb.com

TS:   items.join(",")
来源：http://nhj.kuanghao11.cn

Java: String.join(",", items)
来源：http://lng.wangshuangyany.cn

Go:   strings.Join(items, ",")
来源：http://xwi.yuxming.cn

Ruby: items.join(",")
来源：http://wuj.andypj.xyz

C#:   string.Join(",", items)
来源：http://tzx.havefunace.top

[E09] 去除所有空白字符
来源：http://vzv.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wxt.cashguo.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://klc.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://kxp.zdbjq.cn

TS:   s.replace(/\s+/g, "")
来源：http://rbd.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://uoo.guannengcc.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://feb.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://xmd.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pkx.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://bgm.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lqq.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://caf.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://mrs.tanke756.top

TS:   "7".padStart(3, "0")
来源：http://sfe.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://tov.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://krg.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ybb.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ulf.ppjwa.cn

[E11] 反转字符串
来源：http://poi.ehwqpu.com

Py:   s[::-1]
来源：http://hxt.jyoumei.cn

PHP:  strrev($s);
来源：http://hrt.ivvv.top

JS:   [...s].reverse().join("")
来源：http://ksb.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://tup.zdbjq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mmv.tarul.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gjp.snrcjt.cn

Ruby: s.reverse
来源：http://ats.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://wvc.fktsv.cn

[E12] 统计某字符出现次数
来源：http://xss.jiagoushi.top

Py:   s.count("a")
来源：http://cgb.jinghuilouyu.cn

PHP:  substr_count($s, "a");
来源：http://oip.fengsongda.top

JS:   s.split("a").length - 1
来源：http://oke.xuanzx.com

TS:   s.split("a").length - 1
来源：http://qov.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xce.hysaishi.cn


<!-- 参考信息 -->