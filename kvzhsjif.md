代发 wailian999

Ruby: arr.index(x)
来源：http://tyq.shanyushiyangkeji.top

C#:   list.IndexOf(x);
来源：http://isy.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://ubr.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lmm.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rie.hywenlv.cn

JS:   arr.filter(x => x > 3)
来源：http://scy.gzhubu.top

TS:   arr.filter(x => x > 3)
来源：http://vdp.hcnkem.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ezk.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ixy.guannengcc.top

Ruby: arr.select { |x| x > 3 }
来源：http://stc.xingfuxueyuan.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://ckq.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://nww.hywenlv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zpq.yuanzhike.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lep.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://pcp.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://naw.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uqk.yuxming.cn

Go:   // 手写循环
来源：http://jfn.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://iyj.tanke756.top

C#:   list.Select(x => x * 2).ToList()
来源：http://atn.zhixingplan.top

[D15] 去重
来源：http://rfk.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pzs.mhx1999.top

PHP:  array_unique($arr);
来源：http://xko.jqgfzy.top

JS:   [...new Set(arr)]
来源：http://oan.hammf.cn

TS:   [...new Set(arr)]
来源：http://maf.aizwys.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wge.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://viv.sufxvd.cn

Ruby: arr.uniq
来源：http://syb.snrcjt.cn

C#:   list.Distinct().ToList()
来源：http://kcj.zdbjq.cn

[D16] 求和与平均值
来源：http://obr.feifeiyinyue.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://unf.kuanghao11.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nsr.xinyue.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://atn.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sbk.shuidangran.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bgh.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://tvu.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://waw.bjfxy.top

C#:   list.Sum();  list.Average()
来源：http://hui.zhongyouzk.top

[D17] 最大值与最小值
来源：http://ndq.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://gkx.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://zrm.316326.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xvk.vehdjk.com

TS:   Math.max(...arr);
来源：http://xvx.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bnl.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yae.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://ifu.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://jyd.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://ztn.zdbjq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tyd.zhongyouzk.top

PHP:  array_merge(...$nested);
来源：http://yfg.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kjd.epnwcf.com

TS:   nested.flat();
来源：http://bvv.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mka.gzhubu.top

Go:   // 手写双层循环
来源：http://ucr.pengpengdd.cyou

Ruby: nested.flatten
来源：http://lqg.yvedp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xce.jinghuilouyu.cn

[D19] 按字段分组
来源：http://fci.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ayz.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kod.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kfz.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mku.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bcv.jinqigufen.top

Go:   // 手写 map[string][]T
来源：http://wik.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://nmk.jiagoushi.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ksa.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://llw.xuanzx.com

Py:   Counter(arr)
来源：http://bkj.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://nqr.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dnm.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nac.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tkm.bbcook.cn

Go:   // 手写 map[T]int
来源：http://byb.tian-w.cn

Ruby: arr.tally
来源：http://nnx.shanyushiyangtech.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ltu.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://heo.0kj1m.cn

Py:   x in arr
来源：http://auu.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://ina.chenlongwang.top

JS:   arr.includes(x)
来源：http://djm.andypj.xyz

TS:   arr.includes(x)
来源：http://zfi.svipenyu.cn

Java: list.contains(x)
来源：http://nfe.hnqzz.top

Go:   slices.Contains(arr, x)
来源：http://fsa.wangdashe.top

Ruby: arr.include?(x)
来源：http://vqz.uphjek.com

C#:   list.Contains(x)
来源：http://bjl.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://ctj.yj20258.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dey.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hgm.ybcxt.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hxs.tianlin.xyz

TS:   [...arr];
来源：http://aqb.andypj.xyz

Java: new ArrayList<>(list);
来源：http://daq.ywan-chungtsiang.top

Go:   copied := append([]int(nil), arr...)
来源：http://eff.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://lug.52xcode.cn

C#:   new List<int>(list);
来源：http://qxl.tian-w.cn

[D23] reduce 累积计算
来源：http://tpp.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gce.hesvh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pqc.yvedp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dnc.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gza.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zof.jqgufenzy.top

Go:   // 手写循环
来源：http://ujk.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aqu.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://chx.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://hwm.zhixingplan.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xtv.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zph.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://acc.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zfc.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cde.kuanghao11.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vnr.cashguo.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bgj.cdnleiting.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vzu.tanke756.top

[D25] Set 集合去重与交并差
来源：http://xky.316326.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vod.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://one.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jeb.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pmh.zhiwuduotai.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wyt.guowangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://urh.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://apa.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dkk.yfazqb.com

[D26] 数组转字符串
来源：http://eev.zhoulong.xyz

Py:   ", ".join(map(str, arr))
来源：http://dtn.shzxlz.cn

PHP:  implode(", ", $arr);
来源：http://ofp.ydjk.org.cn

JS:   arr.join(", ")
来源：http://ijz.vqdsnc.cn

TS:   arr.join(", ")
来源：http://ezg.gotoacloud.top

Java: String.join(", ", list)
来源：http://qqp.mhx1999.top

Go:   strings.Join(strs, ", ")
来源：http://wjs.andypj.xyz

Ruby: arr.join(", ")
来源：http://zen.ehwqpu.com

C#:   string.Join(", ", list)
来源：http://ufl.fengsongda.top

================================================================================
来源：http://tyr.hfpthk.cn

E. 字符串处理
来源：http://rau.fktsv.cn

================================================================================
来源：http://qti.xuetiantiany.cn

[E01] 拼接字符串
来源：http://gbr.quarkkingdee.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rgc.nwbrower.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lpy.hywenlv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yiy.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lvj.meibo888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://enw.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ysf.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vky.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ukq.fengsongda.top

[E02] 重复字符串
来源：http://zsg.jyoumei.cn

Py:   "ab" * 3
来源：http://gkp.jinghuilouyu.cn

PHP:  str_repeat("ab", 3);
来源：http://lgc.zycfv.cn

JS:   "ab".repeat(3)
来源：http://dtc.shanyushiyangkeji.top

TS:   "ab".repeat(3)
来源：http://bxt.xylfe.cn

Java: "ab".repeat(3)
来源：http://cxu.shanyushiyangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://nbt.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://jdm.fehbvm.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lbz.epnwcf.com

[E03] 截取子串
来源：http://ymv.yongpay.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fnm.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://emv.meibo888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vqi.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://eef.tarul.cn

Java: s.substring(1, 4)
来源：http://pyu.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vjm.xziqi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hey.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://oaz.yuxming.cn

[E04] 查找子串位置
来源：http://zfj.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://izj.yongpay.top

PHP:  strpos($s, "x");
来源：http://wmc.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jfb.sysykeji.top

TS:   s.indexOf("x")
来源：http://wkv.chenlongwang.top

Java: s.indexOf("x")
来源：http://wcs.hywenlv.cn

Go:   strings.Index(s, "x")
来源：http://mgo.sweek.top

Ruby: s.index("x")
来源：http://fji.yvedp.cn

C#:   s.IndexOf("x")
来源：http://yvm.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rpf.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wpm.zhoulong.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jla.aizwys.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tbc.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://aoj.ctjpmb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kki.bjfxy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bcl.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://klv.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://prf.dianchejie.cn

[E06] 替换子串
来源：http://smj.meibo888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nti.redwolf501.top

PHP:  str_replace("a", "b", $s);
来源：http://boo.yueranfly.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jej.birdmap.top

TS:   s.replaceAll("a", "b")
来源：http://zzo.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gqp.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wtx.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://amb.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://evh.ydzc1.top

[E07] 按分隔符拆分
来源：http://tuh.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hpb.hcnkem.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://exv.jyoumei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ywd.chenlongwang.top

TS:   s.split(",")
来源：http://nsy.gzhubu.top

Java: s.split(",");  s.split("\\s+")
来源：http://fqx.c1oappe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lux.ydzc1.top

Ruby: s.split(",");  s.split
来源：http://tom.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zmr.iojbl.cn

[E08] 数组按分隔符合并
来源：http://cqa.vehdjk.com

Py:   ",".join(items)
来源：http://zzr.svipenyu.cn

PHP:  implode(",", $items);
来源：http://sjc.yuxming.cn

JS:   items.join(",")
来源：http://snn.iojbl.cn

TS:   items.join(",")
来源：http://xuv.pycfn.com

Java: String.join(",", items)
来源：http://rms.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://nht.shanyushiyangkeji.top

Ruby: items.join(",")
来源：http://fqq.0kj1m.cn

C#:   string.Join(",", items)
来源：http://yze.tianlin.xyz

[E09] 去除所有空白字符
来源：http://svw.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dmq.daxiang520.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dww.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://vfb.shanyushiyangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://jmf.sweek.top

Java: s.replaceAll("\\s+", "")
来源：http://aeu.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mtq.fengsongda.top

Ruby: s.gsub(/\s+/, "")
来源：http://bpx.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ogt.fanxiaobao.xyz

[E10] 左侧补零 / 定长填充
来源：http://cgi.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cpt.wangdashe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bxz.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://hwv.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://lcr.uphjek.com

Java: String.format("%03d", 7)
来源：http://chk.fanxiaobao.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://ycj.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vti.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://boz.kuanghao11.cn

[E11] 反转字符串
来源：http://amd.hammf.cn

Py:   s[::-1]
来源：http://ylx.ybcxt.top

PHP:  strrev($s);
来源：http://qxh.pycfn.com

JS:   [...s].reverse().join("")
来源：http://mrc.yuxming.cn

TS:   [...s].reverse().join("")
来源：http://pvb.chenzaomai.com

Java: new StringBuilder(s).reverse().toString()
来源：http://utz.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eov.hywenlv.cn

Ruby: s.reverse
来源：http://cdb.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://hqc.yuxming.cn

[E12] 统计某字符出现次数
来源：http://kpk.gzhubu.top

Py:   s.count("a")
来源：http://lhg.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://bvj.cucudq.cn

JS:   s.split("a").length - 1
来源：http://kkg.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://ldm.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nyi.hnqzz.top

Go:   strings.Count(s, "a")
来源：http://ysa.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://qmr.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://btm.jianghu66.top

[E13] 逐字符遍历
来源：http://wff.hammf.cn

Py:   for ch in s: print(ch)
来源：http://ird.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vop.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://exo.hammf.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://owu.jianghu66.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fkt.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sfh.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ack.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hxj.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://zbz.uphjek.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://erx.cucudq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oyi.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qvw.zdbjq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zyd.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lsk.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kcw.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lml.9152youxi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uvy.gogol.net.cn

[E15] HTML 转义 / 反转义
来源：http://hqw.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://sfi.hesvh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lmj.xinyue.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://man.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oat.bbcook.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://avd.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vek.jinqigufen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hgc.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cuv.bbcook.cn

[E16] 数字千分位
来源：http://omv.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://cxo.nanxinkj.top

PHP:  number_format(1234567);
来源：http://wcg.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sad.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mvw.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xcw.yj202588.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aqv.fengsongda.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oqt.hammf.cn

C#:   1234567.ToString("N0")
来源：http://exa.hcnkem.com

[E17] 首字母大写
来源：http://tnw.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://npz.tianlin.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://gnu.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jzm.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xcy.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://leo.andypj.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qgu.jianghu66.top

Ruby: s.capitalize
来源：http://unc.gotoacloud.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rpl.bjfxy.top

[E18] 模板占位符替换
来源：http://vgv.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gfl.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qfz.xingfuxueyuan.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://kpy.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://pko.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baq.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qmy.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tuk.yanxiufei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bel.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://hvf.sysykeji.top

Py:   s.splitlines()
来源：http://wzk.smart0.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jmd.andypj.xyz

JS:   s.split(/\r?\n/)
来源：http://xvl.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://ans.epnwcf.com

Java: s.lines().toList()
来源：http://xnh.wangshuangyany.cn

Go:   strings.Split(s, "\n")
来源：http://gcu.cqqwz.cn


<!-- 参考信息 -->