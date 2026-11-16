代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://lmv.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dph.smart0.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://voo.daxiang520.top

[D06] 数组长度
来源：http://kug.zdqjudy.top

Py:   len(arr)
来源：http://bpw.ywan-chungtsiang.top

PHP:  count($arr);
来源：http://xoi.hesvh.cn

JS:   arr.length
来源：http://wsc.zhengqikj.top

TS:   arr.length
来源：http://ych.yuxming.cn

Java: list.size();
来源：http://tcq.kuanghao11.cn

Go:   len(arr)
来源：http://hru.cashguo.top

Ruby: arr.length; arr.size
来源：http://ujj.chenlongwang.top

C#:   list.Count;
来源：http://hxb.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://eqe.sjlbkw.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qqt.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rjo.vqdsnc.cn

JS:   arr.slice(1, 4);
来源：http://eqn.havefunace.top

TS:   arr.slice(1, 4);
来源：http://iwy.ehwqpu.com

Java: list.subList(1, 4);
来源：http://akd.fktsv.cn

Go:   arr[1:4]
来源：http://vep.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://wrv.yonumen.top

C#:   list.GetRange(1, 3);
来源：http://ubj.vqdsnc.cn

[D08] 合并两个数组
来源：http://voo.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://ogp.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://egl.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bbn.jinqigufen.top

TS:   [...a, ...b];
来源：http://ype.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ojf.bbcook.cn

Go:   append(a, b...)
来源：http://kqp.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://nak.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://uqa.cashguo.top

[D09] 排序（升序）
来源：http://enf.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://spx.ppjwa.cn

PHP:  sort($arr);
来源：http://nww.jinqigufen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lya.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://exl.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://gsa.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ear.ehwqpu.com

Ruby: arr.sort
来源：http://nsr.ivvv.top

C#:   list.Sort();
来源：http://dli.yonumen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wus.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lrk.xinyue.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sfs.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://brp.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tur.gotoacloud.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nwt.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ast.feifeiyinyue.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dez.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gfl.pycfn.com

[D11] 反转数组
来源：http://kte.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://asm.zhijiandao.cn

PHP:  array_reverse($arr);
来源：http://vzt.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vko.shuidangran.top

TS:   [...arr].reverse();
来源：http://jrk.uphjek.com

Java: Collections.reverse(list);
来源：http://wan.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://fff.epnwcf.com

Ruby: arr.reverse
来源：http://yzi.gogol.net.cn

C#:   list.Reverse();
来源：http://ucn.xuanzx.com

[D12] 查找元素下标
来源：http://pkv.zdqjudy.top

Py:   arr.index(x);  x in arr
来源：http://elz.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nqq.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jsz.birdmap.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dkm.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xcm.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://yzb.andypj.xyz

Ruby: arr.index(x)
来源：http://fzw.hnqzz.top

C#:   list.IndexOf(x);
来源：http://weg.hesvh.cn

[D13] 过滤（保留满足条件的）
来源：http://ans.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://znw.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qfj.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://jxw.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://uie.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://msq.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jbi.kuanghao11.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cnt.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://cml.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://cji.yvedp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iuf.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fqs.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://rjm.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://tfo.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://krb.cqqwz.cn

Go:   // 手写循环
来源：http://oql.0kj1m.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hbf.yvedp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rvl.wangdashe.top

[D15] 去重
来源：http://zir.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vkk.xziqi.cn

PHP:  array_unique($arr);
来源：http://ucd.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://clv.gzhubu.top

TS:   [...new Set(arr)]
来源：http://tam.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hpq.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://aqd.xinyue.icu

Ruby: arr.uniq
来源：http://smh.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://mch.vehdjk.com

[D16] 求和与平均值
来源：http://lqs.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vyz.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jan.fehbvm.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://voh.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xic.hfpthk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lmn.hysaishi.cn

Go:   // 手写循环累加
来源：http://ezv.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iwe.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://pba.yj20258888.top

[D17] 最大值与最小值
来源：http://ghj.birdmap.top

Py:   max(arr);  min(arr)
来源：http://jty.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://ftv.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lwv.cashguo.top

TS:   Math.max(...arr);
来源：http://mjg.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://das.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yvz.shanyushiyangkeji.top

Ruby: arr.max;  arr.min
来源：http://uux.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://nmt.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://xxv.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ciu.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://vph.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wjz.bjfxy.top

TS:   nested.flat();
来源：http://egy.dashuyun.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rpu.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://vpc.yanxiufei.cn

Ruby: nested.flatten
来源：http://eat.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dom.tanke756.top

[D19] 按字段分组
来源：http://hvr.pengpengdd.cyou

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tsq.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jsa.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kgz.tianlin.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://thj.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://abp.guowangkeji.top

Go:   // 手写 map[string][]T
来源：http://jzj.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lgz.redwolf501.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://avv.yj202588.top

[D20] 统计每个元素出现次数
来源：http://ibw.shzxlz.cn

Py:   Counter(arr)
来源：http://kil.cucudq.cn

PHP:  array_count_values($arr);
来源：http://wzx.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sff.fanxiaobao.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zzz.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jgc.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://ufi.zdqjudy.top

Ruby: arr.tally
来源：http://lol.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lle.guannengcc.top

[D21] 判断是否包含某元素
来源：http://vzb.sufxvd.cn

Py:   x in arr
来源：http://tyg.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://rmg.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://ahp.sysykeji.top

TS:   arr.includes(x)
来源：http://jot.daxiang520.top

Java: list.contains(x)
来源：http://cjn.shanyushiyangtech.top

Go:   slices.Contains(arr, x)
来源：http://zrd.gzhubu.top

Ruby: arr.include?(x)
来源：http://clu.dashuyun.cn

C#:   list.Contains(x)
来源：http://bav.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://emp.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ipi.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://epo.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://asc.ctjpmb.com

TS:   [...arr];
来源：http://mwr.fehbvm.com

Java: new ArrayList<>(list);
来源：http://nvx.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://ffe.andypj.xyz

Ruby: arr.dup;  arr.clone
来源：http://vhh.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://sln.zhiwuduotai.top

[D23] reduce 累积计算
来源：http://jhd.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jip.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hqo.jlsjyb.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qzs.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wdk.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://wxe.chenzaomai.com

Go:   // 手写循环
来源：http://esy.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vuv.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lfg.yanxiufei.cn

[D24] 字典 / Map 基本操作
来源：http://kev.yvedp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ifw.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ljp.guowangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ffa.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://urr.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rpl.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xio.fktsv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://moy.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tml.aizwys.cn

[D25] Set 集合去重与交并差
来源：http://dxq.fehbvm.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zfi.xuetiantiany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lgx.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iov.aizwys.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zbo.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://frl.ydzc1.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zog.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bxq.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tei.zhiwuduotai.top

[D26] 数组转字符串
来源：http://cen.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://rsq.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://khu.wangdashe.top

JS:   arr.join(", ")
来源：http://acs.zhongyouzk.top

TS:   arr.join(", ")
来源：http://frs.guannengcc.top

Java: String.join(", ", list)
来源：http://dkq.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://gem.daria6918.cn

Ruby: arr.join(", ")
来源：http://pdq.xinyue.icu

C#:   string.Join(", ", list)
来源：http://pff.hesvh.cn

================================================================================
来源：http://qjf.c1oappe.top

E. 字符串处理
来源：http://kkl.ivvv.top

================================================================================
来源：http://dxq.jianghu66.top

[E01] 拼接字符串
来源：http://txh.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wvf.zhongyouzk.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ppk.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hzd.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qnw.tanke756.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kco.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dqq.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tvd.jyoumei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://guv.pengpengdd.cyou

[E02] 重复字符串
来源：http://ezg.svipenyu.cn

Py:   "ab" * 3
来源：http://jpr.jinyuanbaomall.cn

PHP:  str_repeat("ab", 3);
来源：http://ovs.epnwcf.com

JS:   "ab".repeat(3)
来源：http://hyf.iojbl.cn

TS:   "ab".repeat(3)
来源：http://teg.tarul.cn

Java: "ab".repeat(3)
来源：http://esm.aizwys.cn

Go:   strings.Repeat("ab", 3)
来源：http://xmv.daria6918.cn

Ruby: "ab" * 3
来源：http://evo.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dcl.aizwys.cn

[E03] 截取子串
来源：http://wcs.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mag.hywenlv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bug.haohaochexian.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://guw.316326.xyz

TS:   s.slice(1, 4)
来源：http://lob.vehdjk.com

Java: s.substring(1, 4)
来源：http://gyc.xziqi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qkq.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://evx.bbcook.cn

C#:   s.Substring(1, 3)
来源：http://mjm.feifeiyinyue.top

[E04] 查找子串位置
来源：http://oca.316326.xyz

Py:   s.find("x");  s.index("x")
来源：http://nur.hongshengwenyu.top

PHP:  strpos($s, "x");
来源：http://gqx.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qjt.jyoumei.cn

TS:   s.indexOf("x")
来源：http://amb.gotoacloud.top

Java: s.indexOf("x")
来源：http://pcy.cashguo.top

Go:   strings.Index(s, "x")
来源：http://zei.cashguo.top

Ruby: s.index("x")
来源：http://pba.redwolf501.top

C#:   s.IndexOf("x")
来源：http://hna.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ikp.smart0.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fxs.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mnl.wangdashe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bdl.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vfs.jianghu66.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wjg.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ukf.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kpt.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rbw.daxiang520.top

[E06] 替换子串
来源：http://ccl.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wwv.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://tac.svipenyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gmg.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://mji.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iju.tian-w.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pyp.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yze.hammf.cn

C#:   s.Replace("a", "b")
来源：http://uwn.zdbjq.cn

[E07] 按分隔符拆分
来源：http://emf.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ebx.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://llm.pycfn.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://pwr.hysaishi.cn

TS:   s.split(",")
来源：http://oor.daxiang520.top

Java: s.split(",");  s.split("\\s+")
来源：http://uti.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kwh.feifeiyinyue.top

Ruby: s.split(",");  s.split
来源：http://tkr.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eny.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://btj.xinyue.icu

Py:   ",".join(items)
来源：http://puc.sysykeji.top

PHP:  implode(",", $items);
来源：http://los.hesvh.cn

JS:   items.join(",")
来源：http://dco.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://tsj.yongpay.top

Java: String.join(",", items)
来源：http://iqf.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://ppm.yueranfly.top

Ruby: items.join(",")
来源：http://phd.ydzc1.top

C#:   string.Join(",", items)
来源：http://zkn.jqgfzy.top

[E09] 去除所有空白字符
来源：http://xcx.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ucs.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dpx.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://vdq.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://rna.jqgufenzy.top

Java: s.replaceAll("\\s+", "")
来源：http://rjg.cheryme.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mum.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://wxi.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fhv.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://xqc.snrcjt.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nvf.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zmr.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://wiu.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://zrw.jinghuilouyu.cn

Java: String.format("%03d", 7)
来源：http://ouu.hnqzz.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://eax.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tnp.yangfankeji.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bqo.hesvh.cn

[E11] 反转字符串
来源：http://pmy.meibo888.top

Py:   s[::-1]
来源：http://zcl.guowangkeji.top

PHP:  strrev($s);
来源：http://nqw.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://kka.hnxiangtu.top

TS:   [...s].reverse().join("")
来源：http://dhi.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ivn.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ygt.cqqwz.cn

Ruby: s.reverse
来源：http://pub.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://vqh.chenlongwang.top

[E12] 统计某字符出现次数
来源：http://air.yfazqb.com

Py:   s.count("a")
来源：http://ofr.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://gtd.xylfe.cn

JS:   s.split("a").length - 1
来源：http://tlx.316326.xyz

TS:   s.split("a").length - 1
来源：http://ivp.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ehv.yanxiufei.cn


<!-- 参考信息 -->