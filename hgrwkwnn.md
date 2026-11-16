代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://ckt.wangshuangyany.cn

C#:   a.Concat(b).ToList()
来源：http://olf.fengsongda.top

[D09] 排序（升序）
来源：http://mxr.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://pyz.pycfn.com

PHP:  sort($arr);
来源：http://obd.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hjn.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://aup.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vri.aibaodan.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ipi.tianlin.xyz

Ruby: arr.sort
来源：http://mpy.zhijiandao.cn

C#:   list.Sort();
来源：http://zxc.sjlbkw.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vuj.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xoh.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ysk.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dxr.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iuz.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://exh.fzhhl.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mym.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ugw.havefunace.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uqz.vehdjk.com

[D11] 反转数组
来源：http://qcp.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://fki.xingfuxueyuan.xyz

PHP:  array_reverse($arr);
来源：http://sbg.hammf.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cfn.aibaodan.cn

TS:   [...arr].reverse();
来源：http://lst.yueranfly.top

Java: Collections.reverse(list);
来源：http://oqz.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://iro.redwolf501.top

Ruby: arr.reverse
来源：http://qma.jianghu66.top

C#:   list.Reverse();
来源：http://xle.ppjwa.cn

[D12] 查找元素下标
来源：http://aqd.hesvh.cn

Py:   arr.index(x);  x in arr
来源：http://agn.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xxg.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pwe.zhaomingkeji.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://boy.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rqu.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://nyi.iojbl.cn

Ruby: arr.index(x)
来源：http://qxm.tianlin.xyz

C#:   list.IndexOf(x);
来源：http://iyg.yangfankeji.com

[D13] 过滤（保留满足条件的）
来源：http://nfw.tarul.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hte.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wkp.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://xxc.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://kyk.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dmg.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xsr.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xtx.jiagoushi.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fgg.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://bbk.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xrg.redwolf501.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ktm.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://gkz.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://ihd.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://awp.bjfxy.top

Go:   // 手写循环
来源：http://iri.uphjek.com

Ruby: arr.map { |x| x * 2 }
来源：http://qrt.yj20258888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://exm.haohaochexian.top

[D15] 去重
来源：http://crz.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wdb.tianlin.xyz

PHP:  array_unique($arr);
来源：http://pae.shanyushiyangkeji.top

JS:   [...new Set(arr)]
来源：http://gre.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://fxl.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dlk.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://iez.jqgfzy.top

Ruby: arr.uniq
来源：http://foy.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://wmc.fzhhl.top

[D16] 求和与平均值
来源：http://fni.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uhx.hfpthk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://stw.ybcxt.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rac.yonumen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://okx.shzxlz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dpm.hesvh.cn

Go:   // 手写循环累加
来源：http://sla.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mps.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://bvg.epnwcf.com

[D17] 最大值与最小值
来源：http://lzp.guowangkeji.top

Py:   max(arr);  min(arr)
来源：http://vqu.sweek.top

PHP:  max($arr);  min($arr);
来源：http://lkp.tianlin.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kge.wangdashe.top

TS:   Math.max(...arr);
来源：http://zdn.guannengcc.top

Java: Collections.max(list);  Collections.min(list);
来源：http://njv.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oos.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://chg.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://ejz.yueranfly.top

[D18] 扁平化嵌套数组
来源：http://lkf.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dtl.yanxiufei.cn

PHP:  array_merge(...$nested);
来源：http://kqa.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ooq.vqdsnc.cn

TS:   nested.flat();
来源：http://wib.bbcook.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iuj.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://rme.jiagoushi.top

Ruby: nested.flatten
来源：http://kfu.xuetiantiany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kng.zhixingplan.top

[D19] 按字段分组
来源：http://wxw.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ggm.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dki.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kij.xingfuxueyuan.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://eor.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lww.nanxinkj.top

Go:   // 手写 map[string][]T
来源：http://pda.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tyn.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uni.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://aff.kuanghao11.cn

Py:   Counter(arr)
来源：http://yop.fehbvm.com

PHP:  array_count_values($arr);
来源：http://jbq.vehdjk.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cqv.sweek.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lnk.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kfy.guannengcc.top

Go:   // 手写 map[T]int
来源：http://nae.sjlbkw.cn

Ruby: arr.tally
来源：http://vkn.pycfn.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mwq.ydzc1.top

[D21] 判断是否包含某元素
来源：http://jvk.tarul.cn

Py:   x in arr
来源：http://jks.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://fmh.dianchejie.cn

JS:   arr.includes(x)
来源：http://nqu.hnqzz.top

TS:   arr.includes(x)
来源：http://lkk.ydjk.org.cn

Java: list.contains(x)
来源：http://gah.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://qjn.yj20258.top

Ruby: arr.include?(x)
来源：http://mnc.cqqwz.cn

C#:   list.Contains(x)
来源：http://uza.shzxlz.cn

[D22] 复制数组（避免共享引用）
来源：http://ozz.c1oappe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://elz.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fdl.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gve.sxryk.cn

TS:   [...arr];
来源：http://lkl.xinyue.icu

Java: new ArrayList<>(list);
来源：http://afo.epnwcf.com

Go:   copied := append([]int(nil), arr...)
来源：http://sit.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://etw.hnqzz.top

C#:   new List<int>(list);
来源：http://nct.feifeiyinyue.top

[D23] reduce 累积计算
来源：http://gbi.hysaishi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xrq.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lxk.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://osv.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lyu.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://egm.chenlongwang.top

Go:   // 手写循环
来源：http://qih.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rfm.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hfv.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://gru.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hjn.sysykeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mdd.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://asm.dianchejie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rqh.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zpk.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kyd.cheryme.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ygt.yuanzhike.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cvf.snrcjt.cn

[D25] Set 集合去重与交并差
来源：http://xdm.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vjo.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yqc.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://chw.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bps.svipenyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rbj.xinyue.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rli.cucudq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nyg.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rqb.zhoulong.xyz

[D26] 数组转字符串
来源：http://moj.52xcode.cn

Py:   ", ".join(map(str, arr))
来源：http://eik.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://kvt.snrcjt.cn

JS:   arr.join(", ")
来源：http://yvo.jianghu66.top

TS:   arr.join(", ")
来源：http://jss.redwolf501.top

Java: String.join(", ", list)
来源：http://vju.hysaishi.cn

Go:   strings.Join(strs, ", ")
来源：http://uia.guannengcc.top

Ruby: arr.join(", ")
来源：http://lgz.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://zkp.ybcxt.top

================================================================================
来源：http://nkh.jiagoushi.top

E. 字符串处理
来源：http://qin.jianghu66.top

================================================================================
来源：http://oqd.hongshengwenyu.top

[E01] 拼接字符串
来源：http://hib.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uxi.ybcxt.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ket.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sdk.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://agm.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ahj.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://geh.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://czs.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ikw.hywenlv.cn

[E02] 重复字符串
来源：http://tzk.chenjidiqi.icu

Py:   "ab" * 3
来源：http://pwy.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://urq.guannengcc.top

JS:   "ab".repeat(3)
来源：http://bxj.fehbvm.com

TS:   "ab".repeat(3)
来源：http://qhi.daria6918.cn

Java: "ab".repeat(3)
来源：http://iqk.hnqzz.top

Go:   strings.Repeat("ab", 3)
来源：http://njx.guannengcc.top

Ruby: "ab" * 3
来源：http://opl.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xui.iojbl.cn

[E03] 截取子串
来源：http://lus.quarkkingdee.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cko.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fvp.zhoulong.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://quy.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://imr.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://bot.jinyuanbaomall.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://atg.svipenyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ewg.xinyue.icu

C#:   s.Substring(1, 3)
来源：http://mag.yanxiufei.cn

[E04] 查找子串位置
来源：http://ayo.sysykeji.top

Py:   s.find("x");  s.index("x")
来源：http://arn.cucudq.cn

PHP:  strpos($s, "x");
来源：http://roa.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tfl.birdmap.top

TS:   s.indexOf("x")
来源：http://amc.nanxinkj.top

Java: s.indexOf("x")
来源：http://oqq.zhijiandao.cn

Go:   strings.Index(s, "x")
来源：http://xip.yvedp.cn

Ruby: s.index("x")
来源：http://wdl.meibo888.top

C#:   s.IndexOf("x")
来源：http://sum.dianchejie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vad.fanxiaobao.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kss.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aft.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lkc.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ica.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jnm.yonumen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cfs.nanxinkj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pax.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hdd.meibo888.top

[E06] 替换子串
来源：http://kqh.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jds.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://jio.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uwn.yuanzhike.top

TS:   s.replaceAll("a", "b")
来源：http://xaq.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://soy.cashguo.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xvs.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nxd.ivvv.top

C#:   s.Replace("a", "b")
来源：http://nlh.cqqwz.cn

[E07] 按分隔符拆分
来源：http://jyj.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mri.ehwqpu.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kso.andypj.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://bjk.cqqwz.cn

TS:   s.split(",")
来源：http://clq.hywenlv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://owo.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://czr.jinqigufen.top

Ruby: s.split(",");  s.split
来源：http://xpt.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mpi.aibaodan.cn

[E08] 数组按分隔符合并
来源：http://mlk.quarkkingdee.top

Py:   ",".join(items)
来源：http://wqj.hnqzz.top

PHP:  implode(",", $items);
来源：http://wyi.sjlbkw.cn

JS:   items.join(",")
来源：http://kob.wangshuangyany.cn

TS:   items.join(",")
来源：http://blu.chenlongwang.top

Java: String.join(",", items)
来源：http://btp.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://rxk.hfpthk.cn

Ruby: items.join(",")
来源：http://wom.gogol.net.cn

C#:   string.Join(",", items)
来源：http://baq.pycfn.com

[E09] 去除所有空白字符
来源：http://hfg.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zhk.hywenlv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ozv.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://zyx.ehwqpu.com

TS:   s.replace(/\s+/g, "")
来源：http://euf.xylfe.cn

Java: s.replaceAll("\\s+", "")
来源：http://rqo.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ick.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://mby.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rya.yj20258888.top

[E10] 左侧补零 / 定长填充
来源：http://htf.hfpthk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kpi.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ovl.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://tpj.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://chc.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://ows.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://jjl.jinyuanbaomall.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zij.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xbd.chenlongwang.top

[E11] 反转字符串
来源：http://cqg.hammf.cn

Py:   s[::-1]
来源：http://tit.jinqigfzy.top

PHP:  strrev($s);
来源：http://ngw.svipenyu.cn

JS:   [...s].reverse().join("")
来源：http://rzm.aizwys.cn

TS:   [...s].reverse().join("")
来源：http://jzu.c1oappe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ygb.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vxe.shuidangran.top

Ruby: s.reverse
来源：http://njz.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://uqt.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://uib.316326.xyz

Py:   s.count("a")
来源：http://ark.fengsongda.top

PHP:  substr_count($s, "a");
来源：http://oio.zhiwuduotai.top

JS:   s.split("a").length - 1
来源：http://blc.pycfn.com

TS:   s.split("a").length - 1
来源：http://cek.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fpd.yj20258888.top

Go:   strings.Count(s, "a")
来源：http://rmy.yangfankeji.com

Ruby: s.count("a")
来源：http://vkn.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://ffe.yuanzhike.top

[E13] 逐字符遍历
来源：http://hia.hammf.cn

Py:   for ch in s: print(ch)
来源：http://fgq.xziqi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://soq.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://axu.zhiwuduotai.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sdm.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ohb.9152youxi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mag.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bfy.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xwh.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://mri.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ucg.ydjk.org.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hbu.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rit.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dmi.yonumen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dhs.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tvp.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ooa.shangyingyoupin.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xuo.zhengqikj.top

[E15] HTML 转义 / 反转义
来源：http://jje.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kbs.wangdashe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pzw.chenzaomai.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mgh.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ogz.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://azc.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ooq.iojbl.cn


<!-- 参考信息 -->