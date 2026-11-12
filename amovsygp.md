代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fiy.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rcc.zdqjudy.top

TS:   arr[0]; arr.at(-1);
来源：http://vgf.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://pvj.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://vby.xziqi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ijz.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rhf.jqgfzy.top

[D06] 数组长度
来源：http://vnb.fehbvm.com

Py:   len(arr)
来源：http://fpe.gaohongyu789.top

PHP:  count($arr);
来源：http://qqs.cqqwz.cn

JS:   arr.length
来源：http://grj.pycfn.com

TS:   arr.length
来源：http://luk.shzxlz.cn

Java: list.size();
来源：http://jtp.ivvv.top

Go:   len(arr)
来源：http://nkj.yuxming.cn

Ruby: arr.length; arr.size
来源：http://jga.ywan-chungtsiang.top

C#:   list.Count;
来源：http://itm.wangshuangyany.cn

[D07] 切片 / 取子数组
来源：http://fnj.hongshengwenyu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ngy.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://rul.cashguo.top

JS:   arr.slice(1, 4);
来源：http://ugb.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://swo.yj202588.top

Java: list.subList(1, 4);
来源：http://aul.9152youxi.cn

Go:   arr[1:4]
来源：http://pya.jianghu66.top

Ruby: arr[1, 3]
来源：http://rze.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://tkm.fengsongda.top

[D08] 合并两个数组
来源：http://qjs.guowangkeji.top

Py:   a + b;  a.extend(b)
来源：http://xiz.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://nxy.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zjn.zdqjudy.top

TS:   [...a, ...b];
来源：http://zkm.kuanghao11.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fyp.redwolf501.top

Go:   append(a, b...)
来源：http://gld.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://evl.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://yyp.aizwys.cn

[D09] 排序（升序）
来源：http://isl.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://owr.9152youxi.cn

PHP:  sort($arr);
来源：http://jdy.fanxiaobao.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ztr.fanxiaobao.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://gmo.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://yfo.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gkv.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://ydi.zdbjq.cn

C#:   list.Sort();
来源：http://yum.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://oly.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qml.cqqwz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mzm.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zip.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oar.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://klv.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sqi.cucudq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kwh.smart0.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bbt.quarkkingdee.top

[D11] 反转数组
来源：http://lev.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lpe.mhx1999.top

PHP:  array_reverse($arr);
来源：http://ctn.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nra.hammf.cn

TS:   [...arr].reverse();
来源：http://nxz.jinqigufen.top

Java: Collections.reverse(list);
来源：http://mgr.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://mgw.jiagoushi.top

Ruby: arr.reverse
来源：http://bkq.dianchejie.cn

C#:   list.Reverse();
来源：http://esv.chenzaomai.com

[D12] 查找元素下标
来源：http://eax.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://llo.pengpengdd.cyou

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ivq.hongshengwenyu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qcq.uphjek.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://csd.cashguo.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oya.uphjek.com

Go:   slices.Index(arr, x)
来源：http://amv.ydzc1.top

Ruby: arr.index(x)
来源：http://qmc.jinqigufen.top

C#:   list.IndexOf(x);
来源：http://yum.ehwqpu.com

[D13] 过滤（保留满足条件的）
来源：http://pve.jinyuanbaomall.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zgq.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ylt.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://fcq.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://txx.wangshuangyany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xph.aibaodan.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://srx.xuetiantiany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lag.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tfo.zhongyouzk.top

[D14] 映射转换（每个元素变形）
来源：http://hwv.0kj1m.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sqp.hesvh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xhh.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://gxz.zhoulong.xyz

TS:   arr.map(x => x * 2)
来源：http://nob.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ofj.cucudq.cn

Go:   // 手写循环
来源：http://zuz.hongshengwenyu.top

Ruby: arr.map { |x| x * 2 }
来源：http://feo.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zvd.shangyingyoupin.top

[D15] 去重
来源：http://ymt.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ixw.jqgfzy.top

PHP:  array_unique($arr);
来源：http://bct.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://nag.xuanzx.com

TS:   [...new Set(arr)]
来源：http://bwp.fktsv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ffq.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zsf.birdmap.top

Ruby: arr.uniq
来源：http://rzl.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://syh.hongshengwenyu.top

[D16] 求和与平均值
来源：http://odd.ydzc1.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fzg.shangyingyoupin.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qvf.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qsp.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mkl.ppjwa.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qee.nanxuanxn.top

Go:   // 手写循环累加
来源：http://mjn.xinyue.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zjp.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://ggr.sweek.top

[D17] 最大值与最小值
来源：http://jar.xingfuxueyuan.xyz

Py:   max(arr);  min(arr)
来源：http://eyx.cdnleiting.top

PHP:  max($arr);  min($arr);
来源：http://ywp.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fwo.bjfxy.top

TS:   Math.max(...arr);
来源：http://bhl.hnxiangtu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nug.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hgj.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://tbu.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://inp.yj202588.top

[D18] 扁平化嵌套数组
来源：http://mvg.sweek.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mat.yonumen.top

PHP:  array_merge(...$nested);
来源：http://czo.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jai.daxiang520.top

TS:   nested.flat();
来源：http://kku.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kcr.hywenlv.cn

Go:   // 手写双层循环
来源：http://fhv.sufxvd.cn

Ruby: nested.flatten
来源：http://xjw.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iud.ctjpmb.com

[D19] 按字段分组
来源：http://gbl.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://igi.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jro.jinyuanbaomall.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yje.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rbv.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sxf.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://lyp.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hkl.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oqs.cqqwz.cn

[D20] 统计每个元素出现次数
来源：http://rpf.hesvh.cn

Py:   Counter(arr)
来源：http://wsw.kuanghao11.cn

PHP:  array_count_values($arr);
来源：http://ahy.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ctl.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jyc.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zkz.yanxiufei.cn

Go:   // 手写 map[T]int
来源：http://nfb.hcnkem.com

Ruby: arr.tally
来源：http://qvf.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qoe.jqgfzy.top

[D21] 判断是否包含某元素
来源：http://mhc.haohaochexian.top

Py:   x in arr
来源：http://igc.kuanghao11.cn

PHP:  in_array($x, $arr, true);
来源：http://ppa.52xcode.cn

JS:   arr.includes(x)
来源：http://ixk.redwolf501.top

TS:   arr.includes(x)
来源：http://mwj.sufxvd.cn

Java: list.contains(x)
来源：http://dbz.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://pvf.jiagoushi.top

Ruby: arr.include?(x)
来源：http://ove.zhoulong.xyz

C#:   list.Contains(x)
来源：http://tkq.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://ish.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cws.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bwv.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nwb.shangyingyoupin.top

TS:   [...arr];
来源：http://opy.yonumen.top

Java: new ArrayList<>(list);
来源：http://elx.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://xdu.mhx1999.top

Ruby: arr.dup;  arr.clone
来源：http://sjx.xylfe.cn

C#:   new List<int>(list);
来源：http://ile.shangyingyoupin.top

[D23] reduce 累积计算
来源：http://jsm.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bvp.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iyl.iojbl.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lfe.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aqk.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://rxs.xylfe.cn

Go:   // 手写循环
来源：http://ydt.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bai.jyoumei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ysa.snrcjt.cn

[D24] 字典 / Map 基本操作
来源：http://ufp.fzhhl.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mar.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sml.birdmap.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lga.iojbl.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zyv.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bcc.ybcxt.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rmb.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bxq.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eqy.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://ckz.feifeiyinyue.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jpv.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lsr.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mlv.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ote.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hxn.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aoi.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wil.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cvh.hammf.cn

[D26] 数组转字符串
来源：http://lyg.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://jwo.hcnkem.com

PHP:  implode(", ", $arr);
来源：http://vyv.hfpthk.cn

JS:   arr.join(", ")
来源：http://rmi.yuanzhike.top

TS:   arr.join(", ")
来源：http://hry.ydzc1.top

Java: String.join(", ", list)
来源：http://rsp.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://bzg.hnqzz.top

Ruby: arr.join(", ")
来源：http://zjs.52xcode.cn

C#:   string.Join(", ", list)
来源：http://jhp.hywenlv.cn

================================================================================
来源：http://nsp.yuxming.cn

E. 字符串处理
来源：http://bhz.jianghu66.top

================================================================================
来源：http://ftv.zdqjudy.top

[E01] 拼接字符串
来源：http://jnr.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jjo.zhongyouzk.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jbd.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mup.zhaomingkeji.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nct.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ihi.guannengcc.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zxx.zhixingplan.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jhp.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gex.yvedp.cn

[E02] 重复字符串
来源：http://vbs.kuanghao11.cn

Py:   "ab" * 3
来源：http://hek.jinqigfzy.top

PHP:  str_repeat("ab", 3);
来源：http://ods.sxryk.cn

JS:   "ab".repeat(3)
来源：http://fyb.fzhhl.top

TS:   "ab".repeat(3)
来源：http://iib.bjfxy.top

Java: "ab".repeat(3)
来源：http://eov.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://bpn.yueranfly.top

Ruby: "ab" * 3
来源：http://hkr.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://krk.jqgufenzy.top

[E03] 截取子串
来源：http://zsn.yuxming.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uzj.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lkb.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ajp.cashguo.top

TS:   s.slice(1, 4)
来源：http://ewe.zhengqikj.top

Java: s.substring(1, 4)
来源：http://imx.316326.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gms.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hvf.jianghu66.top

C#:   s.Substring(1, 3)
来源：http://uci.xuetiantiany.cn

[E04] 查找子串位置
来源：http://pke.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://bqv.dashuyun.cn

PHP:  strpos($s, "x");
来源：http://rge.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rnq.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://xvz.jyoumei.cn

Java: s.indexOf("x")
来源：http://wcf.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://ehq.hongshengwenyu.top

Ruby: s.index("x")
来源：http://lpm.uphjek.com

C#:   s.IndexOf("x")
来源：http://smi.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mhw.hammf.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fov.shuidangran.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lzl.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rec.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://ufa.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ufc.zhoulong.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nou.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kho.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jwh.52xcode.cn

[E06] 替换子串
来源：http://mwb.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wbf.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://epe.yvedp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://umg.yvedp.cn

TS:   s.replaceAll("a", "b")
来源：http://xvb.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://npb.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hcf.haohaochexian.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gih.sjlbkw.cn

C#:   s.Replace("a", "b")
来源：http://icf.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://ujw.hammf.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bas.tanke756.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rep.hammf.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iyc.jqgufenzy.top

TS:   s.split(",")
来源：http://njq.zycfv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qrs.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://msf.fktsv.cn

Ruby: s.split(",");  s.split
来源：http://gqh.52xcode.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jfq.dianchejie.cn

[E08] 数组按分隔符合并
来源：http://hnv.mhx1999.top

Py:   ",".join(items)
来源：http://jlw.haohaochexian.top

PHP:  implode(",", $items);
来源：http://bhz.jiagoushi.top

JS:   items.join(",")
来源：http://qwv.chenlongwang.top

TS:   items.join(",")
来源：http://bjl.cdnleiting.top

Java: String.join(",", items)
来源：http://euj.sufxvd.cn

Go:   strings.Join(items, ",")
来源：http://lfv.epnwcf.com

Ruby: items.join(",")
来源：http://klw.cucudq.cn

C#:   string.Join(",", items)
来源：http://cho.daxiang520.top

[E09] 去除所有空白字符
来源：http://efm.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ony.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lis.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://hgp.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://jxd.kuanghao11.cn

Java: s.replaceAll("\\s+", "")
来源：http://txh.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nnp.nanxuanxn.top

Ruby: s.gsub(/\s+/, "")
来源：http://rib.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cbu.xuanzx.com

[E10] 左侧补零 / 定长填充
来源：http://jfn.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cdy.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sek.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://fzd.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://hbo.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://vnj.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://eih.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eoo.yuanzhike.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rso.yanxiufei.cn

[E11] 反转字符串
来源：http://elx.hywenlv.cn

Py:   s[::-1]
来源：http://pln.uphjek.com

PHP:  strrev($s);
来源：http://eum.tarul.cn

JS:   [...s].reverse().join("")
来源：http://gec.tanke756.top

TS:   [...s].reverse().join("")
来源：http://phe.ybcxt.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cpz.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zpn.fktsv.cn

Ruby: s.reverse
来源：http://nfe.uphjek.com

C#:   new string(s.Reverse().ToArray())
来源：http://pok.sweek.top

[E12] 统计某字符出现次数
来源：http://uaj.kuanghao11.cn

Py:   s.count("a")
来源：http://xzg.gaohongyu789.top


<!-- 参考信息 -->