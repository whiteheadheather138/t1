代发 wailian999

Py:   len(arr)
来源：http://nsq.yuxming.cn

PHP:  count($arr);
来源：http://jqs.birdmap.top

JS:   arr.length
来源：http://ybe.cucudq.cn

TS:   arr.length
来源：http://wfg.kuanghao11.cn

Java: list.size();
来源：http://mbe.fengsongda.top

Go:   len(arr)
来源：http://muo.ydzc1.top

Ruby: arr.length; arr.size
来源：http://nus.shzxlz.cn

C#:   list.Count;
来源：http://nco.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://ghs.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kgp.yvedp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lrj.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://jrn.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://rrl.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://vir.9152youxi.cn

Go:   arr[1:4]
来源：http://fqq.shanyushiyangkeji.top

Ruby: arr[1, 3]
来源：http://xun.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://jpo.0kj1m.cn

[D08] 合并两个数组
来源：http://rmy.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://qbt.bjfxy.top

PHP:  array_merge($a, $b);
来源：http://mvp.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://hua.fktsv.cn

TS:   [...a, ...b];
来源：http://xku.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://shh.cheryme.top

Go:   append(a, b...)
来源：http://rzi.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://fkm.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://frx.gogol.net.cn

[D09] 排序（升序）
来源：http://upd.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://ydb.ehwqpu.com

PHP:  sort($arr);
来源：http://spa.zhijiandao.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gzf.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pzf.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nmr.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uzc.bbcook.cn

Ruby: arr.sort
来源：http://odq.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://cov.feifeiyinyue.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cpi.haohaochexian.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kko.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bjx.wangdashe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rqq.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://etf.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mal.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://anv.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fcv.chenjidiqi.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lfp.hfpthk.cn

[D11] 反转数组
来源：http://lde.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://gac.xylfe.cn

PHP:  array_reverse($arr);
来源：http://lql.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jzu.daria6918.cn

TS:   [...arr].reverse();
来源：http://efg.hfpthk.cn

Java: Collections.reverse(list);
来源：http://ggi.smart0.xyz

Go:   slices.Reverse(arr)
来源：http://acr.guannengcc.top

Ruby: arr.reverse
来源：http://ayn.nwbrower.top

C#:   list.Reverse();
来源：http://zdg.yanxiufei.cn

[D12] 查找元素下标
来源：http://akl.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://vik.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pnd.fanxiaobao.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uto.quarkkingdee.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aqd.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://omj.sufxvd.cn

Go:   slices.Index(arr, x)
来源：http://lav.tian-w.cn

Ruby: arr.index(x)
来源：http://pso.uphjek.com

C#:   list.IndexOf(x);
来源：http://qqr.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://rkj.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qjl.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qbl.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://qal.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://ebd.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fss.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wdf.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://zhr.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nzt.feifeiyinyue.top

[D14] 映射转换（每个元素变形）
来源：http://stz.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lnn.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bpq.wangshuangyany.cn

JS:   arr.map(x => x * 2)
来源：http://ckh.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://rna.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bct.cashguo.top

Go:   // 手写循环
来源：http://uwz.cdnleiting.top

Ruby: arr.map { |x| x * 2 }
来源：http://zbn.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pez.fehbvm.com

[D15] 去重
来源：http://lzw.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vih.gzhubu.top

PHP:  array_unique($arr);
来源：http://jxa.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://xxc.316326.xyz

TS:   [...new Set(arr)]
来源：http://uqh.sxryk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gxn.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cyl.hesvh.cn

Ruby: arr.uniq
来源：http://ayd.zhijiandao.cn

C#:   list.Distinct().ToList()
来源：http://rvb.chenjidiqi.icu

[D16] 求和与平均值
来源：http://lbt.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://isu.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rpc.chenzaomai.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ylq.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mgc.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oga.tian-w.cn

Go:   // 手写循环累加
来源：http://yxv.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zsv.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://goh.ctjpmb.com

[D17] 最大值与最小值
来源：http://mmu.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://cka.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://xeo.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kqd.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://qsz.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ghy.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hyj.meibo888.top

Ruby: arr.max;  arr.min
来源：http://hns.jyoumei.cn

C#:   list.Max();  list.Min()
来源：http://ond.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://qsg.sufxvd.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kbl.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://vfj.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mod.meibo888.top

TS:   nested.flat();
来源：http://tcp.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wql.chenlongwang.top

Go:   // 手写双层循环
来源：http://erp.fanxiaobao.xyz

Ruby: nested.flatten
来源：http://osd.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cyd.jiagoushi.top

[D19] 按字段分组
来源：http://zgx.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uac.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qcw.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nef.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hhj.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yqh.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://tar.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rrv.hcnkem.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://npd.havefunace.top

[D20] 统计每个元素出现次数
来源：http://ila.gogol.net.cn

Py:   Counter(arr)
来源：http://ifw.sxryk.cn

PHP:  array_count_values($arr);
来源：http://wge.ywan-chungtsiang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gew.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://epp.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kjr.zhongyouzk.top

Go:   // 手写 map[T]int
来源：http://lpj.vqdsnc.cn

Ruby: arr.tally
来源：http://vty.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fgt.cheryme.top

[D21] 判断是否包含某元素
来源：http://qwx.sxryk.cn

Py:   x in arr
来源：http://xdx.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://pom.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://ghp.jinqigfzy.top

TS:   arr.includes(x)
来源：http://psl.xingfuxueyuan.xyz

Java: list.contains(x)
来源：http://abf.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://hpj.jianghu66.top

Ruby: arr.include?(x)
来源：http://zpq.mhx1999.top

C#:   list.Contains(x)
来源：http://dia.chenzaomai.com

[D22] 复制数组（避免共享引用）
来源：http://qzr.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qsv.hywenlv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pex.gzhubu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hnm.ivvv.top

TS:   [...arr];
来源：http://bfn.yueranfly.top

Java: new ArrayList<>(list);
来源：http://iog.fktsv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ndi.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://ges.aizwys.cn

C#:   new List<int>(list);
来源：http://mzq.hesvh.cn

[D23] reduce 累积计算
来源：http://cbo.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nsy.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ixf.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ogm.shzxlz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vcz.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zmd.ctjpmb.com

Go:   // 手写循环
来源：http://cqv.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://krp.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qnq.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://jss.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://byt.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fri.dashuyun.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wid.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ued.wangdashe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rwg.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gpo.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aqo.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yut.hnxiangtu.top

[D25] Set 集合去重与交并差
来源：http://pzg.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xtr.tian-w.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zxc.redwolf501.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hfc.shanyushiyangtech.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://egd.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xfw.zhoulong.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gsu.yongpay.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cqz.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uhc.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://irr.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://ydf.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://qgu.jinghuilouyu.cn

JS:   arr.join(", ")
来源：http://yub.hfpthk.cn

TS:   arr.join(", ")
来源：http://iue.redwolf501.top

Java: String.join(", ", list)
来源：http://ybi.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://hir.chenzaomai.com

Ruby: arr.join(", ")
来源：http://cma.xuanzx.com

C#:   string.Join(", ", list)
来源：http://roh.daxiang520.top

================================================================================
来源：http://zyt.tianlin.xyz

E. 字符串处理
来源：http://qmi.cucudq.cn

================================================================================
来源：http://kgn.zhoulong.xyz

[E01] 拼接字符串
来源：http://cew.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://huy.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ify.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hjn.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pvq.ydjk.org.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mfs.9152youxi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yha.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xle.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xgf.hnxiangtu.top

[E02] 重复字符串
来源：http://idd.yueranfly.top

Py:   "ab" * 3
来源：http://lid.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://dna.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://yqn.tarul.cn

TS:   "ab".repeat(3)
来源：http://vck.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://xxa.hammf.cn

Go:   strings.Repeat("ab", 3)
来源：http://knp.xylfe.cn

Ruby: "ab" * 3
来源：http://yqw.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bee.daxiang520.top

[E03] 截取子串
来源：http://mgt.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nnd.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aeh.jianghu66.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ukk.sjlbkw.cn

TS:   s.slice(1, 4)
来源：http://ovr.sufxvd.cn

Java: s.substring(1, 4)
来源：http://xsc.daxiang520.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gvy.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dbg.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://vyo.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://edl.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://gbh.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://fgw.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zfw.haohaochexian.top

TS:   s.indexOf("x")
来源：http://suy.sufxvd.cn

Java: s.indexOf("x")
来源：http://chx.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://ooa.zhengqikj.top

Ruby: s.index("x")
来源：http://zch.zhiwuduotai.top

C#:   s.IndexOf("x")
来源：http://fwg.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pkn.yfazqb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hts.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ojz.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qpq.sysykeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vow.ydjk.org.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bdj.tian-w.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xjk.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ziw.cqqwz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qgo.chenzaomai.com

[E06] 替换子串
来源：http://tip.hnqzz.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pea.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://tbp.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://txt.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://zfm.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jcm.hnxiangtu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zkb.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ega.tanke756.top

C#:   s.Replace("a", "b")
来源：http://oei.zhijiandao.cn

[E07] 按分隔符拆分
来源：http://xsb.sjlbkw.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bsf.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://krv.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jux.sysykeji.top

TS:   s.split(",")
来源：http://vud.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://hgr.cheryme.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gxs.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://lbl.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vwg.xuetiantiany.cn

[E08] 数组按分隔符合并
来源：http://zaq.xylfe.cn

Py:   ",".join(items)
来源：http://olo.uphjek.com

PHP:  implode(",", $items);
来源：http://urq.yueranfly.top

JS:   items.join(",")
来源：http://jal.yuanzhike.top

TS:   items.join(",")
来源：http://mzq.xziqi.cn

Java: String.join(",", items)
来源：http://vih.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://rys.smart0.xyz

Ruby: items.join(",")
来源：http://tyj.ydzc1.top

C#:   string.Join(",", items)
来源：http://cuv.jlsjyb.cn

[E09] 去除所有空白字符
来源：http://iod.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://alk.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ehk.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://djz.wangshuangyany.cn

TS:   s.replace(/\s+/g, "")
来源：http://rox.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://nzd.redwolf501.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lja.cucudq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yjs.guannengcc.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qcs.316326.xyz

[E10] 左侧补零 / 定长填充
来源：http://bai.chenjidiqi.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wsb.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://edv.jinyuanbaomall.cn

JS:   "7".padStart(3, "0")
来源：http://kso.feifeiyinyue.top

TS:   "7".padStart(3, "0")
来源：http://nbp.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://grx.zhaomingkeji.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://kgx.zhaomingkeji.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nih.tanke756.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oel.yuxming.cn

[E11] 反转字符串
来源：http://vgs.sjlbkw.cn

Py:   s[::-1]
来源：http://nfm.zhongyouzk.top

PHP:  strrev($s);
来源：http://arm.ivvv.top

JS:   [...s].reverse().join("")
来源：http://rqj.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://wzf.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://buz.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://kjo.xinyue.icu

Ruby: s.reverse
来源：http://phi.feifeiyinyue.top

C#:   new string(s.Reverse().ToArray())
来源：http://rxn.hcnkem.com

[E12] 统计某字符出现次数
来源：http://ohn.chenzaomai.com

Py:   s.count("a")
来源：http://yhw.yonumen.top

PHP:  substr_count($s, "a");
来源：http://ngn.ywan-chungtsiang.top

JS:   s.split("a").length - 1
来源：http://xwh.yj20258.top

TS:   s.split("a").length - 1
来源：http://pop.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rbn.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://evw.nanxinkj.top

Ruby: s.count("a")
来源：http://jjx.uphjek.com

C#:   s.Count(c => c == 'a')
来源：http://jcp.zdqjudy.top

[E13] 逐字符遍历
来源：http://mia.hesvh.cn


<!-- 参考信息 -->