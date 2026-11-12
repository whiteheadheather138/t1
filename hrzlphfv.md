代发 wailian999

C#:   list.Reverse();
来源：http://ylc.ydjk.org.cn

[D12] 查找元素下标
来源：http://ees.vqdsnc.cn

Py:   arr.index(x);  x in arr
来源：http://wff.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vwh.zhengqikj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jxf.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ska.haohaochexian.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nfa.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://bpg.bbcook.cn

Ruby: arr.index(x)
来源：http://nfq.wangdashe.top

C#:   list.IndexOf(x);
来源：http://vjx.zhongyouzk.top

[D13] 过滤（保留满足条件的）
来源：http://onf.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pxn.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vwa.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://djf.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://hob.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dnd.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://czi.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://pmf.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wrt.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://wez.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ims.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wum.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://wfq.zhaomingkeji.xyz

TS:   arr.map(x => x * 2)
来源：http://wkg.pycfn.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://nnz.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://quc.ybcxt.top

Ruby: arr.map { |x| x * 2 }
来源：http://tko.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rdm.tian-w.cn

[D15] 去重
来源：http://gqg.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dtz.xylfe.cn

PHP:  array_unique($arr);
来源：http://gmr.hesvh.cn

JS:   [...new Set(arr)]
来源：http://lxz.yj20258.top

TS:   [...new Set(arr)]
来源：http://ynv.epnwcf.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hkr.jiagoushi.top

Go:   // 用 map[T]struct{} 手写
来源：http://kig.xylfe.cn

Ruby: arr.uniq
来源：http://snt.zdbjq.cn

C#:   list.Distinct().ToList()
来源：http://juy.fengsongda.top

[D16] 求和与平均值
来源：http://uen.wangdashe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zsi.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ntf.birdmap.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://isf.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tkj.fktsv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://awo.ydzc1.top

Go:   // 手写循环累加
来源：http://rxp.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mvi.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://uzf.snrcjt.cn

[D17] 最大值与最小值
来源：http://qyq.havefunace.top

Py:   max(arr);  min(arr)
来源：http://ndn.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://wdx.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ryj.iojbl.cn

TS:   Math.max(...arr);
来源：http://jpj.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mbo.ydzc1.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gzd.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://bth.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://cfi.tarul.cn

[D18] 扁平化嵌套数组
来源：http://wer.jlsjyb.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yaq.tanke756.top

PHP:  array_merge(...$nested);
来源：http://yhk.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wkh.uphjek.com

TS:   nested.flat();
来源：http://heu.smart0.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wco.pengpengdd.cyou

Go:   // 手写双层循环
来源：http://ams.dashuyun.cn

Ruby: nested.flatten
来源：http://url.zhiwuduotai.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ddn.shangyingyoupin.top

[D19] 按字段分组
来源：http://pku.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lwv.nwbrower.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oke.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fse.zdbjq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hdf.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gov.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://eai.fehbvm.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://onj.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vid.yuxming.cn

[D20] 统计每个元素出现次数
来源：http://fzj.zhixingplan.top

Py:   Counter(arr)
来源：http://kaw.bjfxy.top

PHP:  array_count_values($arr);
来源：http://vqe.fktsv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tzi.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yul.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mwu.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://ihb.hysaishi.cn

Ruby: arr.tally
来源：http://pyq.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://unl.aizwys.cn

[D21] 判断是否包含某元素
来源：http://fyu.bbcook.cn

Py:   x in arr
来源：http://gmv.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://nxg.snrcjt.cn

JS:   arr.includes(x)
来源：http://gjs.hcnkem.com

TS:   arr.includes(x)
来源：http://tlw.chenjidiqi.icu

Java: list.contains(x)
来源：http://aka.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://byo.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://sts.ivvv.top

C#:   list.Contains(x)
来源：http://vye.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://mej.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hzd.gogol.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://coy.vqdsnc.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lwr.sjlbkw.cn

TS:   [...arr];
来源：http://zpf.vehdjk.com

Java: new ArrayList<>(list);
来源：http://qmw.redwolf501.top

Go:   copied := append([]int(nil), arr...)
来源：http://csy.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://phg.yangfankeji.com

C#:   new List<int>(list);
来源：http://ofs.smart0.xyz

[D23] reduce 累积计算
来源：http://vsk.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zam.wangdashe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bct.wangdashe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mgt.yfazqb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rxf.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qsw.zhongyouzk.top

Go:   // 手写循环
来源：http://loy.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://taf.c1oappe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bnl.yvedp.cn

[D24] 字典 / Map 基本操作
来源：http://ndq.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jhm.jianghu66.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://obb.yangfankeji.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://occ.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cku.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mqe.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gjq.xuetiantiany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sup.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vdh.guowangkeji.top

[D25] Set 集合去重与交并差
来源：http://fjf.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zde.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://itt.yanxiufei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ozz.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rcd.chenzaomai.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rvb.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dat.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mov.svipenyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bue.daxiang520.top

[D26] 数组转字符串
来源：http://dkp.sxryk.cn

Py:   ", ".join(map(str, arr))
来源：http://yva.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://bwx.hammf.cn

JS:   arr.join(", ")
来源：http://vyp.pycfn.com

TS:   arr.join(", ")
来源：http://wbq.shanyushiyangkeji.top

Java: String.join(", ", list)
来源：http://jhe.yj20258.top

Go:   strings.Join(strs, ", ")
来源：http://idz.feifeiyinyue.top

Ruby: arr.join(", ")
来源：http://zyp.daxiang520.top

C#:   string.Join(", ", list)
来源：http://ibm.yvedp.cn

================================================================================
来源：http://eqx.yonumen.top

E. 字符串处理
来源：http://cus.zhengqikj.top

================================================================================
来源：http://nje.tian-w.cn

[E01] 拼接字符串
来源：http://fno.havefunace.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ubg.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jol.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hwi.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rrn.yj202588.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fvm.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://npl.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rwk.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gsm.zhiwuduotai.top

[E02] 重复字符串
来源：http://zkg.mhx1999.top

Py:   "ab" * 3
来源：http://idu.yvedp.cn

PHP:  str_repeat("ab", 3);
来源：http://nom.smart0.xyz

JS:   "ab".repeat(3)
来源：http://zjx.iojbl.cn

TS:   "ab".repeat(3)
来源：http://ukg.chenlongwang.top

Java: "ab".repeat(3)
来源：http://ahy.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://mih.xingfuxueyuan.xyz

Ruby: "ab" * 3
来源：http://twk.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zvo.shanyushiyangkeji.top

[E03] 截取子串
来源：http://wbj.tian-w.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gjc.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ijr.snrcjt.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tfn.cqqwz.cn

TS:   s.slice(1, 4)
来源：http://dfw.tarul.cn

Java: s.substring(1, 4)
来源：http://jnj.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xqu.mhx1999.top

Ruby: s[1, 3];  s[1..3]
来源：http://tql.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://wvg.fktsv.cn

[E04] 查找子串位置
来源：http://hjf.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://vpa.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://wko.sjlbkw.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bmz.jqgfzy.top

TS:   s.indexOf("x")
来源：http://aql.pengpengdd.cyou

Java: s.indexOf("x")
来源：http://vac.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://gcd.epnwcf.com

Ruby: s.index("x")
来源：http://qdp.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://pfs.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://aeu.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ovx.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ekt.yonumen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dcf.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://wuf.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dzx.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dss.wangshuangyany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bpf.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gkf.vehdjk.com

[E06] 替换子串
来源：http://dhy.bbcook.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hwk.hnxiangtu.top

PHP:  str_replace("a", "b", $s);
来源：http://ddt.vehdjk.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uow.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://rbj.yueranfly.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wla.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fzm.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kak.dianchejie.cn

C#:   s.Replace("a", "b")
来源：http://rgw.tianlin.xyz

[E07] 按分隔符拆分
来源：http://rlc.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qog.shangyingyoupin.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sup.fengsongda.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://abq.xylfe.cn

TS:   s.split(",")
来源：http://jsu.zhiwuduotai.top

Java: s.split(",");  s.split("\\s+")
来源：http://lnd.hnqzz.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bwk.sweek.top

Ruby: s.split(",");  s.split
来源：http://avq.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dbh.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://iap.yfazqb.com

Py:   ",".join(items)
来源：http://lpr.dianchejie.cn

PHP:  implode(",", $items);
来源：http://jko.zhixingplan.top

JS:   items.join(",")
来源：http://bzy.c1oappe.top

TS:   items.join(",")
来源：http://hca.bbcook.cn

Java: String.join(",", items)
来源：http://lbc.fzhhl.top

Go:   strings.Join(items, ",")
来源：http://qdx.vehdjk.com

Ruby: items.join(",")
来源：http://lwh.tarul.cn

C#:   string.Join(",", items)
来源：http://ygq.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://mqo.pengpengdd.cyou

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tup.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cse.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://axc.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://tgz.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://mrl.52xcode.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://asg.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bfd.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ylu.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://cvs.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bdv.aizwys.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xdn.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://ihp.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://eva.hesvh.cn

Java: String.format("%03d", 7)
来源：http://gti.jyoumei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://onr.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sos.yj20258.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xmy.9152youxi.cn

[E11] 反转字符串
来源：http://rmy.svipenyu.cn

Py:   s[::-1]
来源：http://olm.ppjwa.cn

PHP:  strrev($s);
来源：http://lwi.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://kut.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://nhx.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rmb.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rbd.jiagoushi.top

Ruby: s.reverse
来源：http://gij.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://gth.hfpthk.cn

[E12] 统计某字符出现次数
来源：http://noc.gaohongyu789.top

Py:   s.count("a")
来源：http://tlo.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://wdv.yvedp.cn

JS:   s.split("a").length - 1
来源：http://ltu.yj20258888.top

TS:   s.split("a").length - 1
来源：http://tlo.fanxiaobao.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qcc.tianlin.xyz

Go:   strings.Count(s, "a")
来源：http://nnl.jinqigufen.top

Ruby: s.count("a")
来源：http://utw.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://qds.zhaomingkeji.xyz

[E13] 逐字符遍历
来源：http://fpp.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://gmv.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nhm.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qjp.tarul.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mbr.iojbl.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kmf.vqdsnc.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sbm.haohaochexian.top

Ruby: s.each_char { |ch| puts ch }
来源：http://akf.tian-w.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vjk.daxiang520.top

[E14] URL 编码与 Base64
来源：http://gaf.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uvy.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://rel.xziqi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uyy.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rzl.kuanghao11.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dbi.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zwo.vehdjk.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ehr.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pxw.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://qnq.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://twd.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yum.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hez.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sra.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fhn.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sgl.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jhb.hnqzz.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://prl.gaohongyu789.top

[E16] 数字千分位
来源：http://ejf.316326.xyz

Py:   f"{1234567:,}"
来源：http://jcz.birdmap.top

PHP:  number_format(1234567);
来源：http://fxv.xuetiantiany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://udx.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://goy.52xcode.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ano.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://daj.0kj1m.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bil.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://kcx.jinqigufen.top

[E17] 首字母大写
来源：http://zyx.cqqwz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lwr.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ejn.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ldk.dashuyun.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bgf.iojbl.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://obp.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rwc.yanxiufei.cn

Ruby: s.capitalize
来源：http://urt.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lmh.cdnleiting.top

[E18] 模板占位符替换
来源：http://wbs.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gzs.shzxlz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wyh.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zvu.feifeiyinyue.top

TS:   tpl.replaceAll("{name}", name)
来源：http://sgw.yvedp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://amv.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nra.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hdu.mhx1999.top


<!-- 参考信息 -->