代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tbg.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jjw.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fkh.xinyue.icu

Go:   slices.Index(arr, x)
来源：http://ueb.daria6918.cn

Ruby: arr.index(x)
来源：http://bpx.tianlin.xyz

C#:   list.IndexOf(x);
来源：http://src.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://gld.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hwn.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xgl.yfazqb.com

JS:   arr.filter(x => x > 3)
来源：http://zab.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://tvr.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jwt.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://awj.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://llz.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fod.fzhhl.top

[D14] 映射转换（每个元素变形）
来源：http://iue.svipenyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cxf.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hkw.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://rif.hywenlv.cn

TS:   arr.map(x => x * 2)
来源：http://ijf.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gmq.wangdashe.top

Go:   // 手写循环
来源：http://gty.xingfuxueyuan.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://ghg.yvedp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jhr.cucudq.cn

[D15] 去重
来源：http://rha.gogol.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vyo.sysykeji.top

PHP:  array_unique($arr);
来源：http://hmk.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://sxq.wangdashe.top

TS:   [...new Set(arr)]
来源：http://ozy.gotoacloud.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aoy.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://ihi.jqgufenzy.top

Ruby: arr.uniq
来源：http://lhj.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://gtj.yonumen.top

[D16] 求和与平均值
来源：http://ztw.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ble.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vuk.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rrt.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mrj.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qwi.ctjpmb.com

Go:   // 手写循环累加
来源：http://nib.hywenlv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bia.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://dib.meibo888.top

[D17] 最大值与最小值
来源：http://gcr.zhoulong.xyz

Py:   max(arr);  min(arr)
来源：http://mhl.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://yyv.bjfxy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dqb.yueranfly.top

TS:   Math.max(...arr);
来源：http://ctn.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://tmr.shanyushiyangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eqt.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://pbi.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://moy.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://jpj.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kbb.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://gfr.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ktd.ppjwa.cn

TS:   nested.flat();
来源：http://lry.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yaf.jqgufenzy.top

Go:   // 手写双层循环
来源：http://ogg.hammf.cn

Ruby: nested.flatten
来源：http://wvz.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tbw.fengsongda.top

[D19] 按字段分组
来源：http://atj.sweek.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cvd.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://euw.yanxiufei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ggp.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bbe.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zad.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://dma.hysaishi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://aka.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xua.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://gle.yonumen.top

Py:   Counter(arr)
来源：http://cfw.zhiwuduotai.top

PHP:  array_count_values($arr);
来源：http://msd.fanxiaobao.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hib.zhongyouzk.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aoe.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wwd.sweek.top

Go:   // 手写 map[T]int
来源：http://tob.xylfe.cn

Ruby: arr.tally
来源：http://wyo.gogol.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tmo.smart0.xyz

[D21] 判断是否包含某元素
来源：http://cbp.guannengcc.top

Py:   x in arr
来源：http://ead.chenzaomai.com

PHP:  in_array($x, $arr, true);
来源：http://ieb.redwolf501.top

JS:   arr.includes(x)
来源：http://yxx.cheryme.top

TS:   arr.includes(x)
来源：http://lxl.tianlin.xyz

Java: list.contains(x)
来源：http://pop.zhongyouzk.top

Go:   slices.Contains(arr, x)
来源：http://mdj.havefunace.top

Ruby: arr.include?(x)
来源：http://pen.xuetiantiany.cn

C#:   list.Contains(x)
来源：http://gbs.zhoulong.xyz

[D22] 复制数组（避免共享引用）
来源：http://nxd.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nbt.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://trc.gotoacloud.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uqg.jlsjyb.cn

TS:   [...arr];
来源：http://lav.kuanghao11.cn

Java: new ArrayList<>(list);
来源：http://kss.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://bry.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://rak.guowangkeji.top

C#:   new List<int>(list);
来源：http://mrk.yanxiufei.cn

[D23] reduce 累积计算
来源：http://sfj.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bmm.zhengqikj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zvw.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ttx.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qla.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zpe.zhoulong.xyz

Go:   // 手写循环
来源：http://quj.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ddu.zhijiandao.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vpz.birdmap.top

[D24] 字典 / Map 基本操作
来源：http://xbd.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xsj.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qwq.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ysu.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sbr.feifeiyinyue.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tsp.havefunace.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ncq.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iiv.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dri.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://pjl.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cqb.sxryk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qxg.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bnq.xuetiantiany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://laj.yvedp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ufy.wangshuangyany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xyt.vehdjk.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qqd.sufxvd.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wuo.yueranfly.top

[D26] 数组转字符串
来源：http://pxo.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://xoa.xuanzx.com

PHP:  implode(", ", $arr);
来源：http://ouo.cqqwz.cn

JS:   arr.join(", ")
来源：http://dej.epnwcf.com

TS:   arr.join(", ")
来源：http://etl.fktsv.cn

Java: String.join(", ", list)
来源：http://xim.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://rtz.hcnkem.com

Ruby: arr.join(", ")
来源：http://xod.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://kpl.bjfxy.top

================================================================================
来源：http://xdl.xuanzx.com

E. 字符串处理
来源：http://kxz.gzhubu.top

================================================================================
来源：http://vcp.cqqwz.cn

[E01] 拼接字符串
来源：http://yeb.yvedp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sgg.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qan.dianchejie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dze.yueranfly.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vkr.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://trj.fehbvm.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wvf.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lvo.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tnv.yuanzhike.top

[E02] 重复字符串
来源：http://yqb.hywenlv.cn

Py:   "ab" * 3
来源：http://qoj.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://ghn.snrcjt.cn

JS:   "ab".repeat(3)
来源：http://umm.vehdjk.com

TS:   "ab".repeat(3)
来源：http://sgn.yuanzhike.top

Java: "ab".repeat(3)
来源：http://mgz.guannengcc.top

Go:   strings.Repeat("ab", 3)
来源：http://qqu.52xcode.cn

Ruby: "ab" * 3
来源：http://mpo.yj20258.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uey.nanxinkj.top

[E03] 截取子串
来源：http://axm.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jok.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nji.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qqr.yj20258.top

TS:   s.slice(1, 4)
来源：http://vmu.tian-w.cn

Java: s.substring(1, 4)
来源：http://nrp.jqgfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eda.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ohh.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://stl.redwolf501.top

[E04] 查找子串位置
来源：http://kvz.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://sei.wangdashe.top

PHP:  strpos($s, "x");
来源：http://xwh.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://izb.quarkkingdee.top

TS:   s.indexOf("x")
来源：http://pej.bbcook.cn

Java: s.indexOf("x")
来源：http://kgq.yj20258.top

Go:   strings.Index(s, "x")
来源：http://bgx.epnwcf.com

Ruby: s.index("x")
来源：http://pbt.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://qie.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dwt.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://apx.sxryk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vem.havefunace.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jgr.zhengqikj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pur.jqgfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://plo.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xus.9152youxi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qac.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sze.tian-w.cn

[E06] 替换子串
来源：http://qlz.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fme.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://efd.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lry.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://kmo.epnwcf.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://asa.ctjpmb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xft.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vls.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://qry.sjlbkw.cn

[E07] 按分隔符拆分
来源：http://ggi.hfpthk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://arm.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rlp.yueranfly.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zma.yangfankeji.com

TS:   s.split(",")
来源：http://opd.sysykeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://hfa.bjfxy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ods.yonumen.top

Ruby: s.split(",");  s.split
来源：http://fmd.yj20258888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fjp.chenzaomai.com

[E08] 数组按分隔符合并
来源：http://sgq.kuanghao11.cn

Py:   ",".join(items)
来源：http://ohw.ppjwa.cn

PHP:  implode(",", $items);
来源：http://pyn.vehdjk.com

JS:   items.join(",")
来源：http://dmn.guowangkeji.top

TS:   items.join(",")
来源：http://qst.yuanzhike.top

Java: String.join(",", items)
来源：http://tzx.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://mkb.yongpay.top

Ruby: items.join(",")
来源：http://dmc.hysaishi.cn

C#:   string.Join(",", items)
来源：http://czd.gogol.net.cn

[E09] 去除所有空白字符
来源：http://oke.smart0.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yda.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pec.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://fin.cdnleiting.top

TS:   s.replace(/\s+/g, "")
来源：http://hyw.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://rgm.chenjidiqi.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://aaq.cqqwz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nqk.pengpengdd.cyou

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nos.zdbjq.cn

[E10] 左侧补零 / 定长填充
来源：http://kdk.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://knb.snrcjt.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hzd.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://rba.jinqigfzy.top

TS:   "7".padStart(3, "0")
来源：http://btq.cdnleiting.top

Java: String.format("%03d", 7)
来源：http://yzt.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kva.zdqjudy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rxj.jinyuanbaomall.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://byz.nanxuanxn.top

[E11] 反转字符串
来源：http://qfi.birdmap.top

Py:   s[::-1]
来源：http://qxq.wangdashe.top

PHP:  strrev($s);
来源：http://jad.havefunace.top

JS:   [...s].reverse().join("")
来源：http://zqg.zhoulong.xyz

TS:   [...s].reverse().join("")
来源：http://glx.jiagoushi.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zbr.meibo888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wcy.guowangkeji.top

Ruby: s.reverse
来源：http://psi.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://ofa.pycfn.com

[E12] 统计某字符出现次数
来源：http://ncb.havefunace.top

Py:   s.count("a")
来源：http://pxe.sufxvd.cn

PHP:  substr_count($s, "a");
来源：http://fmf.sxryk.cn

JS:   s.split("a").length - 1
来源：http://ujb.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://lkn.meibo888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iyx.xuetiantiany.cn

Go:   strings.Count(s, "a")
来源：http://tjo.daxiang520.top

Ruby: s.count("a")
来源：http://kpg.chenjidiqi.icu

C#:   s.Count(c => c == 'a')
来源：http://hmb.gaohongyu789.top

[E13] 逐字符遍历
来源：http://ala.wangshuangyany.cn

Py:   for ch in s: print(ch)
来源：http://npr.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mgx.zhengqikj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tfh.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pxu.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bsf.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pwm.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qid.ivvv.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wxn.jianghu66.top

[E14] URL 编码与 Base64
来源：http://mjf.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hpy.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kzj.kuanghao11.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://agi.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fna.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xvc.hammf.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lox.epnwcf.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gtq.quarkkingdee.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qja.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://fpz.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jgt.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tmt.chenlongwang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yfu.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ezp.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dum.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zet.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pbz.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qtb.kuanghao11.cn

[E16] 数字千分位
来源：http://uqi.chenlongwang.top

Py:   f"{1234567:,}"
来源：http://kip.xuetiantiany.cn

PHP:  number_format(1234567);
来源：http://sqn.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mdl.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gcz.quarkkingdee.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lsq.yuanzhike.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hzs.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lzs.gotoacloud.top

C#:   1234567.ToString("N0")
来源：http://fhr.wangdashe.top

[E17] 首字母大写
来源：http://vnb.smart0.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://acf.vehdjk.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://odi.yj20258.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gga.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wtz.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gjy.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://czg.c1oappe.top

Ruby: s.capitalize
来源：http://yet.jinqigufen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://upq.ivvv.top

[E18] 模板占位符替换
来源：http://vxo.zhengqikj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jqb.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qms.havefunace.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vqw.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ola.wangshuangyany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ivg.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lus.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qvg.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ncw.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://hur.hcnkem.com

Py:   s.splitlines()
来源：http://sua.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eet.ehwqpu.com


<!-- 参考信息 -->