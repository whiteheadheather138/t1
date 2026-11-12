代发 wailian999

TS:   arr.slice(1, 4);
来源：http://swi.yongpay.top

Java: list.subList(1, 4);
来源：http://tbh.shzxlz.cn

Go:   arr[1:4]
来源：http://ikx.yuxming.cn

Ruby: arr[1, 3]
来源：http://dbf.nwbrower.top

C#:   list.GetRange(1, 3);
来源：http://zsu.xingfuxueyuan.xyz

[D08] 合并两个数组
来源：http://lyb.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://rin.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://fnw.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kmu.jinqigufen.top

TS:   [...a, ...b];
来源：http://ale.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fyx.hongshengwenyu.top

Go:   append(a, b...)
来源：http://xjb.vqdsnc.cn

Ruby: a + b;  a.concat(b)
来源：http://xyt.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://yku.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://yfi.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://ygf.aibaodan.cn

PHP:  sort($arr);
来源：http://faa.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xwk.tianlin.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://axv.wangshuangyany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cwv.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bzt.ppjwa.cn

Ruby: arr.sort
来源：http://gzy.cheryme.top

C#:   list.Sort();
来源：http://odc.tarul.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qmm.nanxinkj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://umz.chenjidiqi.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gqv.mhx1999.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pcb.yfazqb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blx.xingfuxueyuan.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pfa.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xeg.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mqe.pengpengdd.cyou

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mvh.gogol.net.cn

[D11] 反转数组
来源：http://dyx.ywan-chungtsiang.top

Py:   arr[::-1];  arr.reverse()
来源：http://wdx.9152youxi.cn

PHP:  array_reverse($arr);
来源：http://sao.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wwy.cashguo.top

TS:   [...arr].reverse();
来源：http://zvi.jqgfzy.top

Java: Collections.reverse(list);
来源：http://tti.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://pwq.chenzaomai.com

Ruby: arr.reverse
来源：http://fwt.ybcxt.top

C#:   list.Reverse();
来源：http://bpx.birdmap.top

[D12] 查找元素下标
来源：http://dba.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://zmk.jianghu66.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vnv.tian-w.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iqc.yj20258.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qij.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hee.haohaochexian.top

Go:   slices.Index(arr, x)
来源：http://fkk.gotoacloud.top

Ruby: arr.index(x)
来源：http://wap.yvedp.cn

C#:   list.IndexOf(x);
来源：http://tux.ehwqpu.com

[D13] 过滤（保留满足条件的）
来源：http://yvs.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kbi.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vbc.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://yzn.sweek.top

TS:   arr.filter(x => x > 3)
来源：http://cpq.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bvj.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://okc.jqgufenzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://blw.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://iwt.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://ulw.gaohongyu789.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xxk.jianghu66.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://apx.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://zvb.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://yys.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rfx.daxiang520.top

Go:   // 手写循环
来源：http://lqz.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://lho.shzxlz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sqx.sxryk.cn

[D15] 去重
来源：http://ctb.hysaishi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oxw.ivvv.top

PHP:  array_unique($arr);
来源：http://ust.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://hrw.havefunace.top

TS:   [...new Set(arr)]
来源：http://klo.hesvh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fkd.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://ilm.zhoulong.xyz

Ruby: arr.uniq
来源：http://dxt.nwbrower.top

C#:   list.Distinct().ToList()
来源：http://spt.andypj.xyz

[D16] 求和与平均值
来源：http://yti.cashguo.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yqn.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wma.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://plb.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://teo.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hys.guannengcc.top

Go:   // 手写循环累加
来源：http://gug.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ocj.xylfe.cn

C#:   list.Sum();  list.Average()
来源：http://klp.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://ioa.hysaishi.cn

Py:   max(arr);  min(arr)
来源：http://nvx.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://tzp.gogol.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jis.daxiang520.top

TS:   Math.max(...arr);
来源：http://xic.sweek.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fkg.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dnj.cheryme.top

Ruby: arr.max;  arr.min
来源：http://jmn.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://nzo.nanxuanxn.top

[D18] 扁平化嵌套数组
来源：http://las.zhiwuduotai.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aft.havefunace.top

PHP:  array_merge(...$nested);
来源：http://per.ydjk.org.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uto.0kj1m.cn

TS:   nested.flat();
来源：http://npk.yj20258.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cek.daxiang520.top

Go:   // 手写双层循环
来源：http://nrb.smart0.xyz

Ruby: nested.flatten
来源：http://kko.tanke756.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nwv.xinyue.icu

[D19] 按字段分组
来源：http://uvm.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oec.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wgc.zdbjq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vfg.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oks.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dov.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://sau.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://blk.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ybw.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://aaf.bbcook.cn

Py:   Counter(arr)
来源：http://qhp.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://ayq.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oyb.yonumen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://arz.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oli.pycfn.com

Go:   // 手写 map[T]int
来源：http://ncw.jiagoushi.top

Ruby: arr.tally
来源：http://juk.nanxinkj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nrc.jianghu66.top

[D21] 判断是否包含某元素
来源：http://vmi.chenlongwang.top

Py:   x in arr
来源：http://cet.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://uee.zdbjq.cn

JS:   arr.includes(x)
来源：http://xzc.tianlin.xyz

TS:   arr.includes(x)
来源：http://wgw.quarkkingdee.top

Java: list.contains(x)
来源：http://pga.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://afm.zdbjq.cn

Ruby: arr.include?(x)
来源：http://jmz.zhoulong.xyz

C#:   list.Contains(x)
来源：http://ufn.cheryme.top

[D22] 复制数组（避免共享引用）
来源：http://lun.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wrr.hesvh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vrk.hysaishi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ssc.guannengcc.top

TS:   [...arr];
来源：http://pgf.yuxming.cn

Java: new ArrayList<>(list);
来源：http://ipg.jinqigfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://gee.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://rdy.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://hql.kuanghao11.cn

[D23] reduce 累积计算
来源：http://whx.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zdb.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cdg.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xpc.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pbj.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rxn.yonumen.top

Go:   // 手写循环
来源：http://qhn.svipenyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sri.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pgu.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://rto.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lns.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ncm.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gmo.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bxz.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://miq.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lkr.hfpthk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tih.yuanzhike.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://egs.sjlbkw.cn

[D25] Set 集合去重与交并差
来源：http://fgp.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wpu.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rko.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://utx.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nbg.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jyg.jqgfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ejf.shangyingyoupin.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tym.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zjl.hnxiangtu.top

[D26] 数组转字符串
来源：http://bvm.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://cds.uphjek.com

PHP:  implode(", ", $arr);
来源：http://oue.jinqigfzy.top

JS:   arr.join(", ")
来源：http://qyj.yvedp.cn

TS:   arr.join(", ")
来源：http://mmb.gzhubu.top

Java: String.join(", ", list)
来源：http://ufp.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://dgv.ydzc1.top

Ruby: arr.join(", ")
来源：http://alg.xinyue.icu

C#:   string.Join(", ", list)
来源：http://eja.gzhubu.top

================================================================================
来源：http://rtc.iojbl.cn

E. 字符串处理
来源：http://jjd.vehdjk.com

================================================================================
来源：http://fuw.xuanzx.com

[E01] 拼接字符串
来源：http://iwf.pycfn.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wsc.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://akw.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ftc.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uxp.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tni.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cbg.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ksp.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bds.hnxiangtu.top

[E02] 重复字符串
来源：http://yga.tian-w.cn

Py:   "ab" * 3
来源：http://esr.tian-w.cn

PHP:  str_repeat("ab", 3);
来源：http://lfj.guannengcc.top

JS:   "ab".repeat(3)
来源：http://sdb.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://glj.yuxming.cn

Java: "ab".repeat(3)
来源：http://ktd.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://ndd.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://nrf.tian-w.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gsl.hnqzz.top

[E03] 截取子串
来源：http://urd.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tqu.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lrg.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yrd.xziqi.cn

TS:   s.slice(1, 4)
来源：http://kys.bbcook.cn

Java: s.substring(1, 4)
来源：http://bnj.vehdjk.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eoz.havefunace.top

Ruby: s[1, 3];  s[1..3]
来源：http://cab.yongpay.top

C#:   s.Substring(1, 3)
来源：http://drp.zhoulong.xyz

[E04] 查找子串位置
来源：http://opv.feifeiyinyue.top

Py:   s.find("x");  s.index("x")
来源：http://xfi.fehbvm.com

PHP:  strpos($s, "x");
来源：http://qjj.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://guh.jiagoushi.top

TS:   s.indexOf("x")
来源：http://lfx.nwbrower.top

Java: s.indexOf("x")
来源：http://qxc.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://ahf.hesvh.cn

Ruby: s.index("x")
来源：http://dwd.epnwcf.com

C#:   s.IndexOf("x")
来源：http://ylz.yfazqb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ulk.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pya.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://coi.zhongyouzk.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ndp.zhixingplan.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://snb.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dho.fengsongda.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gkm.zhengqikj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rqa.0kj1m.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bcm.jinghuilouyu.cn

[E06] 替换子串
来源：http://mxd.jyoumei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nyn.hongshengwenyu.top

PHP:  str_replace("a", "b", $s);
来源：http://oul.sjlbkw.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hio.hysaishi.cn

TS:   s.replaceAll("a", "b")
来源：http://nvz.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://idt.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://adt.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hvx.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://gig.smart0.xyz

[E07] 按分隔符拆分
来源：http://yib.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wgf.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uzr.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ztt.ybcxt.top

TS:   s.split(",")
来源：http://rrt.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nrj.gzhubu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://flv.haohaochexian.top

Ruby: s.split(",");  s.split
来源：http://mbe.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hnm.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://lvh.shanyushiyangtech.top

Py:   ",".join(items)
来源：http://vrp.nanxinkj.top

PHP:  implode(",", $items);
来源：http://etw.pycfn.com

JS:   items.join(",")
来源：http://eqw.chenjidiqi.icu

TS:   items.join(",")
来源：http://qet.hammf.cn

Java: String.join(",", items)
来源：http://hce.fengsongda.top

Go:   strings.Join(items, ",")
来源：http://btv.xuetiantiany.cn

Ruby: items.join(",")
来源：http://ccy.havefunace.top

C#:   string.Join(",", items)
来源：http://scz.xziqi.cn

[E09] 去除所有空白字符
来源：http://tit.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rmb.aibaodan.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xcp.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://wyw.ydjk.org.cn

TS:   s.replace(/\s+/g, "")
来源：http://fbi.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://gsl.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ynh.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://qky.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://heq.nwbrower.top

[E10] 左侧补零 / 定长填充
来源：http://szi.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://maa.tian-w.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mow.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://nhi.zdbjq.cn

TS:   "7".padStart(3, "0")
来源：http://tfo.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://cfh.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lpi.jinqigfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kxi.jyoumei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kiv.havefunace.top

[E11] 反转字符串
来源：http://dew.yj20258.top

Py:   s[::-1]
来源：http://irk.redwolf501.top

PHP:  strrev($s);
来源：http://fwx.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://jlj.tian-w.cn

TS:   [...s].reverse().join("")
来源：http://aie.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bjd.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://itm.fanxiaobao.xyz

Ruby: s.reverse
来源：http://mgy.ivvv.top

C#:   new string(s.Reverse().ToArray())
来源：http://opu.yueranfly.top

[E12] 统计某字符出现次数
来源：http://wqq.ybcxt.top

Py:   s.count("a")
来源：http://uox.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://rcl.hammf.cn

JS:   s.split("a").length - 1
来源：http://yix.wangshuangyany.cn

TS:   s.split("a").length - 1
来源：http://fbw.gotoacloud.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xii.nanxinkj.top

Go:   strings.Count(s, "a")
来源：http://slj.yueranfly.top

Ruby: s.count("a")
来源：http://yqp.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://wrr.iojbl.cn

[E13] 逐字符遍历
来源：http://rbf.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://lyv.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pmr.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://riz.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mgl.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://msl.xingfuxueyuan.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ikz.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://krt.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mhy.pycfn.com

[E14] URL 编码与 Base64
来源：http://ahw.shuidangran.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tak.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://vfx.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cab.tian-w.cn


<!-- 参考信息 -->