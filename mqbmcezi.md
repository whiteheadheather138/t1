代发 wailian999

Java: list.size();
来源：http://uol.tarul.cn

Go:   len(arr)
来源：http://tey.svipenyu.cn

Ruby: arr.length; arr.size
来源：http://det.vqdsnc.cn

C#:   list.Count;
来源：http://dsh.wangshuangyany.cn

[D07] 切片 / 取子数组
来源：http://xag.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jsb.andypj.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://xnn.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://vky.jiagoushi.top

TS:   arr.slice(1, 4);
来源：http://gmu.birdmap.top

Java: list.subList(1, 4);
来源：http://bwv.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://wyi.gzhubu.top

Ruby: arr[1, 3]
来源：http://cdq.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://uve.daxiang520.top

[D08] 合并两个数组
来源：http://yaw.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://lya.xuetiantiany.cn

PHP:  array_merge($a, $b);
来源：http://ocp.hammf.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cmq.yangfankeji.com

TS:   [...a, ...b];
来源：http://fut.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ejo.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://dha.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://kxl.jqgufenzy.top

C#:   a.Concat(b).ToList()
来源：http://xtj.cheryme.top

[D09] 排序（升序）
来源：http://uxx.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://yof.aizwys.cn

PHP:  sort($arr);
来源：http://ynx.mhx1999.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wpf.shuidangran.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rsn.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://oas.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://usg.ppjwa.cn

Ruby: arr.sort
来源：http://vrw.smart0.xyz

C#:   list.Sort();
来源：http://gdb.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://btm.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bet.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hgj.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qye.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wmw.jqgfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wyr.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kot.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tlj.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jci.shzxlz.cn

[D11] 反转数组
来源：http://vwt.birdmap.top

Py:   arr[::-1];  arr.reverse()
来源：http://ahc.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://rdi.kuanghao11.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iki.fengsongda.top

TS:   [...arr].reverse();
来源：http://jjc.fanxiaobao.xyz

Java: Collections.reverse(list);
来源：http://eyt.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://wjn.hcnkem.com

Ruby: arr.reverse
来源：http://fxe.jqgfzy.top

C#:   list.Reverse();
来源：http://gwm.shzxlz.cn

[D12] 查找元素下标
来源：http://dsd.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://yyc.aizwys.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wtw.quarkkingdee.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nxh.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nxa.cheryme.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jgu.yonumen.top

Go:   slices.Index(arr, x)
来源：http://seb.ppjwa.cn

Ruby: arr.index(x)
来源：http://ufd.zycfv.cn

C#:   list.IndexOf(x);
来源：http://idj.yangfankeji.com

[D13] 过滤（保留满足条件的）
来源：http://cdd.wangshuangyany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zlh.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://byf.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://ajx.yueranfly.top

TS:   arr.filter(x => x > 3)
来源：http://gwf.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yfy.yonumen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vfo.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lty.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qgq.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://oqq.haohaochexian.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sir.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fkf.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://kge.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://ttt.zhoulong.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://xvo.zhoulong.xyz

Go:   // 手写循环
来源：http://vnx.cucudq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pto.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wjq.fehbvm.com

[D15] 去重
来源：http://iyy.jqgufenzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rbm.hnqzz.top

PHP:  array_unique($arr);
来源：http://kxd.shanyushiyangkeji.top

JS:   [...new Set(arr)]
来源：http://rqd.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://arq.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xpd.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://rlc.chenjidiqi.icu

Ruby: arr.uniq
来源：http://ult.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://xar.sjlbkw.cn

[D16] 求和与平均值
来源：http://lva.0kj1m.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lmg.xinyue.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nzz.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eai.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aby.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://utv.zhixingplan.top

Go:   // 手写循环累加
来源：http://rwl.zhaomingkeji.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ewh.cashguo.top

C#:   list.Sum();  list.Average()
来源：http://yqb.c1oappe.top

[D17] 最大值与最小值
来源：http://rek.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://ovy.yj20258.top

PHP:  max($arr);  min($arr);
来源：http://dri.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://msz.snrcjt.cn

TS:   Math.max(...arr);
来源：http://luf.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ufl.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lvv.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://gia.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://xjp.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://rwr.sjlbkw.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ybj.fengsongda.top

PHP:  array_merge(...$nested);
来源：http://qny.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jvd.ivvv.top

TS:   nested.flat();
来源：http://wum.haohaochexian.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iwc.ydzc1.top

Go:   // 手写双层循环
来源：http://ijm.hongshengwenyu.top

Ruby: nested.flatten
来源：http://twl.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kwd.zhengqikj.top

[D19] 按字段分组
来源：http://zhv.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fms.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mow.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vjo.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xqh.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rlo.jianghu66.top

Go:   // 手写 map[string][]T
来源：http://tgm.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ndk.sweek.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rcn.gaohongyu789.top

[D20] 统计每个元素出现次数
来源：http://glz.c1oappe.top

Py:   Counter(arr)
来源：http://gof.iojbl.cn

PHP:  array_count_values($arr);
来源：http://srz.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ejg.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cij.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://psb.meibo888.top

Go:   // 手写 map[T]int
来源：http://nci.iojbl.cn

Ruby: arr.tally
来源：http://zba.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xnh.sysykeji.top

[D21] 判断是否包含某元素
来源：http://dfc.sysykeji.top

Py:   x in arr
来源：http://jjs.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://lcx.chenlongwang.top

JS:   arr.includes(x)
来源：http://eiy.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://ulx.xuetiantiany.cn

Java: list.contains(x)
来源：http://huj.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://lzo.ehwqpu.com

Ruby: arr.include?(x)
来源：http://uot.hcnkem.com

C#:   list.Contains(x)
来源：http://wjm.shanyushiyangtech.top

[D22] 复制数组（避免共享引用）
来源：http://rfn.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zhz.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aeq.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yel.wangdashe.top

TS:   [...arr];
来源：http://aat.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://sqg.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://sva.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://swr.tanke756.top

C#:   new List<int>(list);
来源：http://qya.shangyingyoupin.top

[D23] reduce 累积计算
来源：http://xwg.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bul.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tqs.havefunace.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yvm.sjlbkw.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dgo.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hdc.meibo888.top

Go:   // 手写循环
来源：http://asg.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://raj.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lnm.c1oappe.top

[D24] 字典 / Map 基本操作
来源：http://awt.cdnleiting.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uja.shangyingyoupin.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pwy.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fjn.shuidangran.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ypo.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uee.yvedp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mfc.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://emg.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://htb.c1oappe.top

[D25] Set 集合去重与交并差
来源：http://zzs.yj202588.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://alo.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ajj.fanxiaobao.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xko.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://slk.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ikc.zhaomingkeji.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vrj.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://elb.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bge.sysykeji.top

[D26] 数组转字符串
来源：http://mru.xylfe.cn

Py:   ", ".join(map(str, arr))
来源：http://nly.fktsv.cn

PHP:  implode(", ", $arr);
来源：http://fbw.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://ouo.yuxming.cn

TS:   arr.join(", ")
来源：http://pcw.quarkkingdee.top

Java: String.join(", ", list)
来源：http://qzl.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://lqd.bbcook.cn

Ruby: arr.join(", ")
来源：http://vxg.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://rwc.jinqigufen.top

================================================================================
来源：http://dzi.yangfankeji.com

E. 字符串处理
来源：http://cqu.316326.xyz

================================================================================
来源：http://ics.cashguo.top

[E01] 拼接字符串
来源：http://vnz.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rdx.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cyu.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sid.epnwcf.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://djo.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://csu.yuanzhike.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qoo.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fap.52xcode.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dsj.zhiwuduotai.top

[E02] 重复字符串
来源：http://cwa.hywenlv.cn

Py:   "ab" * 3
来源：http://pnt.c1oappe.top

PHP:  str_repeat("ab", 3);
来源：http://uub.vehdjk.com

JS:   "ab".repeat(3)
来源：http://cxb.fengsongda.top

TS:   "ab".repeat(3)
来源：http://qyo.zycfv.cn

Java: "ab".repeat(3)
来源：http://vrr.bbcook.cn

Go:   strings.Repeat("ab", 3)
来源：http://utt.xingfuxueyuan.xyz

Ruby: "ab" * 3
来源：http://ljb.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://anu.redwolf501.top

[E03] 截取子串
来源：http://tvk.yuxming.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bnu.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rue.hnqzz.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pmx.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://glc.ybcxt.top

Java: s.substring(1, 4)
来源：http://inx.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lfx.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://yiw.nwbrower.top

C#:   s.Substring(1, 3)
来源：http://bzs.jianghu66.top

[E04] 查找子串位置
来源：http://iau.vqdsnc.cn

Py:   s.find("x");  s.index("x")
来源：http://klm.cqqwz.cn

PHP:  strpos($s, "x");
来源：http://gqn.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gnl.smart0.xyz

TS:   s.indexOf("x")
来源：http://dyc.jqgufenzy.top

Java: s.indexOf("x")
来源：http://wxf.sysykeji.top

Go:   strings.Index(s, "x")
来源：http://kff.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://qsp.yfazqb.com

C#:   s.IndexOf("x")
来源：http://rzr.haohaochexian.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vhf.wangshuangyany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lds.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wnr.daxiang520.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cky.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://pzp.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iay.gaohongyu789.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hui.dashuyun.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jtn.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://flq.mhx1999.top

[E06] 替换子串
来源：http://gvl.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zpu.daria6918.cn

PHP:  str_replace("a", "b", $s);
来源：http://jgc.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ulo.iojbl.cn

TS:   s.replaceAll("a", "b")
来源：http://hyn.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gdq.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dbq.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uhq.birdmap.top

C#:   s.Replace("a", "b")
来源：http://uds.sysykeji.top

[E07] 按分隔符拆分
来源：http://yit.andypj.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oei.9152youxi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uuu.nwbrower.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://iig.nanxuanxn.top

TS:   s.split(",")
来源：http://ogi.jqgfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://buy.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hdr.birdmap.top

Ruby: s.split(",");  s.split
来源：http://cnv.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zrj.cashguo.top

[E08] 数组按分隔符合并
来源：http://ria.jinqigfzy.top

Py:   ",".join(items)
来源：http://kda.zdbjq.cn

PHP:  implode(",", $items);
来源：http://bin.yueranfly.top

JS:   items.join(",")
来源：http://bwb.yfazqb.com

TS:   items.join(",")
来源：http://ijv.hcnkem.com

Java: String.join(",", items)
来源：http://xea.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://byz.redwolf501.top

Ruby: items.join(",")
来源：http://mmr.yfazqb.com

C#:   string.Join(",", items)
来源：http://gko.havefunace.top

[E09] 去除所有空白字符
来源：http://ewj.dianchejie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://usi.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://use.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://yrt.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://ipp.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://ews.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kcj.uphjek.com

Ruby: s.gsub(/\s+/, "")
来源：http://fxx.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hgo.andypj.xyz

[E10] 左侧补零 / 定长填充
来源：http://qoa.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://etj.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mdo.jqgufenzy.top

JS:   "7".padStart(3, "0")
来源：http://cow.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://vxl.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://jmd.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://caa.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mpc.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rzz.sufxvd.cn

[E11] 反转字符串
来源：http://nho.tanke756.top

Py:   s[::-1]
来源：http://aze.hysaishi.cn

PHP:  strrev($s);
来源：http://esd.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://vda.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://css.ybcxt.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xhu.tian-w.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wpt.zhixingplan.top

Ruby: s.reverse
来源：http://afz.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://kpk.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://ckc.ivvv.top

Py:   s.count("a")
来源：http://fap.jinghuilouyu.cn

PHP:  substr_count($s, "a");
来源：http://hga.fzhhl.top

JS:   s.split("a").length - 1
来源：http://lvu.hongshengwenyu.top

TS:   s.split("a").length - 1
来源：http://gli.yj20258.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zof.tarul.cn

Go:   strings.Count(s, "a")
来源：http://dcr.guowangkeji.top

Ruby: s.count("a")
来源：http://ylf.nwbrower.top

C#:   s.Count(c => c == 'a')
来源：http://shy.snrcjt.cn

[E13] 逐字符遍历
来源：http://gpj.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://kol.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xaa.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vdc.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dgf.ehwqpu.com


<!-- 参考信息 -->