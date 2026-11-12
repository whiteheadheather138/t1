代发 wailian999

[D07] 切片 / 取子数组
来源：http://lrm.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ouk.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lsy.zhaomingkeji.xyz

JS:   arr.slice(1, 4);
来源：http://gxm.snrcjt.cn

TS:   arr.slice(1, 4);
来源：http://xzg.hcnkem.com

Java: list.subList(1, 4);
来源：http://tfi.tanke756.top

Go:   arr[1:4]
来源：http://nnu.haohaochexian.top

Ruby: arr[1, 3]
来源：http://wbc.hnxiangtu.top

C#:   list.GetRange(1, 3);
来源：http://dof.ydzc1.top

[D08] 合并两个数组
来源：http://vgv.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://cta.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://pjt.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://prm.epnwcf.com

TS:   [...a, ...b];
来源：http://ior.316326.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tbj.52xcode.cn

Go:   append(a, b...)
来源：http://vej.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://qyw.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://tay.snrcjt.cn

[D09] 排序（升序）
来源：http://gmm.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://csl.redwolf501.top

PHP:  sort($arr);
来源：http://mir.xingfuxueyuan.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tut.ydzc1.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cqk.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://bor.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://etr.cheryme.top

Ruby: arr.sort
来源：http://cfs.xziqi.cn

C#:   list.Sort();
来源：http://ntv.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kgo.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jdd.uphjek.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vgo.aibaodan.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kvt.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bbj.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rmk.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bga.chenjidiqi.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dpi.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lcv.zhiwuduotai.top

[D11] 反转数组
来源：http://jvh.zhongyouzk.top

Py:   arr[::-1];  arr.reverse()
来源：http://nfl.shuidangran.top

PHP:  array_reverse($arr);
来源：http://xms.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zph.cashguo.top

TS:   [...arr].reverse();
来源：http://pfw.nanxinkj.top

Java: Collections.reverse(list);
来源：http://zzo.snrcjt.cn

Go:   slices.Reverse(arr)
来源：http://nyn.cqqwz.cn

Ruby: arr.reverse
来源：http://lur.xingfuxueyuan.xyz

C#:   list.Reverse();
来源：http://unn.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://rel.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://ubq.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yes.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://icc.redwolf501.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jam.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://guu.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://hns.sjlbkw.cn

Ruby: arr.index(x)
来源：http://lfy.tian-w.cn

C#:   list.IndexOf(x);
来源：http://dct.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://rjh.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yrf.yj202588.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vtz.jianghu66.top

JS:   arr.filter(x => x > 3)
来源：http://iky.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://lqg.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ufx.zhaomingkeji.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hrn.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://cty.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://xnh.aibaodan.cn

[D14] 映射转换（每个元素变形）
来源：http://njh.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qro.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ypc.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://aba.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://cnv.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://bwc.jyoumei.cn

Go:   // 手写循环
来源：http://kjf.yueranfly.top

Ruby: arr.map { |x| x * 2 }
来源：http://uba.zycfv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cpj.sxryk.cn

[D15] 去重
来源：http://ctt.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pkd.snrcjt.cn

PHP:  array_unique($arr);
来源：http://tir.sxryk.cn

JS:   [...new Set(arr)]
来源：http://ihf.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://jow.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qii.ybcxt.top

Go:   // 用 map[T]struct{} 手写
来源：http://ndy.fktsv.cn

Ruby: arr.uniq
来源：http://wqq.cashguo.top

C#:   list.Distinct().ToList()
来源：http://rub.jiagoushi.top

[D16] 求和与平均值
来源：http://ebx.sxryk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lqy.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://emr.hcnkem.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xgz.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tkf.zycfv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dsc.svipenyu.cn

Go:   // 手写循环累加
来源：http://yik.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fis.dashuyun.cn

C#:   list.Sum();  list.Average()
来源：http://cfa.xuetiantiany.cn

[D17] 最大值与最小值
来源：http://nrk.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://hbz.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://aci.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zaf.yj20258.top

TS:   Math.max(...arr);
来源：http://aft.tanke756.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rci.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sms.zhaomingkeji.xyz

Ruby: arr.max;  arr.min
来源：http://ude.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://cen.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://jed.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://umi.yanxiufei.cn

PHP:  array_merge(...$nested);
来源：http://otb.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ckn.jinqigufen.top

TS:   nested.flat();
来源：http://ixd.gzhubu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ins.guannengcc.top

Go:   // 手写双层循环
来源：http://mxb.cdnleiting.top

Ruby: nested.flatten
来源：http://ulf.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jqa.sxryk.cn

[D19] 按字段分组
来源：http://umm.yj202588.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ytb.zdbjq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qaa.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vnr.redwolf501.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rpr.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wja.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://fgl.jinqigufen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ggc.tianlin.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gnc.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://ygl.shuidangran.top

Py:   Counter(arr)
来源：http://eww.quarkkingdee.top

PHP:  array_count_values($arr);
来源：http://tok.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hlw.sweek.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dzh.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jxp.xingfuxueyuan.xyz

Go:   // 手写 map[T]int
来源：http://qwy.zhiwuduotai.top

Ruby: arr.tally
来源：http://qpk.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sxp.ybcxt.top

[D21] 判断是否包含某元素
来源：http://uxm.ywan-chungtsiang.top

Py:   x in arr
来源：http://inq.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://qmc.jiagoushi.top

JS:   arr.includes(x)
来源：http://reu.yuanzhike.top

TS:   arr.includes(x)
来源：http://akg.ybcxt.top

Java: list.contains(x)
来源：http://mze.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://blp.daxiang520.top

Ruby: arr.include?(x)
来源：http://pxr.chenzaomai.com

C#:   list.Contains(x)
来源：http://jhu.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://fpc.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hbz.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gol.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vtw.birdmap.top

TS:   [...arr];
来源：http://jpz.gzhubu.top

Java: new ArrayList<>(list);
来源：http://fgi.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yzp.yj20258888.top

Ruby: arr.dup;  arr.clone
来源：http://qjq.zdbjq.cn

C#:   new List<int>(list);
来源：http://yxc.chenzaomai.com

[D23] reduce 累积计算
来源：http://akr.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qja.jinqigfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mti.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sug.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ygj.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://icw.xinyue.icu

Go:   // 手写循环
来源：http://bly.nanxuanxn.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tut.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cvq.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://dcn.jinqigufen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aew.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jzf.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qzk.yvedp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mdd.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tnn.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://plm.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yxk.c1oappe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qhu.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://oxw.shanyushiyangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iko.ehwqpu.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aae.nanxinkj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nhx.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nlm.fehbvm.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oin.tianlin.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hgz.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bvg.yuanzhike.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jqr.0kj1m.cn

[D26] 数组转字符串
来源：http://xan.zhoulong.xyz

Py:   ", ".join(map(str, arr))
来源：http://nsq.xuetiantiany.cn

PHP:  implode(", ", $arr);
来源：http://qvx.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://pym.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://eto.aizwys.cn

Java: String.join(", ", list)
来源：http://ojl.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://foq.c1oappe.top

Ruby: arr.join(", ")
来源：http://jfx.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://sqc.fengsongda.top

================================================================================
来源：http://pkf.zhongyouzk.top

E. 字符串处理
来源：http://gwp.ehwqpu.com

================================================================================
来源：http://jxn.shangyingyoupin.top

[E01] 拼接字符串
来源：http://cqx.nanxuanxn.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://adg.yj20258888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ygd.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://euy.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://chh.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vsl.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dkc.zhiwuduotai.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xhh.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://znk.c1oappe.top

[E02] 重复字符串
来源：http://gry.smart0.xyz

Py:   "ab" * 3
来源：http://ean.guowangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://urc.bjfxy.top

JS:   "ab".repeat(3)
来源：http://hyx.dianchejie.cn

TS:   "ab".repeat(3)
来源：http://gwd.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://que.zhaomingkeji.xyz

Go:   strings.Repeat("ab", 3)
来源：http://zfd.sysykeji.top

Ruby: "ab" * 3
来源：http://xmm.ydzc1.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wci.fktsv.cn

[E03] 截取子串
来源：http://omp.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vqb.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oev.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jba.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://eeq.wangdashe.top

Java: s.substring(1, 4)
来源：http://qgs.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://anj.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://ycv.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://rfa.guowangkeji.top

[E04] 查找子串位置
来源：http://lkz.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://euw.mhx1999.top

PHP:  strpos($s, "x");
来源：http://tvp.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wxs.fehbvm.com

TS:   s.indexOf("x")
来源：http://agp.zhixingplan.top

Java: s.indexOf("x")
来源：http://rss.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://qrc.sweek.top

Ruby: s.index("x")
来源：http://ejw.fengsongda.top

C#:   s.IndexOf("x")
来源：http://shq.jinghuilouyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qau.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ivd.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wpl.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zur.sweek.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://oij.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ugl.mhx1999.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wuk.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gys.shanyushiyangtech.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jxd.jianghu66.top

[E06] 替换子串
来源：http://fad.zdbjq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://stu.shangyingyoupin.top

PHP:  str_replace("a", "b", $s);
来源：http://igr.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://amz.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://asm.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wnu.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ere.wangshuangyany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jgh.cucudq.cn

C#:   s.Replace("a", "b")
来源：http://dzv.uphjek.com

[E07] 按分隔符拆分
来源：http://qvu.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dqb.tian-w.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kcc.haohaochexian.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fai.chenzaomai.com

TS:   s.split(",")
来源：http://tsu.ybcxt.top

Java: s.split(",");  s.split("\\s+")
来源：http://mkr.shanyushiyangtech.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sdb.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://dsy.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eeh.xziqi.cn

[E08] 数组按分隔符合并
来源：http://vtj.zhixingplan.top

Py:   ",".join(items)
来源：http://bbo.xinyue.icu

PHP:  implode(",", $items);
来源：http://vit.ybcxt.top

JS:   items.join(",")
来源：http://jwx.jlsjyb.cn

TS:   items.join(",")
来源：http://dcx.tianlin.xyz

Java: String.join(",", items)
来源：http://exv.shangyingyoupin.top

Go:   strings.Join(items, ",")
来源：http://dqo.316326.xyz

Ruby: items.join(",")
来源：http://uxg.cheryme.top

C#:   string.Join(",", items)
来源：http://dwe.0kj1m.cn

[E09] 去除所有空白字符
来源：http://yia.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bem.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mtm.wangdashe.top

JS:   s.replace(/\s+/g, "")
来源：http://hzd.redwolf501.top

TS:   s.replace(/\s+/g, "")
来源：http://kdj.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://mkt.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zjg.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xzw.yonumen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xso.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://dac.gzhubu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jpf.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vze.shangyingyoupin.top

JS:   "7".padStart(3, "0")
来源：http://grj.smart0.xyz

TS:   "7".padStart(3, "0")
来源：http://tym.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://fev.chenlongwang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ccr.fzhhl.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://apu.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://spl.hysaishi.cn

[E11] 反转字符串
来源：http://vtu.yj20258888.top

Py:   s[::-1]
来源：http://zgt.sufxvd.cn

PHP:  strrev($s);
来源：http://cjf.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://iln.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://lyl.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zza.cucudq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://glr.jianghu66.top

Ruby: s.reverse
来源：http://hxu.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://nki.hcnkem.com

[E12] 统计某字符出现次数
来源：http://zrg.cucudq.cn

Py:   s.count("a")
来源：http://njy.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://led.xylfe.cn

JS:   s.split("a").length - 1
来源：http://urb.cashguo.top

TS:   s.split("a").length - 1
来源：http://yvf.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://txh.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://knk.tian-w.cn

Ruby: s.count("a")
来源：http://phx.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://hfi.yangfankeji.com

[E13] 逐字符遍历
来源：http://caf.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://gpa.cheryme.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ycz.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://bxc.aibaodan.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://trn.uphjek.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xqo.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jti.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://mvq.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wlx.hnxiangtu.top


<!-- 参考信息 -->