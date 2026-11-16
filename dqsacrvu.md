代发 wailian999

TS:   [...arr].reverse();
来源：http://dyd.guowangkeji.top

Java: Collections.reverse(list);
来源：http://ezv.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://dyp.zdbjq.cn

Ruby: arr.reverse
来源：http://nfs.nanxinkj.top

C#:   list.Reverse();
来源：http://tvu.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://yeg.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://mez.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fgt.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bkf.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yji.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uth.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://fop.52xcode.cn

Ruby: arr.index(x)
来源：http://stk.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://xee.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://xbg.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xwa.xylfe.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sxd.meibo888.top

JS:   arr.filter(x => x > 3)
来源：http://fst.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://bcq.wangshuangyany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zmy.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bux.shanyushiyangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://mnh.shanyushiyangtech.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vpl.sjlbkw.cn

[D14] 映射转换（每个元素变形）
来源：http://rag.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xsk.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zgh.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://wal.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://jxg.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rii.tanke756.top

Go:   // 手写循环
来源：http://nsu.xylfe.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iuo.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://swu.zhengqikj.top

[D15] 去重
来源：http://hwn.shanyushiyangtech.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pcq.uphjek.com

PHP:  array_unique($arr);
来源：http://ler.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://iwb.hcnkem.com

TS:   [...new Set(arr)]
来源：http://dpa.xziqi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yfv.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://glg.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://ogt.yongpay.top

C#:   list.Distinct().ToList()
来源：http://fqf.uphjek.com

[D16] 求和与平均值
来源：http://rjl.aizwys.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tiy.yvedp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qgu.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://suj.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://whl.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uai.sxryk.cn

Go:   // 手写循环累加
来源：http://jcj.hesvh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kdv.hesvh.cn

C#:   list.Sum();  list.Average()
来源：http://rnl.guowangkeji.top

[D17] 最大值与最小值
来源：http://zps.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://bhr.tian-w.cn

PHP:  max($arr);  min($arr);
来源：http://ykc.xuetiantiany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jzl.9152youxi.cn

TS:   Math.max(...arr);
来源：http://kvt.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tpf.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zgs.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://wqz.yueranfly.top

C#:   list.Max();  list.Min()
来源：http://mda.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://suc.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oqi.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://sfy.wangdashe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jcj.xuanzx.com

TS:   nested.flat();
来源：http://htd.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lha.iojbl.cn

Go:   // 手写双层循环
来源：http://iae.yonumen.top

Ruby: nested.flatten
来源：http://eej.svipenyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pqb.svipenyu.cn

[D19] 按字段分组
来源：http://bkk.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tjt.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dig.yj20258.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xgz.yongpay.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uzc.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ppd.daxiang520.top

Go:   // 手写 map[string][]T
来源：http://ghp.0kj1m.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bxp.tianlin.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ehk.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://jiy.haohaochexian.top

Py:   Counter(arr)
来源：http://fbn.cheryme.top

PHP:  array_count_values($arr);
来源：http://pzd.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hrw.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yvg.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uxi.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://jhm.zhoulong.xyz

Ruby: arr.tally
来源：http://dmn.zdbjq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wup.xylfe.cn

[D21] 判断是否包含某元素
来源：http://bkq.52xcode.cn

Py:   x in arr
来源：http://kff.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://vmh.ybcxt.top

JS:   arr.includes(x)
来源：http://dke.epnwcf.com

TS:   arr.includes(x)
来源：http://uxs.mhx1999.top

Java: list.contains(x)
来源：http://mtv.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://lrq.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://ifd.jlsjyb.cn

C#:   list.Contains(x)
来源：http://isc.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://xbl.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hxk.ywan-chungtsiang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jpy.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ihn.dashuyun.cn

TS:   [...arr];
来源：http://ykx.cucudq.cn

Java: new ArrayList<>(list);
来源：http://apl.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://kyz.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://ecj.guowangkeji.top

C#:   new List<int>(list);
来源：http://jbq.yj20258888.top

[D23] reduce 累积计算
来源：http://akt.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://whx.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zzu.316326.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oqc.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://obp.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sbu.hywenlv.cn

Go:   // 手写循环
来源：http://nvp.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wkh.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ayp.yj20258.top

[D24] 字典 / Map 基本操作
来源：http://vcs.xingfuxueyuan.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qkx.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tso.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lcp.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cxu.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://abu.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hof.quarkkingdee.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vwo.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zdm.hysaishi.cn

[D25] Set 集合去重与交并差
来源：http://qkw.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kky.birdmap.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://znd.jianghu66.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hid.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lle.yj20258888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qcb.xinyue.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wne.xziqi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://exl.jinqigfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://raz.sjlbkw.cn

[D26] 数组转字符串
来源：http://qtr.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://gbz.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://fmh.jinghuilouyu.cn

JS:   arr.join(", ")
来源：http://zdi.haohaochexian.top

TS:   arr.join(", ")
来源：http://hhl.shzxlz.cn

Java: String.join(", ", list)
来源：http://oad.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://yzv.jinghuilouyu.cn

Ruby: arr.join(", ")
来源：http://rmb.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://frp.xinyue.icu

================================================================================
来源：http://iyf.hammf.cn

E. 字符串处理
来源：http://tta.yanxiufei.cn

================================================================================
来源：http://nwy.sufxvd.cn

[E01] 拼接字符串
来源：http://rez.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://biy.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ndv.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oug.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wkd.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mlj.zhongyouzk.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iek.feifeiyinyue.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ynf.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://whp.yvedp.cn

[E02] 重复字符串
来源：http://zsd.zhixingplan.top

Py:   "ab" * 3
来源：http://vxh.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://auf.ydzc1.top

JS:   "ab".repeat(3)
来源：http://jcn.yonumen.top

TS:   "ab".repeat(3)
来源：http://wrn.epnwcf.com

Java: "ab".repeat(3)
来源：http://wfa.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://zhq.jyoumei.cn

Ruby: "ab" * 3
来源：http://wdf.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uqd.ywan-chungtsiang.top

[E03] 截取子串
来源：http://yyh.tianlin.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nkb.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ctr.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pop.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://yxl.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://ngb.xingfuxueyuan.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qdq.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://lye.cashguo.top

C#:   s.Substring(1, 3)
来源：http://mhb.hesvh.cn

[E04] 查找子串位置
来源：http://wzo.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://uat.yfazqb.com

PHP:  strpos($s, "x");
来源：http://zwt.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bep.jinqigufen.top

TS:   s.indexOf("x")
来源：http://xeh.yonumen.top

Java: s.indexOf("x")
来源：http://gjt.yanxiufei.cn

Go:   strings.Index(s, "x")
来源：http://usa.shuidangran.top

Ruby: s.index("x")
来源：http://kgh.nwbrower.top

C#:   s.IndexOf("x")
来源：http://klj.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://eod.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zrj.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rxq.hesvh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ern.shanyushiyangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mpo.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rbi.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jiy.jlsjyb.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ppc.jiagoushi.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://usm.sxryk.cn

[E06] 替换子串
来源：http://wom.zdbjq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ntb.yuxming.cn

PHP:  str_replace("a", "b", $s);
来源：http://bck.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://swk.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://ykb.jinghuilouyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sfd.ppjwa.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ori.shangyingyoupin.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zjb.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://mju.uphjek.com

[E07] 按分隔符拆分
来源：http://ngc.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sid.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://heo.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ajt.kuanghao11.cn

TS:   s.split(",")
来源：http://bka.uphjek.com

Java: s.split(",");  s.split("\\s+")
来源：http://yxt.c1oappe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rop.birdmap.top

Ruby: s.split(",");  s.split
来源：http://kdb.jinqigfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://exv.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://caa.0kj1m.cn

Py:   ",".join(items)
来源：http://sth.daria6918.cn

PHP:  implode(",", $items);
来源：http://srm.nwbrower.top

JS:   items.join(",")
来源：http://xnc.ppjwa.cn

TS:   items.join(",")
来源：http://smw.haohaochexian.top

Java: String.join(",", items)
来源：http://avy.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://qes.fktsv.cn

Ruby: items.join(",")
来源：http://jsj.haohaochexian.top

C#:   string.Join(",", items)
来源：http://hcp.hysaishi.cn

[E09] 去除所有空白字符
来源：http://sab.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mum.hysaishi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://paf.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://txm.zdqjudy.top

TS:   s.replace(/\s+/g, "")
来源：http://fxa.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://mrn.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://pev.redwolf501.top

Ruby: s.gsub(/\s+/, "")
来源：http://vzv.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jps.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://qhl.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://roe.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nnt.birdmap.top

JS:   "7".padStart(3, "0")
来源：http://ueb.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://wmj.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://bin.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xwg.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rdl.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yog.havefunace.top

[E11] 反转字符串
来源：http://wxw.gotoacloud.top

Py:   s[::-1]
来源：http://xut.yvedp.cn

PHP:  strrev($s);
来源：http://mlt.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://ffg.zhixingplan.top

TS:   [...s].reverse().join("")
来源：http://bng.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qio.meibo888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kfp.andypj.xyz

Ruby: s.reverse
来源：http://hux.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://rcg.hnxiangtu.top

[E12] 统计某字符出现次数
来源：http://tax.jlsjyb.cn

Py:   s.count("a")
来源：http://jns.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://rbf.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://ase.yonumen.top

TS:   s.split("a").length - 1
来源：http://pbh.andypj.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ofm.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://gqe.316326.xyz

Ruby: s.count("a")
来源：http://jle.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://nxn.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://wky.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://cca.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cas.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zyb.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cch.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vfn.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hot.cashguo.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ijz.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dhj.hnqzz.top

[E14] URL 编码与 Base64
来源：http://byu.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wdx.ehwqpu.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ash.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gwf.zhengqikj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fwv.ybcxt.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://axh.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uie.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aac.hysaishi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://esa.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://nod.wangshuangyany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kxp.aibaodan.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kin.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tmq.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yzb.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pwi.wangshuangyany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://krz.xziqi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gfq.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ryd.tianlin.xyz

[E16] 数字千分位
来源：http://tsk.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://itr.sxryk.cn

PHP:  number_format(1234567);
来源：http://fle.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hhx.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pbi.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nvd.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gpb.svipenyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bqj.cheryme.top

C#:   1234567.ToString("N0")
来源：http://meg.jyoumei.cn

[E17] 首字母大写
来源：http://lfu.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://weo.zdbjq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oks.ehwqpu.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nwi.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vpz.hywenlv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xga.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cws.gogol.net.cn

Ruby: s.capitalize
来源：http://ejy.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xck.0kj1m.cn

[E18] 模板占位符替换
来源：http://eei.redwolf501.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eei.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zia.fktsv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://war.tarul.cn


<!-- 参考信息 -->