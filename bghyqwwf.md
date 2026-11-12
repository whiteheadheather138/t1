代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eqq.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://odb.zhoulong.xyz

TS:   arr[0]; arr.at(-1);
来源：http://uiu.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://yny.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://fbk.jqgfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ceq.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zjb.jiagoushi.top

[D06] 数组长度
来源：http://wut.vqdsnc.cn

Py:   len(arr)
来源：http://gdh.sufxvd.cn

PHP:  count($arr);
来源：http://dyo.ybcxt.top

JS:   arr.length
来源：http://fxk.shangyingyoupin.top

TS:   arr.length
来源：http://jbc.guannengcc.top

Java: list.size();
来源：http://vow.shanyushiyangtech.top

Go:   len(arr)
来源：http://pyr.hnqzz.top

Ruby: arr.length; arr.size
来源：http://ebr.cheryme.top

C#:   list.Count;
来源：http://zix.hnqzz.top

[D07] 切片 / 取子数组
来源：http://isb.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ysb.cheryme.top

PHP:  array_slice($arr, 1, 3);
来源：http://wow.bjfxy.top

JS:   arr.slice(1, 4);
来源：http://zzx.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://kwy.jianghu66.top

Java: list.subList(1, 4);
来源：http://xwe.wangshuangyany.cn

Go:   arr[1:4]
来源：http://gll.epnwcf.com

Ruby: arr[1, 3]
来源：http://ixw.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://uyd.316326.xyz

[D08] 合并两个数组
来源：http://edx.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://uck.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://wft.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ihu.gogol.net.cn

TS:   [...a, ...b];
来源：http://egz.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rku.cqqwz.cn

Go:   append(a, b...)
来源：http://tiu.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://dpo.vqdsnc.cn

C#:   a.Concat(b).ToList()
来源：http://pve.chenzaomai.com

[D09] 排序（升序）
来源：http://xlw.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://mlb.yuanzhike.top

PHP:  sort($arr);
来源：http://bsq.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zdu.uphjek.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://vsy.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://slh.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xid.yuxming.cn

Ruby: arr.sort
来源：http://bul.zhijiandao.cn

C#:   list.Sort();
来源：http://zwb.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tvz.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jdo.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gxd.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://btl.mhx1999.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wsk.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rjo.hesvh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gua.chenjidiqi.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lvk.hywenlv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zgk.yj20258.top

[D11] 反转数组
来源：http://mif.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://ksj.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://wdv.hywenlv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wdx.fengsongda.top

TS:   [...arr].reverse();
来源：http://ntq.meibo888.top

Java: Collections.reverse(list);
来源：http://hea.cheryme.top

Go:   slices.Reverse(arr)
来源：http://dwb.bbcook.cn

Ruby: arr.reverse
来源：http://kxx.jyoumei.cn

C#:   list.Reverse();
来源：http://mul.tanke756.top

[D12] 查找元素下标
来源：http://bls.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://wtz.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ejy.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ntx.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gth.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ujq.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://cja.xziqi.cn

Ruby: arr.index(x)
来源：http://qyu.zdbjq.cn

C#:   list.IndexOf(x);
来源：http://tqp.ehwqpu.com

[D13] 过滤（保留满足条件的）
来源：http://kfu.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jzo.jiagoushi.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vdc.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://xai.shangyingyoupin.top

TS:   arr.filter(x => x > 3)
来源：http://zdr.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pgu.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xxy.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://vct.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://boy.chenjidiqi.icu

[D14] 映射转换（每个元素变形）
来源：http://rfz.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qsg.sweek.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fjk.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://fzk.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://tac.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://oru.uphjek.com

Go:   // 手写循环
来源：http://jbp.tarul.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hbq.shangyingyoupin.top

C#:   list.Select(x => x * 2).ToList()
来源：http://llj.cheryme.top

[D15] 去重
来源：http://etp.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hxr.fzhhl.top

PHP:  array_unique($arr);
来源：http://oho.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://xit.mhx1999.top

TS:   [...new Set(arr)]
来源：http://xnx.tanke756.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wcb.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ndx.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://tao.ehwqpu.com

C#:   list.Distinct().ToList()
来源：http://tun.sufxvd.cn

[D16] 求和与平均值
来源：http://vqt.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ypf.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://obf.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eoe.sxryk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yiy.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iiz.gaohongyu789.top

Go:   // 手写循环累加
来源：http://huj.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zkx.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://pkf.xuetiantiany.cn

[D17] 最大值与最小值
来源：http://off.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://wcj.fanxiaobao.xyz

PHP:  max($arr);  min($arr);
来源：http://raq.zycfv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://erv.dianchejie.cn

TS:   Math.max(...arr);
来源：http://kvh.hfpthk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uuk.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://izz.tarul.cn

Ruby: arr.max;  arr.min
来源：http://syl.bbcook.cn

C#:   list.Max();  list.Min()
来源：http://cbb.yj20258888.top

[D18] 扁平化嵌套数组
来源：http://dfg.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mcw.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://ply.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tyu.chenjidiqi.icu

TS:   nested.flat();
来源：http://wak.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pqk.ehwqpu.com

Go:   // 手写双层循环
来源：http://qex.chenlongwang.top

Ruby: nested.flatten
来源：http://xrh.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rig.tianlin.xyz

[D19] 按字段分组
来源：http://pkn.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qju.hnxiangtu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hvf.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ejs.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uic.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cqk.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://hss.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ewp.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ypk.gotoacloud.top

[D20] 统计每个元素出现次数
来源：http://jlr.meibo888.top

Py:   Counter(arr)
来源：http://lmn.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://ebd.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tqa.jqgfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zwr.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xhe.tanke756.top

Go:   // 手写 map[T]int
来源：http://lko.gzhubu.top

Ruby: arr.tally
来源：http://qly.yj20258888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lgk.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://yic.ywan-chungtsiang.top

Py:   x in arr
来源：http://hxo.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://fue.jianghu66.top

JS:   arr.includes(x)
来源：http://isx.hnxiangtu.top

TS:   arr.includes(x)
来源：http://oyz.zhongyouzk.top

Java: list.contains(x)
来源：http://jhl.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://zyv.gogol.net.cn

Ruby: arr.include?(x)
来源：http://een.hnqzz.top

C#:   list.Contains(x)
来源：http://jhv.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://fgr.yj20258888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lrd.cqqwz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://flm.sxryk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jnn.jinghuilouyu.cn

TS:   [...arr];
来源：http://enw.yj20258888.top

Java: new ArrayList<>(list);
来源：http://lae.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://wzo.ybcxt.top

Ruby: arr.dup;  arr.clone
来源：http://udm.aibaodan.cn

C#:   new List<int>(list);
来源：http://bap.iojbl.cn

[D23] reduce 累积计算
来源：http://cox.sweek.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hup.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ppm.yonumen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lir.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hjz.zhijiandao.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dpz.jinghuilouyu.cn

Go:   // 手写循环
来源：http://ikx.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bzh.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pmv.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://kmk.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wmq.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ble.cqqwz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fqj.ywan-chungtsiang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hxq.sjlbkw.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://smv.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gcr.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://heq.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bnb.yuanzhike.top

[D25] Set 集合去重与交并差
来源：http://uxx.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aks.hammf.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lvy.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zwp.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vjg.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://skf.hfpthk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cjx.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dzh.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xtf.zhongyouzk.top

[D26] 数组转字符串
来源：http://hfy.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://oee.uphjek.com

PHP:  implode(", ", $arr);
来源：http://uei.chenzaomai.com

JS:   arr.join(", ")
来源：http://miu.fzhhl.top

TS:   arr.join(", ")
来源：http://tbp.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://ofy.iojbl.cn

Go:   strings.Join(strs, ", ")
来源：http://xwu.jqgfzy.top

Ruby: arr.join(", ")
来源：http://hxd.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://pmu.yueranfly.top

================================================================================
来源：http://tll.xziqi.cn

E. 字符串处理
来源：http://cho.daria6918.cn

================================================================================
来源：http://rgp.shanyushiyangtech.top

[E01] 拼接字符串
来源：http://elb.pycfn.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kly.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nuf.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://njz.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vdf.jqgufenzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://srp.zhixingplan.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aax.hnxiangtu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://doz.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rqi.jianghu66.top

[E02] 重复字符串
来源：http://yzh.jianghu66.top

Py:   "ab" * 3
来源：http://byn.cqqwz.cn

PHP:  str_repeat("ab", 3);
来源：http://grh.meibo888.top

JS:   "ab".repeat(3)
来源：http://xfv.chenlongwang.top

TS:   "ab".repeat(3)
来源：http://sdl.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://qmz.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://ixo.yuanzhike.top

Ruby: "ab" * 3
来源：http://vgc.cdnleiting.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yzk.vqdsnc.cn

[E03] 截取子串
来源：http://dxl.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://maa.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qfy.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zaj.ydzc1.top

TS:   s.slice(1, 4)
来源：http://rah.nwbrower.top

Java: s.substring(1, 4)
来源：http://vun.zhoulong.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jku.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://yjh.ehwqpu.com

C#:   s.Substring(1, 3)
来源：http://jgw.316326.xyz

[E04] 查找子串位置
来源：http://wij.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://akm.nwbrower.top

PHP:  strpos($s, "x");
来源：http://vlb.snrcjt.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qjr.hcnkem.com

TS:   s.indexOf("x")
来源：http://asy.yueranfly.top

Java: s.indexOf("x")
来源：http://gmu.pengpengdd.cyou

Go:   strings.Index(s, "x")
来源：http://ocb.ctjpmb.com

Ruby: s.index("x")
来源：http://hph.tian-w.cn

C#:   s.IndexOf("x")
来源：http://nww.wangshuangyany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gxz.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hkl.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nxn.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mgg.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bau.hywenlv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ccx.sysykeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ree.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jgy.yuanzhike.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dms.yvedp.cn

[E06] 替换子串
来源：http://imx.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fbt.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://xsm.ivvv.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hch.shanyushiyangtech.top

TS:   s.replaceAll("a", "b")
来源：http://vzp.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ckl.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xzl.yangfankeji.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://arn.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://ccs.yongpay.top

[E07] 按分隔符拆分
来源：http://wxy.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rnl.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lit.quarkkingdee.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nhg.cdnleiting.top

TS:   s.split(",")
来源：http://iar.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://crk.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xfl.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://smy.shanyushiyangtech.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://erc.bbcook.cn

[E08] 数组按分隔符合并
来源：http://rcc.yangfankeji.com

Py:   ",".join(items)
来源：http://oak.epnwcf.com

PHP:  implode(",", $items);
来源：http://ngl.tarul.cn

JS:   items.join(",")
来源：http://trp.zhoulong.xyz

TS:   items.join(",")
来源：http://csm.birdmap.top

Java: String.join(",", items)
来源：http://egg.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://gvg.ppjwa.cn

Ruby: items.join(",")
来源：http://nmg.pycfn.com

C#:   string.Join(",", items)
来源：http://zyw.yj20258888.top

[E09] 去除所有空白字符
来源：http://xvs.dianchejie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iyt.hcnkem.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://csj.meibo888.top

JS:   s.replace(/\s+/g, "")
来源：http://uwa.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://ktw.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://xsl.zhiwuduotai.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://umt.yj20258888.top

Ruby: s.gsub(/\s+/, "")
来源：http://ten.sysykeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://usb.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://pnf.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eyy.zhoulong.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://twv.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://msi.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://ikc.yonumen.top

Java: String.format("%03d", 7)
来源：http://gei.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ghw.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://toj.sweek.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://apj.yonumen.top

[E11] 反转字符串
来源：http://xkj.snrcjt.cn

Py:   s[::-1]
来源：http://qyf.daxiang520.top

PHP:  strrev($s);
来源：http://shw.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://ery.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://csz.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://czp.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://xpe.hesvh.cn

Ruby: s.reverse
来源：http://xyq.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ulb.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://oiw.jqgufenzy.top

Py:   s.count("a")
来源：http://vcd.xinyue.icu


<!-- 参考信息 -->