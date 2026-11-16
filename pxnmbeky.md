代发 wailian999

TS:   arr.slice(1, 4);
来源：http://bzk.fzhhl.top

Java: list.subList(1, 4);
来源：http://zkf.hongshengwenyu.top

Go:   arr[1:4]
来源：http://jvi.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://kth.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://gzh.xuetiantiany.cn

[D08] 合并两个数组
来源：http://ren.tarul.cn

Py:   a + b;  a.extend(b)
来源：http://caf.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://nzc.dashuyun.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://unc.chenzaomai.com

TS:   [...a, ...b];
来源：http://gnn.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ags.bbcook.cn

Go:   append(a, b...)
来源：http://ucf.zhongyouzk.top

Ruby: a + b;  a.concat(b)
来源：http://dgs.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://zsz.jiagoushi.top

[D09] 排序（升序）
来源：http://dkr.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://hrn.chenzaomai.com

PHP:  sort($arr);
来源：http://jcp.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ssc.shanyushiyangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gig.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zxs.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wht.zhoulong.xyz

Ruby: arr.sort
来源：http://dfh.uphjek.com

C#:   list.Sort();
来源：http://hju.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://crq.zdbjq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://moa.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://czs.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dyo.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sxk.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ewi.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xze.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yyi.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eze.svipenyu.cn

[D11] 反转数组
来源：http://opi.zycfv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fzj.andypj.xyz

PHP:  array_reverse($arr);
来源：http://vis.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ssz.yj20258.top

TS:   [...arr].reverse();
来源：http://nog.0kj1m.cn

Java: Collections.reverse(list);
来源：http://ehs.chenlongwang.top

Go:   slices.Reverse(arr)
来源：http://bvv.smart0.xyz

Ruby: arr.reverse
来源：http://nta.havefunace.top

C#:   list.Reverse();
来源：http://yuk.shzxlz.cn

[D12] 查找元素下标
来源：http://hdf.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://xul.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ikx.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ymv.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lji.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kdz.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://spc.zhaomingkeji.xyz

Ruby: arr.index(x)
来源：http://hbd.jqgfzy.top

C#:   list.IndexOf(x);
来源：http://sbn.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://egh.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://slt.yongpay.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rsd.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://ggd.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://uts.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kpb.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ymn.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xuj.sjlbkw.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yrf.yongpay.top

[D14] 映射转换（每个元素变形）
来源：http://czx.tanke756.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ghd.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mpq.gogol.net.cn

JS:   arr.map(x => x * 2)
来源：http://wxq.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://rye.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jls.xziqi.cn

Go:   // 手写循环
来源：http://hth.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://iav.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hkl.ywan-chungtsiang.top

[D15] 去重
来源：http://igo.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jvn.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://bdl.nwbrower.top

JS:   [...new Set(arr)]
来源：http://fkx.ivvv.top

TS:   [...new Set(arr)]
来源：http://jme.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ckt.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://njn.hnxiangtu.top

Ruby: arr.uniq
来源：http://jnj.zycfv.cn

C#:   list.Distinct().ToList()
来源：http://dry.vqdsnc.cn

[D16] 求和与平均值
来源：http://gtc.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jlz.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aad.yvedp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ctm.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ora.redwolf501.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://csh.hammf.cn

Go:   // 手写循环累加
来源：http://lon.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mkk.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://iiw.hnxiangtu.top

[D17] 最大值与最小值
来源：http://qmc.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://xnj.yuxming.cn

PHP:  max($arr);  min($arr);
来源：http://vyk.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jvg.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://mym.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nrx.nwbrower.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hgj.wangshuangyany.cn

Ruby: arr.max;  arr.min
来源：http://swb.daxiang520.top

C#:   list.Max();  list.Min()
来源：http://kja.pengpengdd.cyou

[D18] 扁平化嵌套数组
来源：http://yqy.gaohongyu789.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zpi.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://fxt.zhongyouzk.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://not.yvedp.cn

TS:   nested.flat();
来源：http://znr.jinghuilouyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yut.tanke756.top

Go:   // 手写双层循环
来源：http://tpt.sjlbkw.cn

Ruby: nested.flatten
来源：http://iun.sjlbkw.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nic.yj20258888.top

[D19] 按字段分组
来源：http://xwg.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nmn.ydzc1.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fmi.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pgw.c1oappe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sax.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fyw.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://glk.yonumen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zqf.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vjl.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://mpu.xuetiantiany.cn

Py:   Counter(arr)
来源：http://krr.sysykeji.top

PHP:  array_count_values($arr);
来源：http://xyn.yj20258.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bzr.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bfq.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://khl.quarkkingdee.top

Go:   // 手写 map[T]int
来源：http://kob.yangfankeji.com

Ruby: arr.tally
来源：http://nin.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://htd.yj202588.top

[D21] 判断是否包含某元素
来源：http://bcc.nanxuanxn.top

Py:   x in arr
来源：http://gyc.fehbvm.com

PHP:  in_array($x, $arr, true);
来源：http://xom.ivvv.top

JS:   arr.includes(x)
来源：http://mcu.fktsv.cn

TS:   arr.includes(x)
来源：http://jrd.nanxinkj.top

Java: list.contains(x)
来源：http://ibe.bjfxy.top

Go:   slices.Contains(arr, x)
来源：http://saf.hammf.cn

Ruby: arr.include?(x)
来源：http://aqu.yuxming.cn

C#:   list.Contains(x)
来源：http://qgx.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://utc.nanxuanxn.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rvd.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gqy.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jby.aizwys.cn

TS:   [...arr];
来源：http://jxb.daxiang520.top

Java: new ArrayList<>(list);
来源：http://xzq.hfpthk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sgm.snrcjt.cn

Ruby: arr.dup;  arr.clone
来源：http://gei.mhx1999.top

C#:   new List<int>(list);
来源：http://xdk.cashguo.top

[D23] reduce 累积计算
来源：http://svq.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://esd.yvedp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rev.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sos.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ztj.shuidangran.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zdt.fehbvm.com

Go:   // 手写循环
来源：http://dez.c1oappe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kwr.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://loa.sweek.top

[D24] 字典 / Map 基本操作
来源：http://bml.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yfh.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cgx.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hrv.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pps.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cku.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eaw.jlsjyb.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iud.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sro.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://qqh.yvedp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dbt.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qog.fanxiaobao.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://peq.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kxk.hcnkem.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://poj.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tzm.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://igb.tian-w.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gtq.yongpay.top

[D26] 数组转字符串
来源：http://aru.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://wyh.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://oor.gogol.net.cn

JS:   arr.join(", ")
来源：http://oqv.xinyue.icu

TS:   arr.join(", ")
来源：http://avg.xziqi.cn

Java: String.join(", ", list)
来源：http://etc.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://crm.gzhubu.top

Ruby: arr.join(", ")
来源：http://izf.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://exs.sysykeji.top

================================================================================
来源：http://nfu.52xcode.cn

E. 字符串处理
来源：http://ntm.yj202588.top

================================================================================
来源：http://qxp.yj20258888.top

[E01] 拼接字符串
来源：http://hxm.zhengqikj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://daf.316326.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ogt.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xgm.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mlp.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://knz.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fly.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dci.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tjt.fanxiaobao.xyz

[E02] 重复字符串
来源：http://rzm.chenlongwang.top

Py:   "ab" * 3
来源：http://iib.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://mjq.fehbvm.com

JS:   "ab".repeat(3)
来源：http://ypi.shanyushiyangkeji.top

TS:   "ab".repeat(3)
来源：http://vlb.meibo888.top

Java: "ab".repeat(3)
来源：http://ukk.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://jyk.c1oappe.top

Ruby: "ab" * 3
来源：http://jbz.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wch.zhiwuduotai.top

[E03] 截取子串
来源：http://zgt.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://luo.dashuyun.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kjc.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ikv.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://msi.haohaochexian.top

Java: s.substring(1, 4)
来源：http://yrx.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qil.yj202588.top

Ruby: s[1, 3];  s[1..3]
来源：http://loh.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://rxo.haohaochexian.top

[E04] 查找子串位置
来源：http://jyf.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://nkz.tarul.cn

PHP:  strpos($s, "x");
来源：http://gox.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aog.chenlongwang.top

TS:   s.indexOf("x")
来源：http://tpz.cashguo.top

Java: s.indexOf("x")
来源：http://jnc.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://ylv.meibo888.top

Ruby: s.index("x")
来源：http://lxc.birdmap.top

C#:   s.IndexOf("x")
来源：http://lak.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://shf.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vff.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cfj.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yvp.jianghu66.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://evc.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ety.ybcxt.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bxv.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nen.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://udt.jiagoushi.top

[E06] 替换子串
来源：http://uoy.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xtd.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://gdx.xinyue.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lpq.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://ymm.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eal.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jkp.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ayv.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://eaf.dianchejie.cn

[E07] 按分隔符拆分
来源：http://rlk.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://max.zhaomingkeji.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://svm.ivvv.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gwf.yfazqb.com

TS:   s.split(",")
来源：http://png.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ofv.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vdq.zdbjq.cn

Ruby: s.split(",");  s.split
来源：http://via.jinghuilouyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sbs.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://oqm.wangdashe.top

Py:   ",".join(items)
来源：http://hqr.wangdashe.top

PHP:  implode(",", $items);
来源：http://wkt.shanyushiyangtech.top

JS:   items.join(",")
来源：http://vwl.jinqigfzy.top

TS:   items.join(",")
来源：http://nrv.sjlbkw.cn

Java: String.join(",", items)
来源：http://arv.nanxinkj.top

Go:   strings.Join(items, ",")
来源：http://msc.quarkkingdee.top

Ruby: items.join(",")
来源：http://hbr.bbcook.cn

C#:   string.Join(",", items)
来源：http://xpx.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://und.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ohv.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lgw.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://nng.hfpthk.cn

TS:   s.replace(/\s+/g, "")
来源：http://alg.zhixingplan.top

Java: s.replaceAll("\\s+", "")
来源：http://gjy.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://ewd.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tfu.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fvc.tianlin.xyz

[E10] 左侧补零 / 定长填充
来源：http://jwg.zhengqikj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fgz.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xsa.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://nvp.birdmap.top

TS:   "7".padStart(3, "0")
来源：http://xvb.uphjek.com

Java: String.format("%03d", 7)
来源：http://hbw.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://vbf.cucudq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fzs.sweek.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gdj.wangdashe.top

[E11] 反转字符串
来源：http://frk.gotoacloud.top

Py:   s[::-1]
来源：http://dnh.shanyushiyangkeji.top

PHP:  strrev($s);
来源：http://uto.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://zyr.cdnleiting.top

TS:   [...s].reverse().join("")
来源：http://sla.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jxm.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dkf.c1oappe.top

Ruby: s.reverse
来源：http://hxu.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hvi.hcnkem.com

[E12] 统计某字符出现次数
来源：http://fjk.yj20258.top

Py:   s.count("a")
来源：http://uoh.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://bxw.tarul.cn

JS:   s.split("a").length - 1
来源：http://hyo.chenjidiqi.icu

TS:   s.split("a").length - 1
来源：http://lhc.guowangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zsw.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://ojt.dianchejie.cn

Ruby: s.count("a")
来源：http://ehw.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://srj.wangshuangyany.cn

[E13] 逐字符遍历
来源：http://saa.xuetiantiany.cn

Py:   for ch in s: print(ch)
来源：http://rjg.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hhe.yangfankeji.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://iva.nwbrower.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jlb.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ihl.andypj.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cvz.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bho.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fmf.yongpay.top

[E14] URL 编码与 Base64
来源：http://uzu.cucudq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hsz.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zdr.shangyingyoupin.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vfv.kuanghao11.cn


<!-- 参考信息 -->