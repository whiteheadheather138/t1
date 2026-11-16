代发 wailian999

[D11] 反转数组
来源：http://nyk.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://vfb.316326.xyz

PHP:  array_reverse($arr);
来源：http://lsb.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vsf.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://sqb.cucudq.cn

Java: Collections.reverse(list);
来源：http://khp.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://nzv.zycfv.cn

Ruby: arr.reverse
来源：http://opw.shangyingyoupin.top

C#:   list.Reverse();
来源：http://rom.yueranfly.top

[D12] 查找元素下标
来源：http://vps.yj20258888.top

Py:   arr.index(x);  x in arr
来源：http://jtj.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yqw.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tbn.cdnleiting.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zgy.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dvw.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://lcm.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://trs.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://ffz.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://pgc.jyoumei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hyf.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qla.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://oeh.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://eeh.gogol.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wjt.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qtk.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fie.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fmm.shangyingyoupin.top

[D14] 映射转换（每个元素变形）
来源：http://qbw.yongpay.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fyt.0kj1m.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lvh.yj202588.top

JS:   arr.map(x => x * 2)
来源：http://uyc.zdqjudy.top

TS:   arr.map(x => x * 2)
来源：http://wli.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hwt.bjfxy.top

Go:   // 手写循环
来源：http://wqd.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://otz.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ajy.shanyushiyangkeji.top

[D15] 去重
来源：http://epn.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bvn.fengsongda.top

PHP:  array_unique($arr);
来源：http://txo.yvedp.cn

JS:   [...new Set(arr)]
来源：http://gwu.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://evi.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tzf.iojbl.cn

Go:   // 用 map[T]struct{} 手写
来源：http://adx.iojbl.cn

Ruby: arr.uniq
来源：http://uud.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://pio.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://vmv.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://snn.wangshuangyany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://noi.redwolf501.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iri.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hvf.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tdh.9152youxi.cn

Go:   // 手写循环累加
来源：http://dkk.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fzh.yvedp.cn

C#:   list.Sum();  list.Average()
来源：http://ckc.shangyingyoupin.top

[D17] 最大值与最小值
来源：http://dfl.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://sfp.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://vmd.zhongyouzk.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://khr.yj20258888.top

TS:   Math.max(...arr);
来源：http://wmg.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zrs.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gcc.yonumen.top

Ruby: arr.max;  arr.min
来源：http://usl.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://qel.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://ttp.sysykeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lwu.aibaodan.cn

PHP:  array_merge(...$nested);
来源：http://lkc.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kun.fanxiaobao.xyz

TS:   nested.flat();
来源：http://ckp.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jak.hywenlv.cn

Go:   // 手写双层循环
来源：http://meo.zhiwuduotai.top

Ruby: nested.flatten
来源：http://ose.gogol.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zte.ctjpmb.com

[D19] 按字段分组
来源：http://qwg.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ivo.fengsongda.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jds.fzhhl.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jhl.quarkkingdee.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qmr.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://npn.yongpay.top

Go:   // 手写 map[string][]T
来源：http://pfj.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://oxv.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xzd.yuxming.cn

[D20] 统计每个元素出现次数
来源：http://qpq.yongpay.top

Py:   Counter(arr)
来源：http://vis.zhoulong.xyz

PHP:  array_count_values($arr);
来源：http://xpy.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zyj.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qqh.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qso.ctjpmb.com

Go:   // 手写 map[T]int
来源：http://qsq.zhaomingkeji.xyz

Ruby: arr.tally
来源：http://whh.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wup.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://joa.c1oappe.top

Py:   x in arr
来源：http://hkj.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://dfx.shzxlz.cn

JS:   arr.includes(x)
来源：http://jzz.yj20258888.top

TS:   arr.includes(x)
来源：http://dor.ydjk.org.cn

Java: list.contains(x)
来源：http://puo.quarkkingdee.top

Go:   slices.Contains(arr, x)
来源：http://jro.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://ogn.sxryk.cn

C#:   list.Contains(x)
来源：http://mkj.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://jgj.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ogw.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://agd.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cnn.tian-w.cn

TS:   [...arr];
来源：http://cua.yj20258888.top

Java: new ArrayList<>(list);
来源：http://ldh.cucudq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cdj.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://rrm.dashuyun.cn

C#:   new List<int>(list);
来源：http://rmq.fanxiaobao.xyz

[D23] reduce 累积计算
来源：http://dua.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tgw.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zjf.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://boe.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ojk.ehwqpu.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://rtk.9152youxi.cn

Go:   // 手写循环
来源：http://jzf.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ubd.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mqg.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://svk.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ehd.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mtc.fzhhl.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zsl.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dby.chenzaomai.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yfi.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zuq.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ekk.mhx1999.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vey.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://vbc.bbcook.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://afn.guowangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mvx.gzhubu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://acs.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mkh.nanxinkj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qut.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://evn.quarkkingdee.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zoq.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nek.9152youxi.cn

[D26] 数组转字符串
来源：http://lcm.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://kes.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://day.yonumen.top

JS:   arr.join(", ")
来源：http://rpk.fktsv.cn

TS:   arr.join(", ")
来源：http://trg.yongpay.top

Java: String.join(", ", list)
来源：http://yhc.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://ksl.wangshuangyany.cn

Ruby: arr.join(", ")
来源：http://umx.vqdsnc.cn

C#:   string.Join(", ", list)
来源：http://bpq.mhx1999.top

================================================================================
来源：http://fsp.nwbrower.top

E. 字符串处理
来源：http://eat.mhx1999.top

================================================================================
来源：http://old.zdqjudy.top

[E01] 拼接字符串
来源：http://nly.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tel.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jom.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://csv.guannengcc.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://omz.hnxiangtu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jvs.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nig.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vsp.cdnleiting.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cra.jianghu66.top

[E02] 重复字符串
来源：http://ywj.fktsv.cn

Py:   "ab" * 3
来源：http://gnk.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://kar.cheryme.top

JS:   "ab".repeat(3)
来源：http://vzs.ybcxt.top

TS:   "ab".repeat(3)
来源：http://mqa.chenjidiqi.icu

Java: "ab".repeat(3)
来源：http://uzs.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://jga.yvedp.cn

Ruby: "ab" * 3
来源：http://rfi.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tgq.sweek.top

[E03] 截取子串
来源：http://xua.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tnu.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://drn.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pzx.sjlbkw.cn

TS:   s.slice(1, 4)
来源：http://wkj.guowangkeji.top

Java: s.substring(1, 4)
来源：http://nou.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jyw.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://ynr.zdbjq.cn

C#:   s.Substring(1, 3)
来源：http://wfl.sjlbkw.cn

[E04] 查找子串位置
来源：http://zsw.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://kyy.chenlongwang.top

PHP:  strpos($s, "x");
来源：http://uiv.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lzs.cqqwz.cn

TS:   s.indexOf("x")
来源：http://lve.nanxinkj.top

Java: s.indexOf("x")
来源：http://ysd.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://cmw.tian-w.cn

Ruby: s.index("x")
来源：http://sds.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://nov.epnwcf.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://haw.hnxiangtu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sbc.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vee.epnwcf.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wgv.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vgt.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nzc.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lkv.c1oappe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yem.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jkz.52xcode.cn

[E06] 替换子串
来源：http://tef.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kxb.hfpthk.cn

PHP:  str_replace("a", "b", $s);
来源：http://ebi.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dew.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://izw.jqgfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eme.shanyushiyangtech.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gkn.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nbe.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://iej.zdqjudy.top

[E07] 按分隔符拆分
来源：http://xxy.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xvn.wangdashe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mmo.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vqp.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://qec.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://sdy.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gjk.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://adv.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oun.pycfn.com

[E08] 数组按分隔符合并
来源：http://hyl.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://osh.zdqjudy.top

PHP:  implode(",", $items);
来源：http://gmg.yj20258888.top

JS:   items.join(",")
来源：http://nux.zhaomingkeji.xyz

TS:   items.join(",")
来源：http://tov.jinyuanbaomall.cn

Java: String.join(",", items)
来源：http://chi.yanxiufei.cn

Go:   strings.Join(items, ",")
来源：http://yqx.c1oappe.top

Ruby: items.join(",")
来源：http://xnw.tanke756.top

C#:   string.Join(",", items)
来源：http://ylt.yangfankeji.com

[E09] 去除所有空白字符
来源：http://vhl.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zpb.hcnkem.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hgg.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://irp.jqgfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://xwy.cqqwz.cn

Java: s.replaceAll("\\s+", "")
来源：http://nwi.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qbl.cucudq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jij.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kgg.hnqzz.top

[E10] 左侧补零 / 定长填充
来源：http://yln.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mpr.cashguo.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://guv.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://dtg.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://aij.yj20258.top

Java: String.format("%03d", 7)
来源：http://xma.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://njs.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hii.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ndy.yuanzhike.top

[E11] 反转字符串
来源：http://mfo.kuanghao11.cn

Py:   s[::-1]
来源：http://zto.xylfe.cn

PHP:  strrev($s);
来源：http://czl.ydjk.org.cn

JS:   [...s].reverse().join("")
来源：http://paw.zhixingplan.top

TS:   [...s].reverse().join("")
来源：http://lpb.uphjek.com

Java: new StringBuilder(s).reverse().toString()
来源：http://dic.vqdsnc.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zps.guowangkeji.top

Ruby: s.reverse
来源：http://nhp.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://wnu.zhijiandao.cn

[E12] 统计某字符出现次数
来源：http://pzb.hywenlv.cn

Py:   s.count("a")
来源：http://mca.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://rye.hnqzz.top

JS:   s.split("a").length - 1
来源：http://zmk.sufxvd.cn

TS:   s.split("a").length - 1
来源：http://utz.hnqzz.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fck.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://jzq.dashuyun.cn

Ruby: s.count("a")
来源：http://hzw.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://zxg.guannengcc.top

[E13] 逐字符遍历
来源：http://xoa.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://ijt.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yzd.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yfb.tarul.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yoh.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rti.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tjn.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pme.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tye.yuanzhike.top

[E14] URL 编码与 Base64
来源：http://lzm.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jaq.shuidangran.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://obt.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tpp.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tja.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vmh.xinyue.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fsd.fktsv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xcg.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dhr.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://iys.ppjwa.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hdh.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xwz.ehwqpu.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ukb.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hpo.xuanzx.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qez.jianghu66.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sbv.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jod.yj20258.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uns.jyoumei.cn

[E16] 数字千分位
来源：http://tcl.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://yso.hywenlv.cn

PHP:  number_format(1234567);
来源：http://iga.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cpf.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://oer.feifeiyinyue.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nbp.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fxk.hesvh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rrc.ydjk.org.cn

C#:   1234567.ToString("N0")
来源：http://dia.yvedp.cn

[E17] 首字母大写
来源：http://jjx.haohaochexian.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rvw.hywenlv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://idi.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://myf.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://der.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lrx.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bqx.zhixingplan.top

Ruby: s.capitalize
来源：http://ukd.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zom.uphjek.com


<!-- 参考信息 -->