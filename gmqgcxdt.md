代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jaa.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ewi.tarul.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nhu.meibo888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qub.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qog.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wta.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mrd.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dvc.zhongyouzk.top

[D11] 反转数组
来源：http://puz.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://row.xingfuxueyuan.xyz

PHP:  array_reverse($arr);
来源：http://kxx.hcnkem.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hkq.nanxuanxn.top

TS:   [...arr].reverse();
来源：http://bpz.ydjk.org.cn

Java: Collections.reverse(list);
来源：http://wfc.fehbvm.com

Go:   slices.Reverse(arr)
来源：http://tvd.zhixingplan.top

Ruby: arr.reverse
来源：http://hqm.havefunace.top

C#:   list.Reverse();
来源：http://nml.mhx1999.top

[D12] 查找元素下标
来源：http://qrl.iojbl.cn

Py:   arr.index(x);  x in arr
来源：http://raz.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dyl.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eix.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fer.0kj1m.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wja.jinqigufen.top

Go:   slices.Index(arr, x)
来源：http://zta.haohaochexian.top

Ruby: arr.index(x)
来源：http://jnt.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://izv.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://lpg.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qzp.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sdn.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://vtx.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://kob.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kvg.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://emo.zhixingplan.top

Ruby: arr.select { |x| x > 3 }
来源：http://lmo.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hye.zdbjq.cn

[D14] 映射转换（每个元素变形）
来源：http://tur.jinghuilouyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vgm.snrcjt.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nku.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://hwc.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://jot.daria6918.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://psw.zdqjudy.top

Go:   // 手写循环
来源：http://vzp.jinghuilouyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fva.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jyj.cucudq.cn

[D15] 去重
来源：http://iat.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jjm.gzhubu.top

PHP:  array_unique($arr);
来源：http://wll.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://cgr.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://uig.xuanzx.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zoo.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cri.nanxuanxn.top

Ruby: arr.uniq
来源：http://gum.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://tcw.c1oappe.top

[D16] 求和与平均值
来源：http://nmc.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jxn.redwolf501.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jgt.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ivw.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://txx.sysykeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://and.wangdashe.top

Go:   // 手写循环累加
来源：http://oqp.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zqu.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://sqc.fktsv.cn

[D17] 最大值与最小值
来源：http://dkk.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://lvg.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://dip.xylfe.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://onf.fzhhl.top

TS:   Math.max(...arr);
来源：http://aol.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hkw.birdmap.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ome.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://aov.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://iau.wangshuangyany.cn

[D18] 扁平化嵌套数组
来源：http://jlz.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bpf.gogol.net.cn

PHP:  array_merge(...$nested);
来源：http://ejx.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mqi.zhongyouzk.top

TS:   nested.flat();
来源：http://vzm.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nog.guowangkeji.top

Go:   // 手写双层循环
来源：http://xrr.uphjek.com

Ruby: nested.flatten
来源：http://kcy.birdmap.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kjs.cucudq.cn

[D19] 按字段分组
来源：http://qhf.tian-w.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xos.xuetiantiany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xfc.zhongyouzk.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dnq.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://enc.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gda.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://pek.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jzr.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aux.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://dmh.shuidangran.top

Py:   Counter(arr)
来源：http://pbq.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://ghx.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uoj.gzhubu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ehc.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pvi.xylfe.cn

Go:   // 手写 map[T]int
来源：http://awk.zhijiandao.cn

Ruby: arr.tally
来源：http://hio.yj20258888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://did.hywenlv.cn

[D21] 判断是否包含某元素
来源：http://nxz.mhx1999.top

Py:   x in arr
来源：http://vci.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://qkc.zhongyouzk.top

JS:   arr.includes(x)
来源：http://awc.yfazqb.com

TS:   arr.includes(x)
来源：http://soh.sxryk.cn

Java: list.contains(x)
来源：http://szx.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://qrx.shangyingyoupin.top

Ruby: arr.include?(x)
来源：http://zca.sufxvd.cn

C#:   list.Contains(x)
来源：http://udn.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://gzc.tian-w.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xac.feifeiyinyue.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uvc.sxryk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xwn.sjlbkw.cn

TS:   [...arr];
来源：http://xuj.cqqwz.cn

Java: new ArrayList<>(list);
来源：http://xxu.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://xoe.iojbl.cn

Ruby: arr.dup;  arr.clone
来源：http://swb.ybcxt.top

C#:   new List<int>(list);
来源：http://edk.yanxiufei.cn

[D23] reduce 累积计算
来源：http://ynk.ybcxt.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://peq.zdqjudy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kdc.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hxp.guannengcc.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tok.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pzo.shzxlz.cn

Go:   // 手写循环
来源：http://ssn.smart0.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rmf.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rfk.cdnleiting.top

[D24] 字典 / Map 基本操作
来源：http://kym.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ehi.jianghu66.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zgj.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kbs.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vrl.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tsd.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zxt.epnwcf.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kln.jqgfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wlx.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://cxs.bbcook.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jsv.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vha.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nso.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qvl.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dlf.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ufd.jinyuanbaomall.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://czx.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ois.fengsongda.top

[D26] 数组转字符串
来源：http://csx.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://yar.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://acg.jqgufenzy.top

JS:   arr.join(", ")
来源：http://vgl.bbcook.cn

TS:   arr.join(", ")
来源：http://sue.sysykeji.top

Java: String.join(", ", list)
来源：http://cbv.hammf.cn

Go:   strings.Join(strs, ", ")
来源：http://epj.guannengcc.top

Ruby: arr.join(", ")
来源：http://ide.hysaishi.cn

C#:   string.Join(", ", list)
来源：http://xke.feifeiyinyue.top

================================================================================
来源：http://hcz.andypj.xyz

E. 字符串处理
来源：http://ydg.chenlongwang.top

================================================================================
来源：http://lbw.hfpthk.cn

[E01] 拼接字符串
来源：http://zdk.ydzc1.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ufn.jianghu66.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xlh.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hjq.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rls.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cut.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qqf.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qly.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pnm.nanxuanxn.top

[E02] 重复字符串
来源：http://mfg.yongpay.top

Py:   "ab" * 3
来源：http://vcg.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://yjh.feifeiyinyue.top

JS:   "ab".repeat(3)
来源：http://qmg.9152youxi.cn

TS:   "ab".repeat(3)
来源：http://sxq.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://guw.xuetiantiany.cn

Go:   strings.Repeat("ab", 3)
来源：http://nyg.dianchejie.cn

Ruby: "ab" * 3
来源：http://obz.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jyg.feifeiyinyue.top

[E03] 截取子串
来源：http://boh.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fev.shanyushiyangtech.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wbz.c1oappe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lbm.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://ead.nanxuanxn.top

Java: s.substring(1, 4)
来源：http://jfn.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zbk.aibaodan.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zbf.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://fiq.pengpengdd.cyou

[E04] 查找子串位置
来源：http://ibd.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://vkg.yj20258888.top

PHP:  strpos($s, "x");
来源：http://eeg.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zqk.jianghu66.top

TS:   s.indexOf("x")
来源：http://ddu.daxiang520.top

Java: s.indexOf("x")
来源：http://egb.gogol.net.cn

Go:   strings.Index(s, "x")
来源：http://abi.aizwys.cn

Ruby: s.index("x")
来源：http://uww.316326.xyz

C#:   s.IndexOf("x")
来源：http://myf.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qtq.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aag.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eah.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://scb.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ylt.andypj.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://twm.gaohongyu789.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aop.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cjh.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zez.yj20258.top

[E06] 替换子串
来源：http://gxm.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xdu.daria6918.cn

PHP:  str_replace("a", "b", $s);
来源：http://jnv.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hbs.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://gmj.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://anh.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://adm.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dut.gaohongyu789.top

C#:   s.Replace("a", "b")
来源：http://ueh.ctjpmb.com

[E07] 按分隔符拆分
来源：http://snj.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lvz.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pok.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://hks.feifeiyinyue.top

TS:   s.split(",")
来源：http://eje.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://eow.hysaishi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rrh.yuxming.cn

Ruby: s.split(",");  s.split
来源：http://upu.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vrk.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://lmx.vehdjk.com

Py:   ",".join(items)
来源：http://xwe.bbcook.cn

PHP:  implode(",", $items);
来源：http://vqg.jianghu66.top

JS:   items.join(",")
来源：http://qqg.dianchejie.cn

TS:   items.join(",")
来源：http://lmg.jyoumei.cn

Java: String.join(",", items)
来源：http://uqz.pycfn.com

Go:   strings.Join(items, ",")
来源：http://gam.hammf.cn

Ruby: items.join(",")
来源：http://mrp.hesvh.cn

C#:   string.Join(",", items)
来源：http://xiq.zhijiandao.cn

[E09] 去除所有空白字符
来源：http://lfi.zhengqikj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vgj.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tbf.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://umv.xziqi.cn

TS:   s.replace(/\s+/g, "")
来源：http://uco.wangshuangyany.cn

Java: s.replaceAll("\\s+", "")
来源：http://jwn.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xsx.hnxiangtu.top

Ruby: s.gsub(/\s+/, "")
来源：http://wym.jyoumei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hvm.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://dka.fehbvm.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://prg.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://svr.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://eeg.tanke756.top

TS:   "7".padStart(3, "0")
来源：http://cbr.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://ihz.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mfp.zhijiandao.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://car.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wsn.hywenlv.cn

[E11] 反转字符串
来源：http://ztz.cucudq.cn

Py:   s[::-1]
来源：http://dbw.hnxiangtu.top

PHP:  strrev($s);
来源：http://kao.birdmap.top

JS:   [...s].reverse().join("")
来源：http://epc.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://fva.fanxiaobao.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://eni.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://egs.xylfe.cn

Ruby: s.reverse
来源：http://gmu.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://omn.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://rez.hysaishi.cn

Py:   s.count("a")
来源：http://wej.jiagoushi.top

PHP:  substr_count($s, "a");
来源：http://mhl.hcnkem.com

JS:   s.split("a").length - 1
来源：http://vnb.hnqzz.top

TS:   s.split("a").length - 1
来源：http://ekx.yj20258.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ukb.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://rnm.ydzc1.top

Ruby: s.count("a")
来源：http://jwn.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://zul.daxiang520.top

[E13] 逐字符遍历
来源：http://mcf.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://xch.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ouv.zhijiandao.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gsu.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pwf.dianchejie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yfo.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bjt.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://evb.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://adh.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://igs.zdbjq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jgg.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://svs.yj20258888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kbd.sysykeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gcf.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ggs.vehdjk.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qdv.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gmd.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gud.jyoumei.cn

[E15] HTML 转义 / 反转义
来源：http://isg.dashuyun.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bna.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zmw.c1oappe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uty.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ozl.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kzt.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vfm.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wtd.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vke.yangfankeji.com

[E16] 数字千分位
来源：http://ijs.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://bns.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://ksv.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://inw.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://adh.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mtb.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tnk.vehdjk.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lhu.sweek.top

C#:   1234567.ToString("N0")
来源：http://cvo.shuidangran.top

[E17] 首字母大写
来源：http://rhw.zhoulong.xyz


<!-- 参考信息 -->