代发 wailian999

C#:   list.Reverse();
来源：http://piw.jlsjyb.cn

[D12] 查找元素下标
来源：http://qkx.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://ajm.havefunace.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zcv.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zgo.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pbv.yanxiufei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://koi.yj202588.top

Go:   slices.Index(arr, x)
来源：http://kli.ctjpmb.com

Ruby: arr.index(x)
来源：http://ctp.zdqjudy.top

C#:   list.IndexOf(x);
来源：http://cfx.shanyushiyangtech.top

[D13] 过滤（保留满足条件的）
来源：http://btw.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xbs.yvedp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zrk.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://bjf.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://bee.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ban.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bhh.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oay.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qde.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://kyi.zhijiandao.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zil.yj20258888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vlv.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://nrs.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://rgo.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://eht.snrcjt.cn

Go:   // 手写循环
来源：http://dnq.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://vba.yangfankeji.com

C#:   list.Select(x => x * 2).ToList()
来源：http://syx.pycfn.com

[D15] 去重
来源：http://vgt.yanxiufei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lbl.ppjwa.cn

PHP:  array_unique($arr);
来源：http://ore.yonumen.top

JS:   [...new Set(arr)]
来源：http://yph.fengsongda.top

TS:   [...new Set(arr)]
来源：http://bby.jqgufenzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kig.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://uyc.dashuyun.cn

Ruby: arr.uniq
来源：http://ljv.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://rak.chenjidiqi.icu

[D16] 求和与平均值
来源：http://zns.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vnr.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kac.nanxinkj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://khn.ydzc1.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fxf.gzhubu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hti.redwolf501.top

Go:   // 手写循环累加
来源：http://jcv.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://grt.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://def.xuetiantiany.cn

[D17] 最大值与最小值
来源：http://urq.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://koe.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://uwn.wangdashe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cot.fktsv.cn

TS:   Math.max(...arr);
来源：http://tdg.shuidangran.top

Java: Collections.max(list);  Collections.min(list);
来源：http://twv.nanxuanxn.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ysr.316326.xyz

Ruby: arr.max;  arr.min
来源：http://ozl.xuanzx.com

C#:   list.Max();  list.Min()
来源：http://xfp.tian-w.cn

[D18] 扁平化嵌套数组
来源：http://uow.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ljh.tian-w.cn

PHP:  array_merge(...$nested);
来源：http://wic.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ted.gaohongyu789.top

TS:   nested.flat();
来源：http://hxj.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pxu.hcnkem.com

Go:   // 手写双层循环
来源：http://ife.fktsv.cn

Ruby: nested.flatten
来源：http://cqk.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ahu.guannengcc.top

[D19] 按字段分组
来源：http://cty.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aml.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://evw.xuetiantiany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vqz.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://bbe.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://atl.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://wzg.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lqq.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://erx.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://uce.jlsjyb.cn

Py:   Counter(arr)
来源：http://gwu.vehdjk.com

PHP:  array_count_values($arr);
来源：http://pct.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jte.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xse.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bba.shangyingyoupin.top

Go:   // 手写 map[T]int
来源：http://zwd.chenjidiqi.icu

Ruby: arr.tally
来源：http://pat.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://clu.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://koj.shangyingyoupin.top

Py:   x in arr
来源：http://nhz.ywan-chungtsiang.top

PHP:  in_array($x, $arr, true);
来源：http://ypk.chenzaomai.com

JS:   arr.includes(x)
来源：http://ynq.zhijiandao.cn

TS:   arr.includes(x)
来源：http://esh.pycfn.com

Java: list.contains(x)
来源：http://vdo.yj20258888.top

Go:   slices.Contains(arr, x)
来源：http://mys.hysaishi.cn

Ruby: arr.include?(x)
来源：http://xlx.jlsjyb.cn

C#:   list.Contains(x)
来源：http://wnx.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://eux.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xwx.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lyd.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gyb.cucudq.cn

TS:   [...arr];
来源：http://tlx.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://uzc.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mgc.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://rlw.smart0.xyz

C#:   new List<int>(list);
来源：http://pfb.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://ooq.cheryme.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ohv.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://swe.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qof.sufxvd.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cwe.smart0.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://kpo.dianchejie.cn

Go:   // 手写循环
来源：http://xqr.daria6918.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://anz.fengsongda.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://egk.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://jcd.xinyue.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wdr.chenzaomai.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vmj.dianchejie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pyb.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yvx.ehwqpu.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dxu.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qnu.mhx1999.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fqr.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://end.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://zdm.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rxs.hesvh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mle.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://irf.jinyuanbaomall.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kbf.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pxp.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mnb.hesvh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jxn.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ert.fktsv.cn

[D26] 数组转字符串
来源：http://hbi.meibo888.top

Py:   ", ".join(map(str, arr))
来源：http://xiy.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://xwa.yvedp.cn

JS:   arr.join(", ")
来源：http://vsm.jinqigufen.top

TS:   arr.join(", ")
来源：http://uxt.yj202588.top

Java: String.join(", ", list)
来源：http://bbv.shuidangran.top

Go:   strings.Join(strs, ", ")
来源：http://eee.fzhhl.top

Ruby: arr.join(", ")
来源：http://sem.birdmap.top

C#:   string.Join(", ", list)
来源：http://qrf.zhongyouzk.top

================================================================================
来源：http://nhq.nanxinkj.top

E. 字符串处理
来源：http://qcw.meibo888.top

================================================================================
来源：http://zwr.hongshengwenyu.top

[E01] 拼接字符串
来源：http://scg.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sjm.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xne.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://die.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ofh.sweek.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wlj.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://imm.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gop.tianlin.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uot.ctjpmb.com

[E02] 重复字符串
来源：http://ipr.yanxiufei.cn

Py:   "ab" * 3
来源：http://qoo.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://zyv.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://rtx.hcnkem.com

TS:   "ab".repeat(3)
来源：http://lly.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://pbk.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://ddi.shuidangran.top

Ruby: "ab" * 3
来源：http://viw.guowangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xdn.redwolf501.top

[E03] 截取子串
来源：http://cca.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bar.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://buy.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rga.shuidangran.top

TS:   s.slice(1, 4)
来源：http://ubk.tarul.cn

Java: s.substring(1, 4)
来源：http://osh.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xeg.jinqigufen.top

Ruby: s[1, 3];  s[1..3]
来源：http://ovq.hammf.cn

C#:   s.Substring(1, 3)
来源：http://sfv.kuanghao11.cn

[E04] 查找子串位置
来源：http://ami.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://fkq.bbcook.cn

PHP:  strpos($s, "x");
来源：http://kzz.ybcxt.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nyd.zhongyouzk.top

TS:   s.indexOf("x")
来源：http://qod.hnqzz.top

Java: s.indexOf("x")
来源：http://hnd.bbcook.cn

Go:   strings.Index(s, "x")
来源：http://ufu.cqqwz.cn

Ruby: s.index("x")
来源：http://joa.sweek.top

C#:   s.IndexOf("x")
来源：http://vtb.c1oappe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://war.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://adp.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ahe.meibo888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jue.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://odk.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zkq.hnxiangtu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nwf.zhaomingkeji.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://leg.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://syr.ywan-chungtsiang.top

[E06] 替换子串
来源：http://vhj.ppjwa.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bnm.birdmap.top

PHP:  str_replace("a", "b", $s);
来源：http://uup.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://juj.birdmap.top

TS:   s.replaceAll("a", "b")
来源：http://gvi.xuetiantiany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eim.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wpb.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nyi.hammf.cn

C#:   s.Replace("a", "b")
来源：http://lec.zdqjudy.top

[E07] 按分隔符拆分
来源：http://kws.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pgd.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dmf.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dyz.ydzc1.top

TS:   s.split(",")
来源：http://lwx.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://plf.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yms.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://oqn.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ati.guannengcc.top

[E08] 数组按分隔符合并
来源：http://gyy.yj20258.top

Py:   ",".join(items)
来源：http://dih.tarul.cn

PHP:  implode(",", $items);
来源：http://pde.hcnkem.com

JS:   items.join(",")
来源：http://ymp.guowangkeji.top

TS:   items.join(",")
来源：http://vxv.daxiang520.top

Java: String.join(",", items)
来源：http://dep.yuanzhike.top

Go:   strings.Join(items, ",")
来源：http://rtb.jianghu66.top

Ruby: items.join(",")
来源：http://ktt.jqgfzy.top

C#:   string.Join(",", items)
来源：http://tpb.xinyue.icu

[E09] 去除所有空白字符
来源：http://zur.uphjek.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ukb.pycfn.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wni.fehbvm.com

JS:   s.replace(/\s+/g, "")
来源：http://zve.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://ptk.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://ptt.yj20258888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://idx.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://sbl.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://goj.daria6918.cn

[E10] 左侧补零 / 定长填充
来源：http://tom.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tss.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dgz.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://rpq.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://eki.hammf.cn

Java: String.format("%03d", 7)
来源：http://oey.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://ndf.hywenlv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wmw.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zxt.svipenyu.cn

[E11] 反转字符串
来源：http://bnv.nanxuanxn.top

Py:   s[::-1]
来源：http://ezo.zhiwuduotai.top

PHP:  strrev($s);
来源：http://ngw.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://lvy.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://kdq.cashguo.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uuw.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://neq.yj202588.top

Ruby: s.reverse
来源：http://luu.hammf.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qpo.yfazqb.com

[E12] 统计某字符出现次数
来源：http://eae.fzhhl.top

Py:   s.count("a")
来源：http://ava.hammf.cn

PHP:  substr_count($s, "a");
来源：http://lrw.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://ghk.cashguo.top

TS:   s.split("a").length - 1
来源：http://hnw.tanke756.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gtq.tanke756.top

Go:   strings.Count(s, "a")
来源：http://rwm.zycfv.cn

Ruby: s.count("a")
来源：http://bbm.fengsongda.top

C#:   s.Count(c => c == 'a')
来源：http://htz.yj20258.top

[E13] 逐字符遍历
来源：http://krr.yj202588.top

Py:   for ch in s: print(ch)
来源：http://pnk.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lhn.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://cci.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://vuo.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cqj.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kvv.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nuo.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hfr.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://hzi.vehdjk.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pnx.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://otg.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dey.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ssq.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hrp.kuanghao11.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bmo.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nww.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jso.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://kvy.meibo888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://udt.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://esw.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cbl.jinghuilouyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://czj.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://klc.sufxvd.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ibn.yueranfly.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fmg.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nsb.kuanghao11.cn

[E16] 数字千分位
来源：http://kbq.aizwys.cn

Py:   f"{1234567:,}"
来源：http://rcx.daria6918.cn

PHP:  number_format(1234567);
来源：http://son.yj20258888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qnk.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vsi.shanyushiyangtech.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://isx.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://meb.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pjz.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://iih.yueranfly.top

[E17] 首字母大写
来源：http://zbe.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vdb.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://jnm.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ymz.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qzg.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dbq.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eln.feifeiyinyue.top

Ruby: s.capitalize
来源：http://sxq.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yvv.yueranfly.top

[E18] 模板占位符替换
来源：http://mha.yongpay.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iyv.xylfe.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vnh.pengpengdd.cyou

JS:   tpl.replaceAll("{name}", name)
来源：http://vgy.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mqv.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fkt.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qnq.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lwm.aibaodan.cn


<!-- 参考信息 -->