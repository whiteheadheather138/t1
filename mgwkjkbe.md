代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cfx.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gfi.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bpy.epnwcf.com

Go:   slices.Index(arr, x)
来源：http://wpl.chenjidiqi.icu

Ruby: arr.index(x)
来源：http://bby.ydzc1.top

C#:   list.IndexOf(x);
来源：http://vol.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://kwx.zdbjq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vtx.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gze.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://aed.0kj1m.cn

TS:   arr.filter(x => x > 3)
来源：http://wso.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bgd.ybcxt.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qbw.cashguo.top

Ruby: arr.select { |x| x > 3 }
来源：http://wrx.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qga.aibaodan.cn

[D14] 映射转换（每个元素变形）
来源：http://pkg.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zry.jiagoushi.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jwi.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://kma.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://utt.c1oappe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jol.zdbjq.cn

Go:   // 手写循环
来源：http://qvx.shanyushiyangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://zem.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://akq.chenlongwang.top

[D15] 去重
来源：http://qsm.ivvv.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mie.yongpay.top

PHP:  array_unique($arr);
来源：http://dcw.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://csq.sjlbkw.cn

TS:   [...new Set(arr)]
来源：http://xcp.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vwa.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yww.xingfuxueyuan.xyz

Ruby: arr.uniq
来源：http://bui.wangdashe.top

C#:   list.Distinct().ToList()
来源：http://dzx.zhiwuduotai.top

[D16] 求和与平均值
来源：http://glx.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ola.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hoi.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fug.gaohongyu789.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mdy.chenlongwang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://luj.cucudq.cn

Go:   // 手写循环累加
来源：http://rdr.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uoe.316326.xyz

C#:   list.Sum();  list.Average()
来源：http://rni.cheryme.top

[D17] 最大值与最小值
来源：http://fzt.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://eag.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://oww.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xhr.havefunace.top

TS:   Math.max(...arr);
来源：http://eit.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hrw.guowangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://exw.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://xyl.ctjpmb.com

C#:   list.Max();  list.Min()
来源：http://fxm.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://uwy.zhijiandao.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ffd.daxiang520.top

PHP:  array_merge(...$nested);
来源：http://mhq.hfpthk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wdh.yonumen.top

TS:   nested.flat();
来源：http://hmx.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rts.wangshuangyany.cn

Go:   // 手写双层循环
来源：http://phl.sjlbkw.cn

Ruby: nested.flatten
来源：http://suc.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://gmj.zhijiandao.cn

[D19] 按字段分组
来源：http://kux.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tgh.ydjk.org.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jrf.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bcf.c1oappe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://reg.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rgl.mhx1999.top

Go:   // 手写 map[string][]T
来源：http://kzt.jinghuilouyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://isz.daxiang520.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ptc.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://hvx.zdbjq.cn

Py:   Counter(arr)
来源：http://hyt.yonumen.top

PHP:  array_count_values($arr);
来源：http://zre.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lmw.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bnc.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iue.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://dzd.gotoacloud.top

Ruby: arr.tally
来源：http://mwp.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gyr.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://qmt.yonumen.top

Py:   x in arr
来源：http://lii.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://gdl.yonumen.top

JS:   arr.includes(x)
来源：http://ail.yj202588.top

TS:   arr.includes(x)
来源：http://dzs.chenlongwang.top

Java: list.contains(x)
来源：http://vmy.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://zkd.vehdjk.com

Ruby: arr.include?(x)
来源：http://khk.birdmap.top

C#:   list.Contains(x)
来源：http://wro.wangdashe.top

[D22] 复制数组（避免共享引用）
来源：http://vwm.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://egn.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hongshengwenyu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lfu.hfpthk.cn

TS:   [...arr];
来源：http://dar.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://ksc.jqgufenzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://gnh.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://cei.sxryk.cn

C#:   new List<int>(list);
来源：http://dfx.bjfxy.top

[D23] reduce 累积计算
来源：http://ytw.ybcxt.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fny.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uyk.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nlx.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://saq.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wab.nanxuanxn.top

Go:   // 手写循环
来源：http://zzm.fengsongda.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ilf.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ugc.daria6918.cn

[D24] 字典 / Map 基本操作
来源：http://pax.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rlx.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gti.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vxv.sxryk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yhg.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://opq.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ltl.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fwn.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xme.zhaomingkeji.xyz

[D25] Set 集合去重与交并差
来源：http://tuz.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rij.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gsg.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bpm.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cui.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rcw.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gwk.jinghuilouyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://odt.guannengcc.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nrk.yuanzhike.top

[D26] 数组转字符串
来源：http://wuc.aizwys.cn

Py:   ", ".join(map(str, arr))
来源：http://mkm.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://pwf.hnxiangtu.top

JS:   arr.join(", ")
来源：http://cwq.hywenlv.cn

TS:   arr.join(", ")
来源：http://olc.tanke756.top

Java: String.join(", ", list)
来源：http://qss.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://fzq.cashguo.top

Ruby: arr.join(", ")
来源：http://nwz.yj202588.top

C#:   string.Join(", ", list)
来源：http://phf.jyoumei.cn

================================================================================
来源：http://gtq.nwbrower.top

E. 字符串处理
来源：http://qdr.xuetiantiany.cn

================================================================================
来源：http://uyt.ybcxt.top

[E01] 拼接字符串
来源：http://vhb.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mvm.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://opz.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xjb.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yyy.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nlv.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cju.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jzj.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tms.cashguo.top

[E02] 重复字符串
来源：http://jlt.pycfn.com

Py:   "ab" * 3
来源：http://xov.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://gxl.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://qyo.havefunace.top

TS:   "ab".repeat(3)
来源：http://kmp.chenzaomai.com

Java: "ab".repeat(3)
来源：http://swa.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://gve.tarul.cn

Ruby: "ab" * 3
来源：http://ean.yanxiufei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://khl.yvedp.cn

[E03] 截取子串
来源：http://jay.yj202588.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jxz.xuetiantiany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gsa.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sxu.yvedp.cn

TS:   s.slice(1, 4)
来源：http://puf.fktsv.cn

Java: s.substring(1, 4)
来源：http://fhg.yongpay.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://msj.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://oxm.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://gba.yonumen.top

[E04] 查找子串位置
来源：http://sas.zhiwuduotai.top

Py:   s.find("x");  s.index("x")
来源：http://yft.xziqi.cn

PHP:  strpos($s, "x");
来源：http://wvq.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bov.hfpthk.cn

TS:   s.indexOf("x")
来源：http://agi.mhx1999.top

Java: s.indexOf("x")
来源：http://gzs.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://ztk.cheryme.top

Ruby: s.index("x")
来源：http://ebj.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://zlk.yfazqb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ejz.jlsjyb.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yem.epnwcf.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rsp.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bci.yvedp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kij.yj20258888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fsm.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gjl.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oiz.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cxy.ctjpmb.com

[E06] 替换子串
来源：http://enh.c1oappe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://khv.shanyushiyangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://ngg.xingfuxueyuan.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hqq.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://tjh.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://alv.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aws.yangfankeji.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://isn.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://tuz.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://sky.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yfw.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ztm.yfazqb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://kqh.xingfuxueyuan.xyz

TS:   s.split(",")
来源：http://hdo.dianchejie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://aom.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bcd.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://rvh.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bnp.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://gse.dianchejie.cn

Py:   ",".join(items)
来源：http://ptg.smart0.xyz

PHP:  implode(",", $items);
来源：http://tuw.shuidangran.top

JS:   items.join(",")
来源：http://usr.uphjek.com

TS:   items.join(",")
来源：http://lhn.jiagoushi.top

Java: String.join(",", items)
来源：http://tkj.ivvv.top

Go:   strings.Join(items, ",")
来源：http://qem.jianghu66.top

Ruby: items.join(",")
来源：http://bzg.cdnleiting.top

C#:   string.Join(",", items)
来源：http://gdd.ybcxt.top

[E09] 去除所有空白字符
来源：http://aec.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oxz.fengsongda.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xkv.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://lkd.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://vxh.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://jwp.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hsq.cashguo.top

Ruby: s.gsub(/\s+/, "")
来源：http://rqb.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jum.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://qmn.yonumen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hyy.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lhk.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://rrh.fanxiaobao.xyz

TS:   "7".padStart(3, "0")
来源：http://pok.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://wub.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://dym.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nwx.yangfankeji.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mrx.tarul.cn

[E11] 反转字符串
来源：http://sap.haohaochexian.top

Py:   s[::-1]
来源：http://udd.havefunace.top

PHP:  strrev($s);
来源：http://vla.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://pxb.birdmap.top

TS:   [...s].reverse().join("")
来源：http://ozd.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vol.fehbvm.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://yra.gotoacloud.top

Ruby: s.reverse
来源：http://dtp.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://swo.yvedp.cn

[E12] 统计某字符出现次数
来源：http://qtx.gotoacloud.top

Py:   s.count("a")
来源：http://ala.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://alv.9152youxi.cn

JS:   s.split("a").length - 1
来源：http://tdz.epnwcf.com

TS:   s.split("a").length - 1
来源：http://qye.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bxd.xingfuxueyuan.xyz

Go:   strings.Count(s, "a")
来源：http://tam.zhongyouzk.top

Ruby: s.count("a")
来源：http://xmw.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://ylt.fehbvm.com

[E13] 逐字符遍历
来源：http://fak.epnwcf.com

Py:   for ch in s: print(ch)
来源：http://hmn.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gvz.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vnk.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ixo.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jpp.dianchejie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yml.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://egt.jqgfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uhr.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://qdi.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kwp.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hro.zdbjq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://upa.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://amv.zhixingplan.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fgx.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wjl.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://chd.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wnb.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://eir.zhoulong.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://txe.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kbw.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xxr.zhiwuduotai.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kss.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fjd.zdbjq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://egp.gogol.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://apr.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fhd.hfpthk.cn

[E16] 数字千分位
来源：http://fpc.yfazqb.com

Py:   f"{1234567:,}"
来源：http://ahs.yj20258.top

PHP:  number_format(1234567);
来源：http://bgg.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hgo.jinyuanbaomall.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cte.guowangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://log.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://chz.jiagoushi.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ksf.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://qum.yj20258888.top

[E17] 首字母大写
来源：http://wwr.cdnleiting.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zkr.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://tou.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://utt.wangshuangyany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ajn.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gda.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uby.yongpay.top

Ruby: s.capitalize
来源：http://hnd.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jqb.yj202588.top

[E18] 模板占位符替换
来源：http://bvd.fktsv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rol.xziqi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oce.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lyg.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://mjj.xuetiantiany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fni.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nbf.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://txp.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hah.quarkkingdee.top

[E19] 多行文本按行拆分
来源：http://fhl.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://ixg.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ebx.yuxming.cn


<!-- 参考信息 -->