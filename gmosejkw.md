代发 wailian999

C#:   list.Reverse();
来源：http://njz.redwolf501.top

[D12] 查找元素下标
来源：http://nar.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://tpz.shangyingyoupin.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xlf.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tre.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://erl.snrcjt.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wuq.shuidangran.top

Go:   slices.Index(arr, x)
来源：http://otw.ydzc1.top

Ruby: arr.index(x)
来源：http://hek.jyoumei.cn

C#:   list.IndexOf(x);
来源：http://grm.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://vgu.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nrk.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bgs.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://sxr.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://lwx.sysykeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jlb.aibaodan.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://piw.zhixingplan.top

Ruby: arr.select { |x| x > 3 }
来源：http://fig.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vfx.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://gbm.9152youxi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rth.yfazqb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://exc.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://rmz.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://uie.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://voi.9152youxi.cn

Go:   // 手写循环
来源：http://wcf.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://pgz.iojbl.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ljb.nwbrower.top

[D15] 去重
来源：http://cvc.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://spi.shzxlz.cn

PHP:  array_unique($arr);
来源：http://mzd.xylfe.cn

JS:   [...new Set(arr)]
来源：http://yal.ivvv.top

TS:   [...new Set(arr)]
来源：http://qco.aizwys.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://irw.mhx1999.top

Go:   // 用 map[T]struct{} 手写
来源：http://elh.ybcxt.top

Ruby: arr.uniq
来源：http://kek.zhongyouzk.top

C#:   list.Distinct().ToList()
来源：http://etu.aizwys.cn

[D16] 求和与平均值
来源：http://mry.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dpn.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ads.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mxl.jinqigufen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://szx.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baf.quarkkingdee.top

Go:   // 手写循环累加
来源：http://ipe.fanxiaobao.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://axn.gzhubu.top

C#:   list.Sum();  list.Average()
来源：http://xpp.fehbvm.com

[D17] 最大值与最小值
来源：http://mfr.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://qiy.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://avf.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://laj.dashuyun.cn

TS:   Math.max(...arr);
来源：http://hkv.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://biu.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tmh.fanxiaobao.xyz

Ruby: arr.max;  arr.min
来源：http://cwl.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://ium.yonumen.top

[D18] 扁平化嵌套数组
来源：http://gos.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ypa.mhx1999.top

PHP:  array_merge(...$nested);
来源：http://fqy.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yfr.yj20258888.top

TS:   nested.flat();
来源：http://ibo.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ydp.kuanghao11.cn

Go:   // 手写双层循环
来源：http://nqt.uphjek.com

Ruby: nested.flatten
来源：http://xcq.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kcv.hnxiangtu.top

[D19] 按字段分组
来源：http://laz.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dit.cqqwz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dps.jlsjyb.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://srk.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ito.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://typ.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://fzg.jqgufenzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rro.hcnkem.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rdy.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://eym.zhoulong.xyz

Py:   Counter(arr)
来源：http://hrh.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://dba.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gng.fktsv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ipn.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gqy.ydzc1.top

Go:   // 手写 map[T]int
来源：http://wqr.uphjek.com

Ruby: arr.tally
来源：http://yok.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qwf.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://sak.yuanzhike.top

Py:   x in arr
来源：http://jhx.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://jmb.fanxiaobao.xyz

JS:   arr.includes(x)
来源：http://uge.yueranfly.top

TS:   arr.includes(x)
来源：http://yyj.quarkkingdee.top

Java: list.contains(x)
来源：http://xpy.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://rsr.yongpay.top

Ruby: arr.include?(x)
来源：http://tyw.yangfankeji.com

C#:   list.Contains(x)
来源：http://xhd.yueranfly.top

[D22] 复制数组（避免共享引用）
来源：http://mdd.xinyue.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ruf.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uzd.zhaomingkeji.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ryf.hesvh.cn

TS:   [...arr];
来源：http://nel.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://ejx.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tvz.hnxiangtu.top

Ruby: arr.dup;  arr.clone
来源：http://qgn.sjlbkw.cn

C#:   new List<int>(list);
来源：http://usr.redwolf501.top

[D23] reduce 累积计算
来源：http://zna.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mbz.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bfh.jqgfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vin.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://njr.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://luk.tian-w.cn

Go:   // 手写循环
来源：http://iik.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wyu.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tuy.daria6918.cn

[D24] 字典 / Map 基本操作
来源：http://bbz.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wdu.aizwys.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://esd.hongshengwenyu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sbx.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sfp.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mwr.tanke756.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yyc.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wee.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kam.snrcjt.cn

[D25] Set 集合去重与交并差
来源：http://ziq.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rbl.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vhe.haohaochexian.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gul.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://isj.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cuc.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tsf.mhx1999.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pme.ydzc1.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eho.cucudq.cn

[D26] 数组转字符串
来源：http://wav.meibo888.top

Py:   ", ".join(map(str, arr))
来源：http://bfc.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://fnk.vqdsnc.cn

JS:   arr.join(", ")
来源：http://tlh.yuanzhike.top

TS:   arr.join(", ")
来源：http://juy.yvedp.cn

Java: String.join(", ", list)
来源：http://sxh.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://qfh.52xcode.cn

Ruby: arr.join(", ")
来源：http://mxa.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://xmd.guowangkeji.top

================================================================================
来源：http://lmq.zycfv.cn

E. 字符串处理
来源：http://aer.zhongyouzk.top

================================================================================
来源：http://uxk.wangshuangyany.cn

[E01] 拼接字符串
来源：http://kye.ywan-chungtsiang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ikp.aizwys.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gqu.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://slv.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nbe.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kow.zhiwuduotai.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gpl.hnxiangtu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iza.zhijiandao.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xib.hnxiangtu.top

[E02] 重复字符串
来源：http://tdv.smart0.xyz

Py:   "ab" * 3
来源：http://bad.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://wsq.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://kda.bbcook.cn

TS:   "ab".repeat(3)
来源：http://hwk.shanyushiyangtech.top

Java: "ab".repeat(3)
来源：http://xaz.hnqzz.top

Go:   strings.Repeat("ab", 3)
来源：http://gmm.sweek.top

Ruby: "ab" * 3
来源：http://fpn.shanyushiyangtech.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vcp.jinghuilouyu.cn

[E03] 截取子串
来源：http://fcj.0kj1m.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tro.zhixingplan.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://umd.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jwq.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://ngw.0kj1m.cn

Java: s.substring(1, 4)
来源：http://xxs.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pkh.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://drl.sweek.top

C#:   s.Substring(1, 3)
来源：http://tpx.zhijiandao.cn

[E04] 查找子串位置
来源：http://gyf.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://etz.jqgufenzy.top

PHP:  strpos($s, "x");
来源：http://qss.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qtx.tarul.cn

TS:   s.indexOf("x")
来源：http://znp.pycfn.com

Java: s.indexOf("x")
来源：http://pwg.bjfxy.top

Go:   strings.Index(s, "x")
来源：http://qyl.sysykeji.top

Ruby: s.index("x")
来源：http://okm.ydjk.org.cn

C#:   s.IndexOf("x")
来源：http://vpj.chenjidiqi.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://eps.zdqjudy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ost.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xti.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bkx.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://msf.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://esl.cdnleiting.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tct.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rdd.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tnw.ybcxt.top

[E06] 替换子串
来源：http://afp.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://crr.jyoumei.cn

PHP:  str_replace("a", "b", $s);
来源：http://jhv.fanxiaobao.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://obs.xingfuxueyuan.xyz

TS:   s.replaceAll("a", "b")
来源：http://yew.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lgl.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jcc.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rtk.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://kdn.wangdashe.top

[E07] 按分隔符拆分
来源：http://ftf.jiagoushi.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://psw.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nrg.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gvu.xingfuxueyuan.xyz

TS:   s.split(",")
来源：http://skv.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://cxh.fehbvm.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qlx.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://gfw.aibaodan.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://drw.aizwys.cn

[E08] 数组按分隔符合并
来源：http://xzq.yvedp.cn

Py:   ",".join(items)
来源：http://xqg.iojbl.cn

PHP:  implode(",", $items);
来源：http://bgg.jqgfzy.top

JS:   items.join(",")
来源：http://vqt.nwbrower.top

TS:   items.join(",")
来源：http://dqx.havefunace.top

Java: String.join(",", items)
来源：http://lep.dashuyun.cn

Go:   strings.Join(items, ",")
来源：http://hhp.yj202588.top

Ruby: items.join(",")
来源：http://zxf.guannengcc.top

C#:   string.Join(",", items)
来源：http://sne.daxiang520.top

[E09] 去除所有空白字符
来源：http://mcm.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lox.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wyu.cheryme.top

JS:   s.replace(/\s+/g, "")
来源：http://zsd.xuanzx.com

TS:   s.replace(/\s+/g, "")
来源：http://ezh.hywenlv.cn

Java: s.replaceAll("\\s+", "")
来源：http://gpg.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zzy.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kyp.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://agw.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://vft.316326.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jjy.0kj1m.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vkj.fehbvm.com

JS:   "7".padStart(3, "0")
来源：http://pme.ydzc1.top

TS:   "7".padStart(3, "0")
来源：http://hxa.cdnleiting.top

Java: String.format("%03d", 7)
来源：http://nmq.yj20258.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rfa.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gga.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nps.nanxuanxn.top

[E11] 反转字符串
来源：http://jdj.nanxuanxn.top

Py:   s[::-1]
来源：http://sbx.snrcjt.cn

PHP:  strrev($s);
来源：http://dqc.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://hsq.nanxinkj.top

TS:   [...s].reverse().join("")
来源：http://qvi.ybcxt.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xpi.nanxuanxn.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://aly.aibaodan.cn

Ruby: s.reverse
来源：http://lau.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://pix.havefunace.top

[E12] 统计某字符出现次数
来源：http://xak.yj202588.top

Py:   s.count("a")
来源：http://itx.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://tmj.cdnleiting.top

JS:   s.split("a").length - 1
来源：http://jed.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://qvv.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ere.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://swd.chenjidiqi.icu

Ruby: s.count("a")
来源：http://jnj.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://bry.gogol.net.cn

[E13] 逐字符遍历
来源：http://loy.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://icm.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jgi.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bou.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sti.jianghu66.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://phn.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hkb.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xvx.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bsp.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://bnp.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nph.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bgf.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zjl.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gzh.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://guy.hcnkem.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ypx.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bxp.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wiu.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://aik.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mkp.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fpg.yj20258.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cwh.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://dth.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sgc.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://poz.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dtr.dashuyun.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://shs.c1oappe.top

[E16] 数字千分位
来源：http://imq.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://xtt.ehwqpu.com

PHP:  number_format(1234567);
来源：http://hlj.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wgk.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jwn.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yzq.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eet.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nwz.jinqigufen.top

C#:   1234567.ToString("N0")
来源：http://oya.jqgufenzy.top

[E17] 首字母大写
来源：http://rlp.jqgfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://doq.zhongyouzk.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uwv.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dkg.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iak.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://asy.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wyk.0kj1m.cn

Ruby: s.capitalize
来源：http://zbd.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tnt.cashguo.top

[E18] 模板占位符替换
来源：http://fxu.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://leh.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ymf.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fxt.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lco.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dqr.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cmy.wangdashe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nyv.zhaomingkeji.xyz


<!-- 参考信息 -->