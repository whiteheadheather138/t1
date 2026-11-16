代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://eju.shzxlz.cn

[D08] 合并两个数组
来源：http://qhh.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://drb.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://ylc.tanke756.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tzc.9152youxi.cn

TS:   [...a, ...b];
来源：http://qvl.yongpay.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ekj.aizwys.cn

Go:   append(a, b...)
来源：http://awf.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://gjf.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://ifq.daria6918.cn

[D09] 排序（升序）
来源：http://ohd.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://bar.tianlin.xyz

PHP:  sort($arr);
来源：http://tzr.smart0.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dtr.gzhubu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uph.c1oappe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://axw.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mpi.zhongyouzk.top

Ruby: arr.sort
来源：http://jkf.zhixingplan.top

C#:   list.Sort();
来源：http://owb.smart0.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://qxj.hesvh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gbg.sweek.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bih.chenjidiqi.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cer.dianchejie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uav.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xtm.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ayl.daxiang520.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://koo.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://akf.zdqjudy.top

[D11] 反转数组
来源：http://mmb.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://dap.hesvh.cn

PHP:  array_reverse($arr);
来源：http://ujm.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ljw.zdqjudy.top

TS:   [...arr].reverse();
来源：http://tmc.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://wwx.316326.xyz

Go:   slices.Reverse(arr)
来源：http://qfn.c1oappe.top

Ruby: arr.reverse
来源：http://kvi.sysykeji.top

C#:   list.Reverse();
来源：http://oju.bbcook.cn

[D12] 查找元素下标
来源：http://xjz.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://qbo.dashuyun.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xkt.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ruv.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vvd.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gam.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://ear.0kj1m.cn

Ruby: arr.index(x)
来源：http://trl.ybcxt.top

C#:   list.IndexOf(x);
来源：http://bzk.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://wtu.redwolf501.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dvw.52xcode.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gqp.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://tvs.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://kse.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xmm.meibo888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://euw.cqqwz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hgf.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hai.jqgfzy.top

[D14] 映射转换（每个元素变形）
来源：http://gqf.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fdx.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ays.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://nnh.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://trc.cqqwz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://thf.hfpthk.cn

Go:   // 手写循环
来源：http://xzm.ywan-chungtsiang.top

Ruby: arr.map { |x| x * 2 }
来源：http://dic.nwbrower.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mzz.uphjek.com

[D15] 去重
来源：http://gkx.andypj.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uia.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://rtl.gogol.net.cn

JS:   [...new Set(arr)]
来源：http://gmb.sysykeji.top

TS:   [...new Set(arr)]
来源：http://ufc.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eqi.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://zir.chenlongwang.top

Ruby: arr.uniq
来源：http://xbj.cdnleiting.top

C#:   list.Distinct().ToList()
来源：http://tez.aibaodan.cn

[D16] 求和与平均值
来源：http://lvh.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vrp.pengpengdd.cyou

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pjb.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xoe.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wsj.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xvs.cheryme.top

Go:   // 手写循环累加
来源：http://qer.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://unc.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://uhr.hnxiangtu.top

[D17] 最大值与最小值
来源：http://xfg.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://oph.bbcook.cn

PHP:  max($arr);  min($arr);
来源：http://zxr.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rpr.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://wsx.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wyi.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://paz.316326.xyz

Ruby: arr.max;  arr.min
来源：http://dcm.birdmap.top

C#:   list.Max();  list.Min()
来源：http://mut.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://hhh.hongshengwenyu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ghf.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://mav.tianlin.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wdy.jiagoushi.top

TS:   nested.flat();
来源：http://zws.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pxj.snrcjt.cn

Go:   // 手写双层循环
来源：http://cfj.tanke756.top

Ruby: nested.flatten
来源：http://qbe.ehwqpu.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://axz.nanxinkj.top

[D19] 按字段分组
来源：http://cku.ivvv.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sdu.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://few.fanxiaobao.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lxt.sweek.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://htg.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://otc.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://vlg.xziqi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://knz.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fhq.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://rag.ivvv.top

Py:   Counter(arr)
来源：http://esx.ppjwa.cn

PHP:  array_count_values($arr);
来源：http://vnu.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rcr.quarkkingdee.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bph.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ezy.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://ops.gotoacloud.top

Ruby: arr.tally
来源：http://nuf.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://obv.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://yqq.jqgufenzy.top

Py:   x in arr
来源：http://khs.ehwqpu.com

PHP:  in_array($x, $arr, true);
来源：http://fbh.vehdjk.com

JS:   arr.includes(x)
来源：http://jfb.chenzaomai.com

TS:   arr.includes(x)
来源：http://eiu.guannengcc.top

Java: list.contains(x)
来源：http://cnf.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://hox.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://mcy.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://wcz.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://wpc.yuanzhike.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://odf.gogol.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hxx.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sgk.hesvh.cn

TS:   [...arr];
来源：http://fyw.mhx1999.top

Java: new ArrayList<>(list);
来源：http://msi.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://vot.hywenlv.cn

Ruby: arr.dup;  arr.clone
来源：http://sfd.vehdjk.com

C#:   new List<int>(list);
来源：http://qas.hammf.cn

[D23] reduce 累积计算
来源：http://ylk.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dsj.zhoulong.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nor.ydzc1.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rmc.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wwn.hcnkem.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://fbo.xylfe.cn

Go:   // 手写循环
来源：http://ncc.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://spa.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nrj.feifeiyinyue.top

[D24] 字典 / Map 基本操作
来源：http://fex.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dip.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uvh.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rpv.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://emp.daria6918.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vra.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hto.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gze.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://icd.yongpay.top

[D25] Set 集合去重与交并差
来源：http://lgz.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vws.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://obj.nanxinkj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ezj.0kj1m.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jjw.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mbm.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lnj.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vcs.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://imx.xuanzx.com

[D26] 数组转字符串
来源：http://cly.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://maz.yueranfly.top

PHP:  implode(", ", $arr);
来源：http://jdq.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://lej.yj20258888.top

TS:   arr.join(", ")
来源：http://xdi.ivvv.top

Java: String.join(", ", list)
来源：http://sgu.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://zmn.yvedp.cn

Ruby: arr.join(", ")
来源：http://atp.yj20258888.top

C#:   string.Join(", ", list)
来源：http://pvw.iojbl.cn

================================================================================
来源：http://pyq.shzxlz.cn

E. 字符串处理
来源：http://hvg.uphjek.com

================================================================================
来源：http://pqy.hnqzz.top

[E01] 拼接字符串
来源：http://kys.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kex.meibo888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://klz.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wpw.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zxs.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kee.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rag.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aej.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jdw.xziqi.cn

[E02] 重复字符串
来源：http://xwz.sufxvd.cn

Py:   "ab" * 3
来源：http://uxy.nanxuanxn.top

PHP:  str_repeat("ab", 3);
来源：http://gup.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://veh.fehbvm.com

TS:   "ab".repeat(3)
来源：http://pyh.52xcode.cn

Java: "ab".repeat(3)
来源：http://vqw.daria6918.cn

Go:   strings.Repeat("ab", 3)
来源：http://ipi.yuanzhike.top

Ruby: "ab" * 3
来源：http://lda.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rbz.zhaomingkeji.xyz

[E03] 截取子串
来源：http://qbv.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jvd.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://npk.yanxiufei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ipu.birdmap.top

TS:   s.slice(1, 4)
来源：http://cts.jinqigufen.top

Java: s.substring(1, 4)
来源：http://aqh.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pvh.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://tqs.cheryme.top

C#:   s.Substring(1, 3)
来源：http://qjn.jiagoushi.top

[E04] 查找子串位置
来源：http://rsd.yangfankeji.com

Py:   s.find("x");  s.index("x")
来源：http://qkt.xylfe.cn

PHP:  strpos($s, "x");
来源：http://fyg.yj20258888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ies.ybcxt.top

TS:   s.indexOf("x")
来源：http://dig.daxiang520.top

Java: s.indexOf("x")
来源：http://bfj.yj20258.top

Go:   strings.Index(s, "x")
来源：http://lzm.gaohongyu789.top

Ruby: s.index("x")
来源：http://ugl.cucudq.cn

C#:   s.IndexOf("x")
来源：http://ygf.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gxq.shuidangran.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kun.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kce.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ywy.gotoacloud.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lsn.sysykeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://flo.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hjc.zhoulong.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ckl.feifeiyinyue.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ftc.chenzaomai.com

[E06] 替换子串
来源：http://ful.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pbt.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://zwn.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qwd.zhengqikj.top

TS:   s.replaceAll("a", "b")
来源：http://igq.xziqi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wds.gotoacloud.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dkg.nanxinkj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wgv.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://pws.sweek.top

[E07] 按分隔符拆分
来源：http://sdh.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tro.hfpthk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hgk.hesvh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://icu.jlsjyb.cn

TS:   s.split(",")
来源：http://xef.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ums.xuanzx.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rnm.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://wkx.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ohd.meibo888.top

[E08] 数组按分隔符合并
来源：http://ltv.sjlbkw.cn

Py:   ",".join(items)
来源：http://djb.nwbrower.top

PHP:  implode(",", $items);
来源：http://szq.uphjek.com

JS:   items.join(",")
来源：http://qzd.jqgufenzy.top

TS:   items.join(",")
来源：http://amm.hywenlv.cn

Java: String.join(",", items)
来源：http://lfl.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://yip.feifeiyinyue.top

Ruby: items.join(",")
来源：http://klv.yj20258.top

C#:   string.Join(",", items)
来源：http://qzn.gogol.net.cn

[E09] 去除所有空白字符
来源：http://gwi.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lot.hfpthk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://exb.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://sxa.yangfankeji.com

TS:   s.replace(/\s+/g, "")
来源：http://vyi.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://wai.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ztx.uphjek.com

Ruby: s.gsub(/\s+/, "")
来源：http://ytu.cucudq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lfa.jlsjyb.cn

[E10] 左侧补零 / 定长填充
来源：http://vtg.guannengcc.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mpj.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://otg.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://mpe.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://igm.cucudq.cn

Java: String.format("%03d", 7)
来源：http://kkn.jyoumei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bqy.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wge.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cch.jiagoushi.top

[E11] 反转字符串
来源：http://ylh.yonumen.top

Py:   s[::-1]
来源：http://qgq.iojbl.cn

PHP:  strrev($s);
来源：http://kga.zhijiandao.cn

JS:   [...s].reverse().join("")
来源：http://bvz.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://ocl.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://izc.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://bto.zycfv.cn

Ruby: s.reverse
来源：http://jwu.haohaochexian.top

C#:   new string(s.Reverse().ToArray())
来源：http://yoe.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://oky.yanxiufei.cn

Py:   s.count("a")
来源：http://xtp.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://rmx.zhoulong.xyz

JS:   s.split("a").length - 1
来源：http://bar.cheryme.top

TS:   s.split("a").length - 1
来源：http://ldi.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kzo.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://ryi.316326.xyz

Ruby: s.count("a")
来源：http://uzd.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://dbs.ctjpmb.com

[E13] 逐字符遍历
来源：http://vex.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://ykh.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pjv.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gxy.jianghu66.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qsw.tanke756.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qkz.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://slf.jinyuanbaomall.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lpj.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ius.snrcjt.cn

[E14] URL 编码与 Base64
来源：http://taz.vehdjk.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xcg.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ojb.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pji.9152youxi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dkx.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://avc.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zdw.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ggs.mhx1999.top


<!-- 参考信息 -->