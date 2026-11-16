代发 wailian999

C#:   list.Reverse();
来源：http://cgt.sufxvd.cn

[D12] 查找元素下标
来源：http://hfd.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://waj.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ucg.fanxiaobao.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uaa.sysykeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hxr.sxryk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dfk.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://gnf.aibaodan.cn

Ruby: arr.index(x)
来源：http://xlt.yonumen.top

C#:   list.IndexOf(x);
来源：http://igm.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://dzg.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lho.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eid.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://wls.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://qqc.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xyu.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qff.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gpw.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://myi.jqgfzy.top

[D14] 映射转换（每个元素变形）
来源：http://mhw.aibaodan.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ntx.shanyushiyangtech.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hxp.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://mgo.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://shg.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kes.yuanzhike.top

Go:   // 手写循环
来源：http://buw.tanke756.top

Ruby: arr.map { |x| x * 2 }
来源：http://nmg.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kyh.fanxiaobao.xyz

[D15] 去重
来源：http://kjw.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jwe.xuanzx.com

PHP:  array_unique($arr);
来源：http://hlh.316326.xyz

JS:   [...new Set(arr)]
来源：http://ovy.cashguo.top

TS:   [...new Set(arr)]
来源：http://mbt.wangshuangyany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cxb.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://upt.dashuyun.cn

Ruby: arr.uniq
来源：http://yhu.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://ocq.zdqjudy.top

[D16] 求和与平均值
来源：http://jdn.ydzc1.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mwh.guowangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mgf.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xmc.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cyb.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://khk.hesvh.cn

Go:   // 手写循环累加
来源：http://iap.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://trg.cashguo.top

C#:   list.Sum();  list.Average()
来源：http://wgd.sxryk.cn

[D17] 最大值与最小值
来源：http://oju.tanke756.top

Py:   max(arr);  min(arr)
来源：http://jhf.iojbl.cn

PHP:  max($arr);  min($arr);
来源：http://xlg.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://obg.zdbjq.cn

TS:   Math.max(...arr);
来源：http://uaz.yongpay.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ryx.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://owa.52xcode.cn

Ruby: arr.max;  arr.min
来源：http://ajg.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://nwd.zhongyouzk.top

[D18] 扁平化嵌套数组
来源：http://crr.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wmk.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://jtr.shangyingyoupin.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://phs.dianchejie.cn

TS:   nested.flat();
来源：http://rre.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pqk.daxiang520.top

Go:   // 手写双层循环
来源：http://ogr.yuxming.cn

Ruby: nested.flatten
来源：http://ohq.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uxc.hnxiangtu.top

[D19] 按字段分组
来源：http://dnj.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cjc.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rza.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vvv.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pid.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bfi.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://kqs.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fhf.gaohongyu789.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dmn.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://okd.hfpthk.cn

Py:   Counter(arr)
来源：http://kbo.ydjk.org.cn

PHP:  array_count_values($arr);
来源：http://nyf.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ugz.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://htt.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qco.yj20258.top

Go:   // 手写 map[T]int
来源：http://kks.tian-w.cn

Ruby: arr.tally
来源：http://sbf.ywan-chungtsiang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ksf.cashguo.top

[D21] 判断是否包含某元素
来源：http://jlx.ybcxt.top

Py:   x in arr
来源：http://cre.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://otz.cdnleiting.top

JS:   arr.includes(x)
来源：http://eqd.feifeiyinyue.top

TS:   arr.includes(x)
来源：http://vfv.gogol.net.cn

Java: list.contains(x)
来源：http://fgp.chenlongwang.top

Go:   slices.Contains(arr, x)
来源：http://vhq.tanke756.top

Ruby: arr.include?(x)
来源：http://xch.haohaochexian.top

C#:   list.Contains(x)
来源：http://yqe.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://xxa.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wes.zhongyouzk.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fnu.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nym.ctjpmb.com

TS:   [...arr];
来源：http://jct.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://uta.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://voq.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://baj.chenzaomai.com

C#:   new List<int>(list);
来源：http://qfy.redwolf501.top

[D23] reduce 累积计算
来源：http://lti.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ckt.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kxz.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pag.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bvv.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://iyd.yongpay.top

Go:   // 手写循环
来源：http://ptq.jqgfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dxk.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qtr.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://cio.ydzc1.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cir.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gws.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tfe.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aqj.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rjj.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://abc.redwolf501.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cgc.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://foq.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://hei.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jhc.aibaodan.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qkm.mhx1999.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mlt.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tej.nanxinkj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iry.guannengcc.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wla.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wou.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tat.jinqigfzy.top

[D26] 数组转字符串
来源：http://bhi.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://wou.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://ynx.svipenyu.cn

JS:   arr.join(", ")
来源：http://iib.zycfv.cn

TS:   arr.join(", ")
来源：http://ogl.sweek.top

Java: String.join(", ", list)
来源：http://kut.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://cci.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://kqb.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://toh.ivvv.top

================================================================================
来源：http://ybd.sufxvd.cn

E. 字符串处理
来源：http://ros.jlsjyb.cn

================================================================================
来源：http://lfy.xuetiantiany.cn

[E01] 拼接字符串
来源：http://pls.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://equ.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jvz.hongshengwenyu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nvr.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ajo.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://okh.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gdh.zycfv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cvz.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xit.jiagoushi.top

[E02] 重复字符串
来源：http://jqz.cashguo.top

Py:   "ab" * 3
来源：http://xle.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://aye.sysykeji.top

JS:   "ab".repeat(3)
来源：http://wnx.hcnkem.com

TS:   "ab".repeat(3)
来源：http://ovf.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://opl.pycfn.com

Go:   strings.Repeat("ab", 3)
来源：http://enu.zhixingplan.top

Ruby: "ab" * 3
来源：http://ipi.fktsv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xza.hammf.cn

[E03] 截取子串
来源：http://cbe.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pfm.tianlin.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mjx.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://moj.cdnleiting.top

TS:   s.slice(1, 4)
来源：http://uzh.sysykeji.top

Java: s.substring(1, 4)
来源：http://pyj.jinqigufen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gsk.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://lrg.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://vwr.chenjidiqi.icu

[E04] 查找子串位置
来源：http://nes.jinqigufen.top

Py:   s.find("x");  s.index("x")
来源：http://uxl.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://xen.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tef.gogol.net.cn

TS:   s.indexOf("x")
来源：http://etf.gzhubu.top

Java: s.indexOf("x")
来源：http://zah.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://vqv.smart0.xyz

Ruby: s.index("x")
来源：http://lwe.yj20258.top

C#:   s.IndexOf("x")
来源：http://hcv.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yjx.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vvc.tian-w.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://giw.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qdv.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://nny.aibaodan.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vab.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dof.hnqzz.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sgw.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zxq.shanyushiyangkeji.top

[E06] 替换子串
来源：http://pvg.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lea.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://kxs.ydjk.org.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://crj.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://kyy.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zsx.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zgb.xylfe.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hjb.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://kog.havefunace.top

[E07] 按分隔符拆分
来源：http://glg.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lmb.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iwf.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cvr.yueranfly.top

TS:   s.split(",")
来源：http://dez.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://nyi.meibo888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yqd.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://ruo.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ysa.uphjek.com

[E08] 数组按分隔符合并
来源：http://mnz.shzxlz.cn

Py:   ",".join(items)
来源：http://hhn.0kj1m.cn

PHP:  implode(",", $items);
来源：http://fhw.xingfuxueyuan.xyz

JS:   items.join(",")
来源：http://xvt.epnwcf.com

TS:   items.join(",")
来源：http://vxk.mhx1999.top

Java: String.join(",", items)
来源：http://qqa.yonumen.top

Go:   strings.Join(items, ",")
来源：http://ooc.zycfv.cn

Ruby: items.join(",")
来源：http://jew.yuxming.cn

C#:   string.Join(",", items)
来源：http://lro.jqgfzy.top

[E09] 去除所有空白字符
来源：http://rvt.c1oappe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sju.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hft.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://pff.yongpay.top

TS:   s.replace(/\s+/g, "")
来源：http://ssl.ctjpmb.com

Java: s.replaceAll("\\s+", "")
来源：http://skl.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lcs.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zkz.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nxy.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://zuo.yj20258888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bfn.jinyuanbaomall.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pry.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://wjf.hammf.cn

TS:   "7".padStart(3, "0")
来源：http://nuj.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://mfb.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vvq.fanxiaobao.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zoq.yj20258.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bbg.fktsv.cn

[E11] 反转字符串
来源：http://imi.shzxlz.cn

Py:   s[::-1]
来源：http://ilz.fanxiaobao.xyz

PHP:  strrev($s);
来源：http://pnr.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://qmx.ydzc1.top

TS:   [...s].reverse().join("")
来源：http://khf.yj202588.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jht.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mim.fktsv.cn

Ruby: s.reverse
来源：http://qoa.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://smt.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://zli.gotoacloud.top

Py:   s.count("a")
来源：http://ejs.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://pdr.52xcode.cn

JS:   s.split("a").length - 1
来源：http://gbd.yongpay.top

TS:   s.split("a").length - 1
来源：http://frz.fanxiaobao.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gva.hongshengwenyu.top

Go:   strings.Count(s, "a")
来源：http://dwq.bbcook.cn

Ruby: s.count("a")
来源：http://lgi.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://xsf.jqgfzy.top

[E13] 逐字符遍历
来源：http://oiv.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://hgh.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zev.nwbrower.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vbq.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kow.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fro.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wov.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://ikq.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xlh.fktsv.cn

[E14] URL 编码与 Base64
来源：http://dnv.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hcl.ybcxt.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://euh.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sra.yanxiufei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nrq.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hyf.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zot.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uxs.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lbh.yongpay.top

[E15] HTML 转义 / 反转义
来源：http://axr.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://bom.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tog.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://urz.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cqt.yueranfly.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tat.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tde.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jxf.hysaishi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fnt.chenlongwang.top

[E16] 数字千分位
来源：http://ogn.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://thr.nwbrower.top

PHP:  number_format(1234567);
来源：http://iho.dashuyun.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oxa.yuanzhike.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ykc.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iju.birdmap.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dqz.gaohongyu789.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vyu.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://utq.havefunace.top

[E17] 首字母大写
来源：http://lvx.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wam.yonumen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cck.wangdashe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://loa.chenzaomai.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qeq.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hmq.fengsongda.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://snm.havefunace.top

Ruby: s.capitalize
来源：http://dhn.jinqigfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jhc.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://wfa.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sca.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nnx.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tyc.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xwg.aibaodan.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vlq.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sqn.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://svo.shanyushiyangtech.top


<!-- 参考信息 -->