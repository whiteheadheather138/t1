代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mfd.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jcn.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hrv.52xcode.cn

Go:   slices.Index(arr, x)
来源：http://cja.xylfe.cn

Ruby: arr.index(x)
来源：http://ooc.yueranfly.top

C#:   list.IndexOf(x);
来源：http://kyv.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://gjg.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pxo.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ypp.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://jjz.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://fur.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zjw.uphjek.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kga.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wrb.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://usv.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://vox.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qde.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://edq.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://mfv.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://ikm.sufxvd.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xoy.chenjidiqi.icu

Go:   // 手写循环
来源：http://adk.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://hmq.gaohongyu789.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lvf.chenlongwang.top

[D15] 去重
来源：http://dal.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fuc.uphjek.com

PHP:  array_unique($arr);
来源：http://ycj.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://onq.aizwys.cn

TS:   [...new Set(arr)]
来源：http://vcg.xuanzx.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bzb.fengsongda.top

Go:   // 用 map[T]struct{} 手写
来源：http://mmr.shzxlz.cn

Ruby: arr.uniq
来源：http://ybc.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://sng.gotoacloud.top

[D16] 求和与平均值
来源：http://gta.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dkx.yvedp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ick.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qkh.jinghuilouyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ibf.svipenyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yiy.jqgufenzy.top

Go:   // 手写循环累加
来源：http://fbo.tanke756.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oms.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://gdj.yangfankeji.com

[D17] 最大值与最小值
来源：http://sex.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://dif.cashguo.top

PHP:  max($arr);  min($arr);
来源：http://gwu.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mtd.tarul.cn

TS:   Math.max(...arr);
来源：http://nwe.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ysq.sysykeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gql.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://nxi.shuidangran.top

C#:   list.Max();  list.Min()
来源：http://lfu.fanxiaobao.xyz

[D18] 扁平化嵌套数组
来源：http://axj.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ths.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://iiw.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://grz.iojbl.cn

TS:   nested.flat();
来源：http://cyf.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dwc.52xcode.cn

Go:   // 手写双层循环
来源：http://xuq.sufxvd.cn

Ruby: nested.flatten
来源：http://btu.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bky.svipenyu.cn

[D19] 按字段分组
来源：http://wvh.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wah.tarul.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oje.aibaodan.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rpi.kuanghao11.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://igr.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jta.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://oyk.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://txq.jinghuilouyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hwh.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://bkm.jlsjyb.cn

Py:   Counter(arr)
来源：http://bjm.zhaomingkeji.xyz

PHP:  array_count_values($arr);
来源：http://qmp.0kj1m.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://udk.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ywk.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hhq.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://ppp.pengpengdd.cyou

Ruby: arr.tally
来源：http://dbj.yj20258.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qzu.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://llu.jinqigfzy.top

Py:   x in arr
来源：http://xib.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://wus.daria6918.cn

JS:   arr.includes(x)
来源：http://uyd.sysykeji.top

TS:   arr.includes(x)
来源：http://otz.vqdsnc.cn

Java: list.contains(x)
来源：http://lvu.jinyuanbaomall.cn

Go:   slices.Contains(arr, x)
来源：http://bfn.shzxlz.cn

Ruby: arr.include?(x)
来源：http://ciz.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://tcx.zhoulong.xyz

[D22] 复制数组（避免共享引用）
来源：http://pfb.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ymj.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ihc.nwbrower.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jvk.jinqigfzy.top

TS:   [...arr];
来源：http://yvl.andypj.xyz

Java: new ArrayList<>(list);
来源：http://tyr.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kny.xinyue.icu

Ruby: arr.dup;  arr.clone
来源：http://hgw.chenzaomai.com

C#:   new List<int>(list);
来源：http://btl.zhongyouzk.top

[D23] reduce 累积计算
来源：http://msg.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pnj.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://byv.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gzx.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://caw.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://far.vqdsnc.cn

Go:   // 手写循环
来源：http://vcx.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gmi.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ncp.quarkkingdee.top

[D24] 字典 / Map 基本操作
来源：http://zor.pycfn.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sjn.chenzaomai.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mzv.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://usi.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kiq.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ppf.chenjidiqi.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rix.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qor.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ssp.bbcook.cn

[D25] Set 集合去重与交并差
来源：http://zfx.nanxinkj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qaf.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bvl.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kiu.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tge.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xzw.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qnv.shzxlz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nhv.ctjpmb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tcr.gogol.net.cn

[D26] 数组转字符串
来源：http://fic.zdqjudy.top

Py:   ", ".join(map(str, arr))
来源：http://jay.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://jhc.smart0.xyz

JS:   arr.join(", ")
来源：http://ggm.tanke756.top

TS:   arr.join(", ")
来源：http://hxi.zhongyouzk.top

Java: String.join(", ", list)
来源：http://kns.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://oct.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://tuz.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://mgp.chenjidiqi.icu

================================================================================
来源：http://yti.nanxuanxn.top

E. 字符串处理
来源：http://ubh.chenlongwang.top

================================================================================
来源：http://ngz.nanxuanxn.top

[E01] 拼接字符串
来源：http://rop.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://thj.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cys.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kol.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vkf.cqqwz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jsh.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nvy.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ekk.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fac.xingfuxueyuan.xyz

[E02] 重复字符串
来源：http://pdc.wangshuangyany.cn

Py:   "ab" * 3
来源：http://mzj.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://qip.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://zoz.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://qge.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://woa.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://lng.zhengqikj.top

Ruby: "ab" * 3
来源：http://kpv.cdnleiting.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sdi.sysykeji.top

[E03] 截取子串
来源：http://hxh.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aqb.feifeiyinyue.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://biy.zhijiandao.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://odw.jqgufenzy.top

TS:   s.slice(1, 4)
来源：http://yca.shanyushiyangkeji.top

Java: s.substring(1, 4)
来源：http://ebk.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://opb.jqgfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://zux.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://hpz.gzhubu.top

[E04] 查找子串位置
来源：http://crz.hcnkem.com

Py:   s.find("x");  s.index("x")
来源：http://hpz.xuanzx.com

PHP:  strpos($s, "x");
来源：http://ryc.yongpay.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uhe.dashuyun.cn

TS:   s.indexOf("x")
来源：http://spv.zdqjudy.top

Java: s.indexOf("x")
来源：http://tfc.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://pld.snrcjt.cn

Ruby: s.index("x")
来源：http://cok.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://tyt.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jqc.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pod.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://igg.zhongyouzk.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mao.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://gyh.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://prp.hongshengwenyu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://are.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cwb.wangdashe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sop.xuanzx.com

[E06] 替换子串
来源：http://twx.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nlh.yangfankeji.com

PHP:  str_replace("a", "b", $s);
来源：http://bkp.ydjk.org.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xqo.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://thd.hammf.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://duz.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sbq.havefunace.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rbl.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://rwb.jinqigufen.top

[E07] 按分隔符拆分
来源：http://svc.sjlbkw.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ymy.meibo888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cqn.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://rsr.nanxuanxn.top

TS:   s.split(",")
来源：http://hfx.tarul.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sqn.ywan-chungtsiang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ifr.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://zcr.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qxe.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://rly.smart0.xyz

Py:   ",".join(items)
来源：http://dde.hnqzz.top

PHP:  implode(",", $items);
来源：http://foe.zhijiandao.cn

JS:   items.join(",")
来源：http://pug.dashuyun.cn

TS:   items.join(",")
来源：http://rvw.gaohongyu789.top

Java: String.join(",", items)
来源：http://gew.feifeiyinyue.top

Go:   strings.Join(items, ",")
来源：http://wjz.ydjk.org.cn

Ruby: items.join(",")
来源：http://nnq.yj202588.top

C#:   string.Join(",", items)
来源：http://ptv.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://zdl.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pjs.hnqzz.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nyt.feifeiyinyue.top

JS:   s.replace(/\s+/g, "")
来源：http://ozv.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://kqq.andypj.xyz

Java: s.replaceAll("\\s+", "")
来源：http://hfb.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://usn.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://svk.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vsw.sysykeji.top

[E10] 左侧补零 / 定长填充
来源：http://omh.ehwqpu.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tay.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dvh.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://wdq.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://ijh.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://obw.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wuy.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rxk.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://elh.hysaishi.cn

[E11] 反转字符串
来源：http://txc.52xcode.cn

Py:   s[::-1]
来源：http://lal.aizwys.cn

PHP:  strrev($s);
来源：http://pul.tarul.cn

JS:   [...s].reverse().join("")
来源：http://efn.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://evf.quarkkingdee.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ynk.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fgh.xuanzx.com

Ruby: s.reverse
来源：http://rbp.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://ztw.ywan-chungtsiang.top

[E12] 统计某字符出现次数
来源：http://ngz.pengpengdd.cyou

Py:   s.count("a")
来源：http://vtb.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://oez.yueranfly.top

JS:   s.split("a").length - 1
来源：http://jvh.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://ebb.zhengqikj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qfn.sxryk.cn

Go:   strings.Count(s, "a")
来源：http://nzb.nwbrower.top

Ruby: s.count("a")
来源：http://vup.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://chy.yonumen.top

[E13] 逐字符遍历
来源：http://xxn.havefunace.top

Py:   for ch in s: print(ch)
来源：http://ukw.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ble.gogol.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ewr.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yfy.chenjidiqi.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iwj.hesvh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jxw.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cuh.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ycj.yonumen.top

[E14] URL 编码与 Base64
来源：http://atx.guannengcc.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rgy.shuidangran.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gko.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nti.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iqc.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://trb.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mzt.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qnr.52xcode.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xdr.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://oca.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gjl.wangdashe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qhs.sweek.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://npu.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xmb.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dof.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://quw.jqgufenzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uph.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dbd.hnxiangtu.top

[E16] 数字千分位
来源：http://cds.guannengcc.top

Py:   f"{1234567:,}"
来源：http://acs.hnqzz.top

PHP:  number_format(1234567);
来源：http://lld.yanxiufei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vws.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nnz.fehbvm.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eny.epnwcf.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yiu.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xun.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://zxx.jqgufenzy.top

[E17] 首字母大写
来源：http://bcs.chenzaomai.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kdk.hongshengwenyu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://aew.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://csh.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blh.xylfe.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zri.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ysk.shzxlz.cn

Ruby: s.capitalize
来源：http://jfj.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zwz.sxryk.cn

[E18] 模板占位符替换
来源：http://spb.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jnp.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ael.dianchejie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rkq.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jri.c1oappe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jac.hesvh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://thz.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ihs.hongshengwenyu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pyg.aibaodan.cn

[E19] 多行文本按行拆分
来源：http://vxf.xinyue.icu

Py:   s.splitlines()
来源：http://iky.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dtk.yongpay.top


<!-- 参考信息 -->