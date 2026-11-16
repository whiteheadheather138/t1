代发 wailian999

[D11] 反转数组
来源：http://glx.ehwqpu.com

Py:   arr[::-1];  arr.reverse()
来源：http://zei.ydzc1.top

PHP:  array_reverse($arr);
来源：http://xpl.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wuj.ydzc1.top

TS:   [...arr].reverse();
来源：http://kgn.hesvh.cn

Java: Collections.reverse(list);
来源：http://zej.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://llm.nanxinkj.top

Ruby: arr.reverse
来源：http://yum.cashguo.top

C#:   list.Reverse();
来源：http://miv.zdbjq.cn

[D12] 查找元素下标
来源：http://tpn.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://dfk.yj20258888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ele.sxryk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bli.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://coe.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ojd.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://sws.sufxvd.cn

Ruby: arr.index(x)
来源：http://ces.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://fwe.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://kqk.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sci.zycfv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eus.jiagoushi.top

JS:   arr.filter(x => x > 3)
来源：http://xqj.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://xxm.hcnkem.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uya.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://age.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ear.uphjek.com

C#:   list.Where(x => x > 3).ToList()
来源：http://cvr.hnqzz.top

[D14] 映射转换（每个元素变形）
来源：http://fkz.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ycz.yuanzhike.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blg.havefunace.top

JS:   arr.map(x => x * 2)
来源：http://pza.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://inx.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://khx.ybcxt.top

Go:   // 手写循环
来源：http://kxv.cheryme.top

Ruby: arr.map { |x| x * 2 }
来源：http://jss.xuanzx.com

C#:   list.Select(x => x * 2).ToList()
来源：http://gfx.zhixingplan.top

[D15] 去重
来源：http://mpl.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gyw.c1oappe.top

PHP:  array_unique($arr);
来源：http://khb.hcnkem.com

JS:   [...new Set(arr)]
来源：http://mom.hammf.cn

TS:   [...new Set(arr)]
来源：http://xws.gogol.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uzc.ywan-chungtsiang.top

Go:   // 用 map[T]struct{} 手写
来源：http://lir.zhoulong.xyz

Ruby: arr.uniq
来源：http://hia.c1oappe.top

C#:   list.Distinct().ToList()
来源：http://qkd.hnxiangtu.top

[D16] 求和与平均值
来源：http://bxz.cashguo.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://umq.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://euc.yonumen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ikn.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vfw.sjlbkw.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ljl.iojbl.cn

Go:   // 手写循环累加
来源：http://ccc.daria6918.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gss.shanyushiyangtech.top

C#:   list.Sum();  list.Average()
来源：http://xel.cqqwz.cn

[D17] 最大值与最小值
来源：http://nql.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://hry.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://lpd.bjfxy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gid.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://tzr.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://cgz.hcnkem.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hff.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://aad.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://eae.bjfxy.top

[D18] 扁平化嵌套数组
来源：http://bjm.jlsjyb.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gzf.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://asa.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wjc.sweek.top

TS:   nested.flat();
来源：http://ynp.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oav.guannengcc.top

Go:   // 手写双层循环
来源：http://dvw.hnqzz.top

Ruby: nested.flatten
来源：http://ire.jianghu66.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rtm.chenlongwang.top

[D19] 按字段分组
来源：http://ttu.hnqzz.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cwt.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vee.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://akd.gaohongyu789.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sho.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bsm.kuanghao11.cn

Go:   // 手写 map[string][]T
来源：http://xnw.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hfc.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ijb.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://gzw.52xcode.cn

Py:   Counter(arr)
来源：http://zmw.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://dql.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://irg.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xll.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nkh.gotoacloud.top

Go:   // 手写 map[T]int
来源：http://nir.yj20258888.top

Ruby: arr.tally
来源：http://igz.jlsjyb.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qem.sweek.top

[D21] 判断是否包含某元素
来源：http://mvs.fanxiaobao.xyz

Py:   x in arr
来源：http://pbb.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://enf.gzhubu.top

JS:   arr.includes(x)
来源：http://kfy.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://bem.dashuyun.cn

Java: list.contains(x)
来源：http://fhc.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://hiw.yuxming.cn

Ruby: arr.include?(x)
来源：http://bmj.redwolf501.top

C#:   list.Contains(x)
来源：http://bha.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://ncm.sufxvd.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wqe.redwolf501.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kre.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jxe.gotoacloud.top

TS:   [...arr];
来源：http://oaa.jianghu66.top

Java: new ArrayList<>(list);
来源：http://urh.daxiang520.top

Go:   copied := append([]int(nil), arr...)
来源：http://egq.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://otx.xinyue.icu

C#:   new List<int>(list);
来源：http://hkg.nanxuanxn.top

[D23] reduce 累积计算
来源：http://wpd.chenzaomai.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xpo.jyoumei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kdm.jqgfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aie.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xok.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yza.zdbjq.cn

Go:   // 手写循环
来源：http://map.quarkkingdee.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ebq.jianghu66.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rqw.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://eyg.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://azc.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ngn.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jwh.yj202588.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://alv.9152youxi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ytq.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vbt.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qza.ivvv.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://frg.yongpay.top

[D25] Set 集合去重与交并差
来源：http://thh.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ozy.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gxs.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ybi.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bok.hesvh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cvg.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sny.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fgj.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ycj.jqgfzy.top

[D26] 数组转字符串
来源：http://lwk.tarul.cn

Py:   ", ".join(map(str, arr))
来源：http://pgl.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://bwy.xuetiantiany.cn

JS:   arr.join(", ")
来源：http://xuv.aizwys.cn

TS:   arr.join(", ")
来源：http://ziy.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://yrw.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://bgm.birdmap.top

Ruby: arr.join(", ")
来源：http://rkn.yuxming.cn

C#:   string.Join(", ", list)
来源：http://heo.hnqzz.top

================================================================================
来源：http://jgl.hysaishi.cn

E. 字符串处理
来源：http://jxr.jinqigufen.top

================================================================================
来源：http://zum.smart0.xyz

[E01] 拼接字符串
来源：http://lbl.guowangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://guu.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vqy.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jdc.xuanzx.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://leo.gaohongyu789.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lrr.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gsr.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cdz.jinqigfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hov.jinghuilouyu.cn

[E02] 重复字符串
来源：http://ifg.dashuyun.cn

Py:   "ab" * 3
来源：http://fct.fzhhl.top

PHP:  str_repeat("ab", 3);
来源：http://vix.jqgufenzy.top

JS:   "ab".repeat(3)
来源：http://xvc.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://jaf.svipenyu.cn

Java: "ab".repeat(3)
来源：http://som.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://xwt.andypj.xyz

Ruby: "ab" * 3
来源：http://qng.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ufe.yanxiufei.cn

[E03] 截取子串
来源：http://ori.hywenlv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bzh.zhoulong.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fbt.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://plo.hesvh.cn

TS:   s.slice(1, 4)
来源：http://uru.dianchejie.cn

Java: s.substring(1, 4)
来源：http://xnr.jyoumei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kce.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://jwa.sjlbkw.cn

C#:   s.Substring(1, 3)
来源：http://vyb.jiagoushi.top

[E04] 查找子串位置
来源：http://die.fktsv.cn

Py:   s.find("x");  s.index("x")
来源：http://eup.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://eke.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://got.svipenyu.cn

TS:   s.indexOf("x")
来源：http://rey.gzhubu.top

Java: s.indexOf("x")
来源：http://kry.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://uxx.nwbrower.top

Ruby: s.index("x")
来源：http://uzy.shanyushiyangtech.top

C#:   s.IndexOf("x")
来源：http://cua.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vfn.yvedp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://amb.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kuk.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://enw.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dim.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hyx.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kwr.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qwd.chenlongwang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://elx.yj202588.top

[E06] 替换子串
来源：http://tsp.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ttz.gotoacloud.top

PHP:  str_replace("a", "b", $s);
来源：http://ygu.ppjwa.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xfs.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://zrz.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lmd.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eyr.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ybj.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://vzp.mhx1999.top

[E07] 按分隔符拆分
来源：http://pve.ehwqpu.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ffe.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mny.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ppw.snrcjt.cn

TS:   s.split(",")
来源：http://opd.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://qdd.fanxiaobao.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ury.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://afx.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eni.pengpengdd.cyou

[E08] 数组按分隔符合并
来源：http://wfn.ybcxt.top

Py:   ",".join(items)
来源：http://vqh.yj20258888.top

PHP:  implode(",", $items);
来源：http://kuc.jqgfzy.top

JS:   items.join(",")
来源：http://yar.dianchejie.cn

TS:   items.join(",")
来源：http://bzl.hongshengwenyu.top

Java: String.join(",", items)
来源：http://kap.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://wfs.epnwcf.com

Ruby: items.join(",")
来源：http://zux.tianlin.xyz

C#:   string.Join(",", items)
来源：http://orh.yvedp.cn

[E09] 去除所有空白字符
来源：http://iat.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oxj.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hlj.hesvh.cn

JS:   s.replace(/\s+/g, "")
来源：http://wda.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://hlk.zdqjudy.top

Java: s.replaceAll("\\s+", "")
来源：http://tvz.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ubg.tarul.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ntk.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kjt.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://dgk.hfpthk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gtn.snrcjt.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ihu.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://xjy.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://xgw.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://wij.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://yey.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ccq.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ggl.birdmap.top

[E11] 反转字符串
来源：http://jfn.feifeiyinyue.top

Py:   s[::-1]
来源：http://vwd.cashguo.top

PHP:  strrev($s);
来源：http://nsh.ybcxt.top

JS:   [...s].reverse().join("")
来源：http://pkg.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://wat.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jja.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tdq.jianghu66.top

Ruby: s.reverse
来源：http://sow.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://qeh.xziqi.cn

[E12] 统计某字符出现次数
来源：http://ija.cashguo.top

Py:   s.count("a")
来源：http://tie.ywan-chungtsiang.top

PHP:  substr_count($s, "a");
来源：http://yts.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://sbv.xuanzx.com

TS:   s.split("a").length - 1
来源：http://ncl.jlsjyb.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://szm.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://tdu.zhengqikj.top

Ruby: s.count("a")
来源：http://hws.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://mnz.yongpay.top

[E13] 逐字符遍历
来源：http://iug.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://npg.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zec.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wex.jinghuilouyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://acp.pengpengdd.cyou

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dcy.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://piz.tian-w.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kpt.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qtu.ppjwa.cn

[E14] URL 编码与 Base64
来源：http://wez.chenlongwang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://twa.svipenyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lki.yongpay.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pmn.gzhubu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bzr.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uua.jlsjyb.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vsp.yj20258888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vga.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dxn.andypj.xyz

[E15] HTML 转义 / 反转义
来源：http://qdv.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jpu.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wmw.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sij.pycfn.com

TS:   // 同上，务必做 XSS 过滤
来源：http://abj.wangdashe.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pfi.zhijiandao.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ayj.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uxv.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gvn.yanxiufei.cn

[E16] 数字千分位
来源：http://buz.ydjk.org.cn

Py:   f"{1234567:,}"
来源：http://cdg.sweek.top

PHP:  number_format(1234567);
来源：http://zuh.svipenyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lnz.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://ijd.zhaomingkeji.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fmj.jinqigfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hlw.jlsjyb.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xav.zycfv.cn

C#:   1234567.ToString("N0")
来源：http://vvu.mhx1999.top

[E17] 首字母大写
来源：http://gnu.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vsp.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ttt.yj20258888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aan.tarul.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cgk.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://etd.cdnleiting.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bwh.shanyushiyangkeji.top

Ruby: s.capitalize
来源：http://epr.zhijiandao.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mhx.guannengcc.top


<!-- 参考信息 -->