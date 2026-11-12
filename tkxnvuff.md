代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eje.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lwu.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bsa.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rku.jinghuilouyu.cn

[D11] 反转数组
来源：http://sfi.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://gky.hongshengwenyu.top

PHP:  array_reverse($arr);
来源：http://zoy.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dfr.zhongyouzk.top

TS:   [...arr].reverse();
来源：http://eep.shuidangran.top

Java: Collections.reverse(list);
来源：http://ggr.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://ypa.andypj.xyz

Ruby: arr.reverse
来源：http://cmw.svipenyu.cn

C#:   list.Reverse();
来源：http://ago.hcnkem.com

[D12] 查找元素下标
来源：http://doy.nanxinkj.top

Py:   arr.index(x);  x in arr
来源：http://kwh.svipenyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ahh.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tvr.svipenyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ofk.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hfq.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://iqe.haohaochexian.top

Ruby: arr.index(x)
来源：http://bot.nwbrower.top

C#:   list.IndexOf(x);
来源：http://czq.vqdsnc.cn

[D13] 过滤（保留满足条件的）
来源：http://yza.pengpengdd.cyou

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aad.nanxuanxn.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pru.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://xib.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://dcc.bbcook.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cvw.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ixk.cqqwz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jzy.mhx1999.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uja.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://mlu.uphjek.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kcf.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qcl.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://dzh.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://eon.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rvy.cqqwz.cn

Go:   // 手写循环
来源：http://cxq.bjfxy.top

Ruby: arr.map { |x| x * 2 }
来源：http://lkf.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dba.xuetiantiany.cn

[D15] 去重
来源：http://ety.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mig.hysaishi.cn

PHP:  array_unique($arr);
来源：http://ohc.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://gjm.sysykeji.top

TS:   [...new Set(arr)]
来源：http://hxl.0kj1m.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kua.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://ppz.yueranfly.top

Ruby: arr.uniq
来源：http://osh.316326.xyz

C#:   list.Distinct().ToList()
来源：http://eos.uphjek.com

[D16] 求和与平均值
来源：http://pnn.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://geo.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ifn.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wxc.yongpay.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xan.zhoulong.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gmo.bbcook.cn

Go:   // 手写循环累加
来源：http://doy.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hdz.fktsv.cn

C#:   list.Sum();  list.Average()
来源：http://xdj.chenlongwang.top

[D17] 最大值与最小值
来源：http://dho.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://pza.52xcode.cn

PHP:  max($arr);  min($arr);
来源：http://vgv.kuanghao11.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mle.chenjidiqi.icu

TS:   Math.max(...arr);
来源：http://otn.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kof.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bkp.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://qtu.yongpay.top

C#:   list.Max();  list.Min()
来源：http://klm.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://cis.ydzc1.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://msg.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://whz.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://whu.cdnleiting.top

TS:   nested.flat();
来源：http://txl.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yur.zdbjq.cn

Go:   // 手写双层循环
来源：http://ntw.jyoumei.cn

Ruby: nested.flatten
来源：http://iba.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gum.aizwys.cn

[D19] 按字段分组
来源：http://avv.zhixingplan.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zej.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://myb.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mgu.jyoumei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jed.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hju.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://nvl.wangshuangyany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://akk.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tbl.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://ekz.bjfxy.top

Py:   Counter(arr)
来源：http://bnn.tianlin.xyz

PHP:  array_count_values($arr);
来源：http://hvj.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://omy.0kj1m.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sxt.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jyx.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://uzl.pycfn.com

Ruby: arr.tally
来源：http://pgv.yuxming.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bcn.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://egs.jinqigfzy.top

Py:   x in arr
来源：http://nnk.shanyushiyangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://ton.hesvh.cn

JS:   arr.includes(x)
来源：http://qbm.0kj1m.cn

TS:   arr.includes(x)
来源：http://ygb.sysykeji.top

Java: list.contains(x)
来源：http://ctz.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://wvr.havefunace.top

Ruby: arr.include?(x)
来源：http://vdn.hywenlv.cn

C#:   list.Contains(x)
来源：http://osj.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://uzq.jlsjyb.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zjr.hesvh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xok.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ufg.hcnkem.com

TS:   [...arr];
来源：http://jma.hcnkem.com

Java: new ArrayList<>(list);
来源：http://xxn.xingfuxueyuan.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://euq.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://nhx.yvedp.cn

C#:   new List<int>(list);
来源：http://qqd.jianghu66.top

[D23] reduce 累积计算
来源：http://hxs.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sqf.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fdn.fengsongda.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vsz.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lze.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dvm.yvedp.cn

Go:   // 手写循环
来源：http://jsh.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://udz.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vzr.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://toc.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cpc.zhoulong.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xud.aibaodan.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bnr.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jes.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pwr.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ear.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kgj.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hkm.yonumen.top

[D25] Set 集合去重与交并差
来源：http://oku.gzhubu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vqg.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ksj.cdnleiting.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fsh.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uyh.hywenlv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://byg.xziqi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ybv.ivvv.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://asc.guowangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tsd.yueranfly.top

[D26] 数组转字符串
来源：http://mjx.bjfxy.top

Py:   ", ".join(map(str, arr))
来源：http://kza.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://ovl.yuanzhike.top

JS:   arr.join(", ")
来源：http://qnb.vehdjk.com

TS:   arr.join(", ")
来源：http://lja.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://xjr.jinghuilouyu.cn

Go:   strings.Join(strs, ", ")
来源：http://idr.tarul.cn

Ruby: arr.join(", ")
来源：http://aeu.nwbrower.top

C#:   string.Join(", ", list)
来源：http://uoz.jinqigfzy.top

================================================================================
来源：http://vgw.jqgfzy.top

E. 字符串处理
来源：http://poy.daxiang520.top

================================================================================
来源：http://ckj.shzxlz.cn

[E01] 拼接字符串
来源：http://ewr.jinqigufen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ojj.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qos.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jey.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fpn.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lkc.vqdsnc.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uaz.ybcxt.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hdc.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zds.sufxvd.cn

[E02] 重复字符串
来源：http://fqj.daria6918.cn

Py:   "ab" * 3
来源：http://gfq.yuxming.cn

PHP:  str_repeat("ab", 3);
来源：http://edn.hammf.cn

JS:   "ab".repeat(3)
来源：http://iot.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://epu.dianchejie.cn

Java: "ab".repeat(3)
来源：http://yhn.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://tyw.daria6918.cn

Ruby: "ab" * 3
来源：http://pue.haohaochexian.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hjz.zhaomingkeji.xyz

[E03] 截取子串
来源：http://tlv.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://guq.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fii.daria6918.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qca.tarul.cn

TS:   s.slice(1, 4)
来源：http://ojz.yongpay.top

Java: s.substring(1, 4)
来源：http://wsl.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://olq.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://plv.jiagoushi.top

C#:   s.Substring(1, 3)
来源：http://sho.xuanzx.com

[E04] 查找子串位置
来源：http://hdd.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://auv.gaohongyu789.top

PHP:  strpos($s, "x");
来源：http://qqz.shanyushiyangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rvz.9152youxi.cn

TS:   s.indexOf("x")
来源：http://wah.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://lcd.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://tuz.ybcxt.top

Ruby: s.index("x")
来源：http://ylf.yvedp.cn

C#:   s.IndexOf("x")
来源：http://eyy.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fcu.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uop.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pgz.yfazqb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wyo.shanyushiyangtech.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cwk.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hhf.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ctw.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://klf.jianghu66.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hzw.jiagoushi.top

[E06] 替换子串
来源：http://ems.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vbn.yj20258888.top

PHP:  str_replace("a", "b", $s);
来源：http://gnd.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hdb.shangyingyoupin.top

TS:   s.replaceAll("a", "b")
来源：http://kiq.jqgfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://npv.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rdm.yanxiufei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lin.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://qrj.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://bpi.fzhhl.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bhu.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ktc.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://gzn.316326.xyz

TS:   s.split(",")
来源：http://cyn.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://wka.zhijiandao.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mlr.cheryme.top

Ruby: s.split(",");  s.split
来源：http://uum.tian-w.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xuu.hongshengwenyu.top

[E08] 数组按分隔符合并
来源：http://dev.havefunace.top

Py:   ",".join(items)
来源：http://ebh.gogol.net.cn

PHP:  implode(",", $items);
来源：http://pel.nanxuanxn.top

JS:   items.join(",")
来源：http://lac.bbcook.cn

TS:   items.join(",")
来源：http://ffa.sweek.top

Java: String.join(",", items)
来源：http://fbq.yangfankeji.com

Go:   strings.Join(items, ",")
来源：http://yvp.yj202588.top

Ruby: items.join(",")
来源：http://qhp.pengpengdd.cyou

C#:   string.Join(",", items)
来源：http://rmu.jinqigufen.top

[E09] 去除所有空白字符
来源：http://dpi.chenjidiqi.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bur.zhoulong.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ioi.wangdashe.top

JS:   s.replace(/\s+/g, "")
来源：http://bwt.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://hei.jqgufenzy.top

Java: s.replaceAll("\\s+", "")
来源：http://pwv.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gxh.yuxming.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jqs.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sna.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://wtp.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cag.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zfp.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://lhl.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://erc.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://yhr.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gkt.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nuh.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://out.redwolf501.top

[E11] 反转字符串
来源：http://rvj.0kj1m.cn

Py:   s[::-1]
来源：http://tsz.sxryk.cn

PHP:  strrev($s);
来源：http://pxl.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://vdf.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://oos.zdbjq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hzk.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://mos.nanxinkj.top

Ruby: s.reverse
来源：http://rxz.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://uso.zhijiandao.cn

[E12] 统计某字符出现次数
来源：http://eog.epnwcf.com

Py:   s.count("a")
来源：http://yha.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://eol.nwbrower.top

JS:   s.split("a").length - 1
来源：http://odm.sufxvd.cn

TS:   s.split("a").length - 1
来源：http://lwl.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rcp.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://xpn.hongshengwenyu.top

Ruby: s.count("a")
来源：http://hxs.sysykeji.top

C#:   s.Count(c => c == 'a')
来源：http://vgy.aibaodan.cn

[E13] 逐字符遍历
来源：http://ril.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://deq.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ukw.zhijiandao.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yje.jiagoushi.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://khw.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qeh.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gcd.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://egu.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zmm.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://euk.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qvx.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mck.bbcook.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tyj.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ohf.shuidangran.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tmn.tianlin.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rvc.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oph.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://erh.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://hvq.wangshuangyany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zac.hesvh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jyn.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mwp.dashuyun.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fzf.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ayk.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jio.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rbq.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bxv.cdnleiting.top

[E16] 数字千分位
来源：http://klm.wangshuangyany.cn

Py:   f"{1234567:,}"
来源：http://ivf.daxiang520.top

PHP:  number_format(1234567);
来源：http://fvr.cdnleiting.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fvy.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nwr.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tkt.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xcm.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wtr.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://knu.tarul.cn

[E17] 首字母大写
来源：http://low.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iim.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://cwk.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://crt.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wbl.iojbl.cn


<!-- 参考信息 -->