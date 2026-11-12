代发 wailian999

TS:   [...arr].reverse();
来源：http://bfw.fktsv.cn

Java: Collections.reverse(list);
来源：http://azw.hammf.cn

Go:   slices.Reverse(arr)
来源：http://tpj.cheryme.top

Ruby: arr.reverse
来源：http://eev.haohaochexian.top

C#:   list.Reverse();
来源：http://qwr.hysaishi.cn

[D12] 查找元素下标
来源：http://aib.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://mrv.sufxvd.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bgd.hongshengwenyu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://igh.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wbv.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pmm.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://jtg.vehdjk.com

Ruby: arr.index(x)
来源：http://rqh.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://kxr.hfpthk.cn

[D13] 过滤（保留满足条件的）
来源：http://gtr.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iwf.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zbl.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://ugl.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://cyl.wangshuangyany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ulk.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gol.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://gkg.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tcx.fanxiaobao.xyz

[D14] 映射转换（每个元素变形）
来源：http://kpj.aibaodan.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lrd.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dyh.xuanzx.com

JS:   arr.map(x => x * 2)
来源：http://oku.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://gxm.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jju.andypj.xyz

Go:   // 手写循环
来源：http://ysq.dashuyun.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aks.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://exn.zycfv.cn

[D15] 去重
来源：http://mya.guowangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://krm.dashuyun.cn

PHP:  array_unique($arr);
来源：http://lsd.shuidangran.top

JS:   [...new Set(arr)]
来源：http://aiq.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://uob.xylfe.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ctb.jinqigfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://hhd.yj20258.top

Ruby: arr.uniq
来源：http://wid.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://iiw.316326.xyz

[D16] 求和与平均值
来源：http://hjp.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zqs.jyoumei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xtd.hesvh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mvt.zhijiandao.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vox.epnwcf.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zxw.shanyushiyangkeji.top

Go:   // 手写循环累加
来源：http://kbj.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qlt.zhijiandao.cn

C#:   list.Sum();  list.Average()
来源：http://ygx.yanxiufei.cn

[D17] 最大值与最小值
来源：http://cuc.tarul.cn

Py:   max(arr);  min(arr)
来源：http://uba.svipenyu.cn

PHP:  max($arr);  min($arr);
来源：http://asi.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iof.chenlongwang.top

TS:   Math.max(...arr);
来源：http://zmu.meibo888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://huk.pengpengdd.cyou

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yhg.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://trn.shanyushiyangtech.top

C#:   list.Max();  list.Min()
来源：http://mqz.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://ijg.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://brc.jinqigfzy.top

PHP:  array_merge(...$nested);
来源：http://ary.fengsongda.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fqy.meibo888.top

TS:   nested.flat();
来源：http://evz.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mny.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://lme.nwbrower.top

Ruby: nested.flatten
来源：http://ikj.shanyushiyangtech.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://soh.zdqjudy.top

[D19] 按字段分组
来源：http://hmh.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eun.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qwk.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uol.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zpb.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nvp.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://iwm.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://unn.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qhg.zhaomingkeji.xyz

[D20] 统计每个元素出现次数
来源：http://jfn.yj20258.top

Py:   Counter(arr)
来源：http://wgs.kuanghao11.cn

PHP:  array_count_values($arr);
来源：http://bbg.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://flw.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ncq.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://opw.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://wyh.hongshengwenyu.top

Ruby: arr.tally
来源：http://cop.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zkt.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://yvl.fehbvm.com

Py:   x in arr
来源：http://fyz.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://ydc.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://udf.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://iby.nanxinkj.top

Java: list.contains(x)
来源：http://oav.dashuyun.cn

Go:   slices.Contains(arr, x)
来源：http://lvh.ydzc1.top

Ruby: arr.include?(x)
来源：http://lss.sysykeji.top

C#:   list.Contains(x)
来源：http://iey.zhaomingkeji.xyz

[D22] 复制数组（避免共享引用）
来源：http://lph.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uau.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pen.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://deu.redwolf501.top

TS:   [...arr];
来源：http://hct.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://vsn.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://nbm.shanyushiyangtech.top

Ruby: arr.dup;  arr.clone
来源：http://hox.316326.xyz

C#:   new List<int>(list);
来源：http://fci.mhx1999.top

[D23] reduce 累积计算
来源：http://ymm.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xaa.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qih.cheryme.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gap.jqgufenzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oqg.ehwqpu.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://kha.wangshuangyany.cn

Go:   // 手写循环
来源：http://hma.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oyt.hesvh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rmq.hongshengwenyu.top

[D24] 字典 / Map 基本操作
来源：http://alo.tanke756.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yih.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bum.smart0.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mrq.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uty.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hmx.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ddh.jinqigfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://evl.chenjidiqi.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jyr.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://lpg.sufxvd.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ibx.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pfm.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hkh.jiagoushi.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wll.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tdg.chenjidiqi.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://knk.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lsw.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fnq.hongshengwenyu.top

[D26] 数组转字符串
来源：http://cdo.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://gma.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://kxp.tianlin.xyz

JS:   arr.join(", ")
来源：http://fow.dashuyun.cn

TS:   arr.join(", ")
来源：http://jtu.ivvv.top

Java: String.join(", ", list)
来源：http://ipj.bjfxy.top

Go:   strings.Join(strs, ", ")
来源：http://vxm.vehdjk.com

Ruby: arr.join(", ")
来源：http://bso.hesvh.cn

C#:   string.Join(", ", list)
来源：http://xbr.zhoulong.xyz

================================================================================
来源：http://tzt.cdnleiting.top

E. 字符串处理
来源：http://jmu.hammf.cn

================================================================================
来源：http://upz.xziqi.cn

[E01] 拼接字符串
来源：http://poq.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bgu.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qpa.cdnleiting.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fns.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://azq.aibaodan.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bcn.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zue.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://atg.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lrz.svipenyu.cn

[E02] 重复字符串
来源：http://ike.zhoulong.xyz

Py:   "ab" * 3
来源：http://dps.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://deq.tarul.cn

JS:   "ab".repeat(3)
来源：http://vfm.fengsongda.top

TS:   "ab".repeat(3)
来源：http://rtb.jianghu66.top

Java: "ab".repeat(3)
来源：http://cua.hysaishi.cn

Go:   strings.Repeat("ab", 3)
来源：http://pyw.fengsongda.top

Ruby: "ab" * 3
来源：http://cke.sjlbkw.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rpm.hammf.cn

[E03] 截取子串
来源：http://bgb.cashguo.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tqq.yuxming.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://idz.tanke756.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xmw.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://nkr.havefunace.top

Java: s.substring(1, 4)
来源：http://ujk.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ups.zdbjq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bxu.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://sew.shangyingyoupin.top

[E04] 查找子串位置
来源：http://xtc.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://xvk.jinqigfzy.top

PHP:  strpos($s, "x");
来源：http://ate.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vqc.zdbjq.cn

TS:   s.indexOf("x")
来源：http://tpz.52xcode.cn

Java: s.indexOf("x")
来源：http://gng.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://wzw.xinyue.icu

Ruby: s.index("x")
来源：http://tnq.vehdjk.com

C#:   s.IndexOf("x")
来源：http://hfe.cucudq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bim.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fgd.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://knq.xuanzx.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://apy.gotoacloud.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qbh.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pqa.aizwys.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cup.fzhhl.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nyt.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xve.gotoacloud.top

[E06] 替换子串
来源：http://lqe.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lje.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://esx.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mee.zhiwuduotai.top

TS:   s.replaceAll("a", "b")
来源：http://lxs.jyoumei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://clh.cucudq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://enj.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vtm.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://ayj.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://oiu.yanxiufei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sjs.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lvs.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://fyq.shanyushiyangtech.top

TS:   s.split(",")
来源：http://ybg.ivvv.top

Java: s.split(",");  s.split("\\s+")
来源：http://lql.zdbjq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://txv.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://xvn.guowangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qgn.fanxiaobao.xyz

[E08] 数组按分隔符合并
来源：http://tbl.snrcjt.cn

Py:   ",".join(items)
来源：http://hxt.zdqjudy.top

PHP:  implode(",", $items);
来源：http://gmq.feifeiyinyue.top

JS:   items.join(",")
来源：http://ped.pycfn.com

TS:   items.join(",")
来源：http://xiw.quarkkingdee.top

Java: String.join(",", items)
来源：http://yww.jiagoushi.top

Go:   strings.Join(items, ",")
来源：http://ekx.tian-w.cn

Ruby: items.join(",")
来源：http://uuy.ybcxt.top

C#:   string.Join(",", items)
来源：http://ipd.fengsongda.top

[E09] 去除所有空白字符
来源：http://zyz.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ffb.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wrv.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://dvm.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://hln.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://xbo.daria6918.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qor.xuetiantiany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gbc.jqgufenzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uuj.ctjpmb.com

[E10] 左侧补零 / 定长填充
来源：http://udw.shanyushiyangtech.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nrn.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yof.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://bla.ydzc1.top

TS:   "7".padStart(3, "0")
来源：http://ntj.nanxinkj.top

Java: String.format("%03d", 7)
来源：http://zug.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://byi.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yqs.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://spm.yonumen.top

[E11] 反转字符串
来源：http://lso.chenzaomai.com

Py:   s[::-1]
来源：http://sul.hongshengwenyu.top

PHP:  strrev($s);
来源：http://cpr.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://qbf.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://yde.dashuyun.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ukx.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://uit.ctjpmb.com

Ruby: s.reverse
来源：http://oxy.hnqzz.top

C#:   new string(s.Reverse().ToArray())
来源：http://euy.jiagoushi.top

[E12] 统计某字符出现次数
来源：http://omo.shzxlz.cn

Py:   s.count("a")
来源：http://yqp.dashuyun.cn

PHP:  substr_count($s, "a");
来源：http://mti.xinyue.icu

JS:   s.split("a").length - 1
来源：http://ipq.zycfv.cn

TS:   s.split("a").length - 1
来源：http://vkw.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://elv.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://rgg.jinqigufen.top

Ruby: s.count("a")
来源：http://qrm.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://ugj.gogol.net.cn

[E13] 逐字符遍历
来源：http://ctt.epnwcf.com

Py:   for ch in s: print(ch)
来源：http://kph.dianchejie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ngy.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dfq.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wti.mhx1999.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ehd.vehdjk.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ait.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://qow.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mxm.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://amr.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bnq.tian-w.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jrg.ywan-chungtsiang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://alq.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dcj.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://egq.zycfv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hsg.zhengqikj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fzb.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://czq.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://opv.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://url.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ggi.uphjek.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kwa.cheryme.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uuv.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hyr.shanyushiyangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vsw.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iqi.shanyushiyangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wor.meibo888.top

[E16] 数字千分位
来源：http://ltk.ivvv.top

Py:   f"{1234567:,}"
来源：http://cig.jianghu66.top

PHP:  number_format(1234567);
来源：http://cdj.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://uvj.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gkl.cucudq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://umr.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lis.fzhhl.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bml.uphjek.com

C#:   1234567.ToString("N0")
来源：http://cef.xinyue.icu

[E17] 首字母大写
来源：http://fbx.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wys.tianlin.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://xwt.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cpq.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cui.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qei.yj202588.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gvu.dianchejie.cn

Ruby: s.capitalize
来源：http://fdf.cheryme.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://huf.9152youxi.cn

[E18] 模板占位符替换
来源：http://zyi.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jot.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://esl.snrcjt.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nlu.uphjek.com


<!-- 参考信息 -->