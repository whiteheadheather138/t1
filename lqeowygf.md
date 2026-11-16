代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qdk.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yfm.yangfankeji.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dek.fanxiaobao.xyz

Go:   slices.Index(arr, x)
来源：http://zsd.yonumen.top

Ruby: arr.index(x)
来源：http://yao.hnqzz.top

C#:   list.IndexOf(x);
来源：http://ctk.iojbl.cn

[D13] 过滤（保留满足条件的）
来源：http://pfa.yangfankeji.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dab.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mdm.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://uns.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://tss.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jos.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zbt.hnqzz.top

Ruby: arr.select { |x| x > 3 }
来源：http://zcw.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://vqf.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://rsb.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://loz.jianghu66.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://buv.jinyuanbaomall.cn

JS:   arr.map(x => x * 2)
来源：http://ebt.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://xkb.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cjx.daria6918.cn

Go:   // 手写循环
来源：http://lyq.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://dkd.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://coe.bbcook.cn

[D15] 去重
来源：http://qgm.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://idu.shanyushiyangkeji.top

PHP:  array_unique($arr);
来源：http://cur.fengsongda.top

JS:   [...new Set(arr)]
来源：http://xcp.mhx1999.top

TS:   [...new Set(arr)]
来源：http://cvu.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fkv.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://wca.xylfe.cn

Ruby: arr.uniq
来源：http://dfi.fengsongda.top

C#:   list.Distinct().ToList()
来源：http://dva.ctjpmb.com

[D16] 求和与平均值
来源：http://wqu.feifeiyinyue.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aoy.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vnh.sjlbkw.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uyx.hnqzz.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fit.fzhhl.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lde.ydzc1.top

Go:   // 手写循环累加
来源：http://ulj.mhx1999.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cwz.9152youxi.cn

C#:   list.Sum();  list.Average()
来源：http://kpi.andypj.xyz

[D17] 最大值与最小值
来源：http://nnm.birdmap.top

Py:   max(arr);  min(arr)
来源：http://vme.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://wnp.hesvh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ycv.guowangkeji.top

TS:   Math.max(...arr);
来源：http://fyc.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pbi.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://erm.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://bab.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://yeh.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://wxs.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kyz.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://zrj.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cpx.ppjwa.cn

TS:   nested.flat();
来源：http://tji.pengpengdd.cyou

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ewg.snrcjt.cn

Go:   // 手写双层循环
来源：http://xcu.sxryk.cn

Ruby: nested.flatten
来源：http://hjz.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ozx.bjfxy.top

[D19] 按字段分组
来源：http://xeo.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://psd.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://piz.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qia.jinqigfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://whp.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wmh.snrcjt.cn

Go:   // 手写 map[string][]T
来源：http://rjg.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vzd.dianchejie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qpf.gogol.net.cn

[D20] 统计每个元素出现次数
来源：http://aau.sufxvd.cn

Py:   Counter(arr)
来源：http://deg.yuxming.cn

PHP:  array_count_values($arr);
来源：http://mih.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qrm.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jej.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jyo.jianghu66.top

Go:   // 手写 map[T]int
来源：http://upz.xuanzx.com

Ruby: arr.tally
来源：http://vzl.daria6918.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yeo.fktsv.cn

[D21] 判断是否包含某元素
来源：http://sie.tanke756.top

Py:   x in arr
来源：http://mqz.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://pto.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://fww.tian-w.cn

TS:   arr.includes(x)
来源：http://hil.52xcode.cn

Java: list.contains(x)
来源：http://kmc.daria6918.cn

Go:   slices.Contains(arr, x)
来源：http://flq.fengsongda.top

Ruby: arr.include?(x)
来源：http://wgt.iojbl.cn

C#:   list.Contains(x)
来源：http://hgm.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://lut.nwbrower.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qnn.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://odo.daxiang520.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bkn.epnwcf.com

TS:   [...arr];
来源：http://ekg.jinqigfzy.top

Java: new ArrayList<>(list);
来源：http://lep.yj202588.top

Go:   copied := append([]int(nil), arr...)
来源：http://nwt.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://rbr.ivvv.top

C#:   new List<int>(list);
来源：http://akb.sxryk.cn

[D23] reduce 累积计算
来源：http://lry.guannengcc.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vzp.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pvs.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ire.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uus.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xdq.sysykeji.top

Go:   // 手写循环
来源：http://exi.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hbp.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lkk.shuidangran.top

[D24] 字典 / Map 基本操作
来源：http://wjw.ppjwa.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xcw.hnxiangtu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rri.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jgz.zhengqikj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uzr.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ibq.tanke756.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zco.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rmo.jinqigufen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gyz.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://eyv.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kgz.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pvk.snrcjt.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yib.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://arh.yj20258888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jfq.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bet.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kze.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bnr.birdmap.top

[D26] 数组转字符串
来源：http://ehc.sjlbkw.cn

Py:   ", ".join(map(str, arr))
来源：http://eya.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://nlz.0kj1m.cn

JS:   arr.join(", ")
来源：http://rlb.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://vst.wangdashe.top

Java: String.join(", ", list)
来源：http://nff.tianlin.xyz

Go:   strings.Join(strs, ", ")
来源：http://mas.hfpthk.cn

Ruby: arr.join(", ")
来源：http://anu.hammf.cn

C#:   string.Join(", ", list)
来源：http://vei.zhengqikj.top

================================================================================
来源：http://agh.c1oappe.top

E. 字符串处理
来源：http://bju.hysaishi.cn

================================================================================
来源：http://cyr.sjlbkw.cn

[E01] 拼接字符串
来源：http://jra.yj202588.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jrs.pycfn.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tot.fengsongda.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zov.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wwf.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cue.zycfv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fea.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ndm.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://euc.zhongyouzk.top

[E02] 重复字符串
来源：http://plz.52xcode.cn

Py:   "ab" * 3
来源：http://qpc.cheryme.top

PHP:  str_repeat("ab", 3);
来源：http://hcp.uphjek.com

JS:   "ab".repeat(3)
来源：http://lqn.9152youxi.cn

TS:   "ab".repeat(3)
来源：http://fxt.jqgfzy.top

Java: "ab".repeat(3)
来源：http://uds.hywenlv.cn

Go:   strings.Repeat("ab", 3)
来源：http://hhg.yj20258.top

Ruby: "ab" * 3
来源：http://dbc.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rku.fzhhl.top

[E03] 截取子串
来源：http://kkf.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wsh.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jgb.haohaochexian.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qdi.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://rom.uphjek.com

Java: s.substring(1, 4)
来源：http://qpx.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kpj.hnxiangtu.top

Ruby: s[1, 3];  s[1..3]
来源：http://jtt.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://cje.havefunace.top

[E04] 查找子串位置
来源：http://dyo.xziqi.cn

Py:   s.find("x");  s.index("x")
来源：http://jer.daxiang520.top

PHP:  strpos($s, "x");
来源：http://whv.hysaishi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://olo.guowangkeji.top

TS:   s.indexOf("x")
来源：http://iiv.zdqjudy.top

Java: s.indexOf("x")
来源：http://qsx.hywenlv.cn

Go:   strings.Index(s, "x")
来源：http://qrn.aizwys.cn

Ruby: s.index("x")
来源：http://ste.316326.xyz

C#:   s.IndexOf("x")
来源：http://gnc.bbcook.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ybl.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xnh.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eti.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xgt.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://nof.redwolf501.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zcr.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gcx.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ebs.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gyc.cashguo.top

[E06] 替换子串
来源：http://odc.xuetiantiany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dcq.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://avs.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hsx.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://gjz.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uem.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ewy.zhengqikj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tsx.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://ayg.sjlbkw.cn

[E07] 按分隔符拆分
来源：http://nch.xuetiantiany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dvu.shanyushiyangtech.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fri.shanyushiyangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hka.jinghuilouyu.cn

TS:   s.split(",")
来源：http://ivs.zycfv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tuw.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hpv.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://qzo.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tcm.gzhubu.top

[E08] 数组按分隔符合并
来源：http://wlu.redwolf501.top

Py:   ",".join(items)
来源：http://cpv.xuanzx.com

PHP:  implode(",", $items);
来源：http://rem.zhixingplan.top

JS:   items.join(",")
来源：http://gcw.aibaodan.cn

TS:   items.join(",")
来源：http://uph.redwolf501.top

Java: String.join(",", items)
来源：http://lty.daxiang520.top

Go:   strings.Join(items, ",")
来源：http://luz.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://egk.hywenlv.cn

C#:   string.Join(",", items)
来源：http://gcf.jqgfzy.top

[E09] 去除所有空白字符
来源：http://tfw.zdbjq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://olg.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://elc.tanke756.top

JS:   s.replace(/\s+/g, "")
来源：http://riw.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://uok.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://pek.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rdo.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://lvb.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ccj.sufxvd.cn

[E10] 左侧补零 / 定长填充
来源：http://fzk.birdmap.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kpt.hywenlv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://thg.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://ohq.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://qlo.xylfe.cn

Java: String.format("%03d", 7)
来源：http://iil.yj20258.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rqi.ywan-chungtsiang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rfv.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://knu.xylfe.cn

[E11] 反转字符串
来源：http://bhn.zhiwuduotai.top

Py:   s[::-1]
来源：http://slg.hywenlv.cn

PHP:  strrev($s);
来源：http://yjm.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://hqj.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://oku.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xpx.snrcjt.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pgr.fehbvm.com

Ruby: s.reverse
来源：http://jen.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://cvc.hammf.cn

[E12] 统计某字符出现次数
来源：http://cgh.sxryk.cn

Py:   s.count("a")
来源：http://uvh.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://nyj.vehdjk.com

JS:   s.split("a").length - 1
来源：http://fuh.fzhhl.top

TS:   s.split("a").length - 1
来源：http://sxv.smart0.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://osg.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://ssa.xylfe.cn

Ruby: s.count("a")
来源：http://bcq.fengsongda.top

C#:   s.Count(c => c == 'a')
来源：http://als.ctjpmb.com

[E13] 逐字符遍历
来源：http://ecv.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://wte.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://elw.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kbx.bjfxy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lxe.dashuyun.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tpu.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xnw.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://baw.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eub.hysaishi.cn

[E14] URL 编码与 Base64
来源：http://onp.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xtc.uphjek.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://lfn.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gcx.ywan-chungtsiang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fue.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mlv.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://urn.ivvv.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ici.xylfe.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wxf.quarkkingdee.top

[E15] HTML 转义 / 反转义
来源：http://uqj.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://eym.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wvc.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uqg.ehwqpu.com

TS:   // 同上，务必做 XSS 过滤
来源：http://kve.jqgufenzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lcd.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kcr.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xjg.feifeiyinyue.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://axx.zhongyouzk.top

[E16] 数字千分位
来源：http://xto.snrcjt.cn

Py:   f"{1234567:,}"
来源：http://qoh.bjfxy.top

PHP:  number_format(1234567);
来源：http://yyj.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://whs.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ski.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lhv.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xat.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kun.sjlbkw.cn

C#:   1234567.ToString("N0")
来源：http://hya.mhx1999.top

[E17] 首字母大写
来源：http://pqa.yvedp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ilk.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bkn.gogol.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pif.hammf.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://osc.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cof.uphjek.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pth.mhx1999.top

Ruby: s.capitalize
来源：http://lzn.zhijiandao.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ofn.tanke756.top

[E18] 模板占位符替换
来源：http://kpz.nanxinkj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nll.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bfl.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hgb.gzhubu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pxf.shangyingyoupin.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nan.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nlh.sufxvd.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://txx.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://olh.sweek.top

[E19] 多行文本按行拆分
来源：http://tus.c1oappe.top

Py:   s.splitlines()
来源：http://gsj.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kpg.ppjwa.cn


<!-- 参考信息 -->