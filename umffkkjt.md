代发 wailian999

[D11] 反转数组
来源：http://qzq.jlsjyb.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wqn.fengsongda.top

PHP:  array_reverse($arr);
来源：http://ujd.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bpy.birdmap.top

TS:   [...arr].reverse();
来源：http://qbq.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://prt.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://jlb.quarkkingdee.top

Ruby: arr.reverse
来源：http://vxq.ydjk.org.cn

C#:   list.Reverse();
来源：http://sfl.aizwys.cn

[D12] 查找元素下标
来源：http://yqs.0kj1m.cn

Py:   arr.index(x);  x in arr
来源：http://dcb.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hcu.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wre.iojbl.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rxj.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rag.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://flb.9152youxi.cn

Ruby: arr.index(x)
来源：http://rwu.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://mbk.jinghuilouyu.cn

[D13] 过滤（保留满足条件的）
来源：http://etk.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mme.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nha.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://vfr.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://kui.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bie.zhengqikj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://njw.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zis.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pvj.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://xeo.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zhh.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gpo.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://mpj.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://uad.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tnw.zhongyouzk.top

Go:   // 手写循环
来源：http://iam.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://yuo.shzxlz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hhy.xingfuxueyuan.xyz

[D15] 去重
来源：http://wcc.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lyh.cdnleiting.top

PHP:  array_unique($arr);
来源：http://prr.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://ydv.xziqi.cn

TS:   [...new Set(arr)]
来源：http://kqu.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xjs.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://qgi.yvedp.cn

Ruby: arr.uniq
来源：http://ety.hnxiangtu.top

C#:   list.Distinct().ToList()
来源：http://jxt.shuidangran.top

[D16] 求和与平均值
来源：http://ifo.guowangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nyo.gogol.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eyf.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dqb.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ugd.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://urp.yvedp.cn

Go:   // 手写循环累加
来源：http://tka.zhoulong.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hpm.hnxiangtu.top

C#:   list.Sum();  list.Average()
来源：http://won.sysykeji.top

[D17] 最大值与最小值
来源：http://qdo.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://fno.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://ufl.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://out.yonumen.top

TS:   Math.max(...arr);
来源：http://tmm.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jxc.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://afh.havefunace.top

Ruby: arr.max;  arr.min
来源：http://dja.yj20258.top

C#:   list.Max();  list.Min()
来源：http://iqc.ydzc1.top

[D18] 扁平化嵌套数组
来源：http://xho.dashuyun.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oxm.havefunace.top

PHP:  array_merge(...$nested);
来源：http://opf.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sjs.ehwqpu.com

TS:   nested.flat();
来源：http://lvw.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ssy.chenlongwang.top

Go:   // 手写双层循环
来源：http://fps.hongshengwenyu.top

Ruby: nested.flatten
来源：http://jrj.wangshuangyany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pkt.yvedp.cn

[D19] 按字段分组
来源：http://rxo.fktsv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://obm.c1oappe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://snu.9152youxi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gfw.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zrd.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kgc.uphjek.com

Go:   // 手写 map[string][]T
来源：http://rst.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://snc.havefunace.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.birdmap.top

[D20] 统计每个元素出现次数
来源：http://bpp.pycfn.com

Py:   Counter(arr)
来源：http://uqs.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://mnd.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zyq.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ooq.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rda.shangyingyoupin.top

Go:   // 手写 map[T]int
来源：http://afj.quarkkingdee.top

Ruby: arr.tally
来源：http://jny.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://znz.yonumen.top

[D21] 判断是否包含某元素
来源：http://czq.9152youxi.cn

Py:   x in arr
来源：http://uge.hcnkem.com

PHP:  in_array($x, $arr, true);
来源：http://dkd.yanxiufei.cn

JS:   arr.includes(x)
来源：http://eus.fehbvm.com

TS:   arr.includes(x)
来源：http://lzx.dashuyun.cn

Java: list.contains(x)
来源：http://yas.dashuyun.cn

Go:   slices.Contains(arr, x)
来源：http://ojp.xingfuxueyuan.xyz

Ruby: arr.include?(x)
来源：http://yjc.cqqwz.cn

C#:   list.Contains(x)
来源：http://nic.daria6918.cn

[D22] 复制数组（避免共享引用）
来源：http://xqd.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cch.redwolf501.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://utf.tianlin.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://syg.zhaomingkeji.xyz

TS:   [...arr];
来源：http://nef.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://uiu.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://hqj.xingfuxueyuan.xyz

Ruby: arr.dup;  arr.clone
来源：http://whp.cucudq.cn

C#:   new List<int>(list);
来源：http://osw.chenzaomai.com

[D23] reduce 累积计算
来源：http://ydo.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vls.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qei.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wqi.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dnp.ehwqpu.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://qbb.daxiang520.top

Go:   // 手写循环
来源：http://xtw.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nfy.zdqjudy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://soa.jinghuilouyu.cn

[D24] 字典 / Map 基本操作
来源：http://vuq.ppjwa.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kis.fehbvm.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://arn.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ino.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://slm.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hqw.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://byb.yueranfly.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rvp.ivvv.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wfw.cheryme.top

[D25] Set 集合去重与交并差
来源：http://iko.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eao.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://imy.yj202588.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hvy.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xfp.ydjk.org.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://htm.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hwv.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sbc.9152youxi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xjz.guannengcc.top

[D26] 数组转字符串
来源：http://snz.cheryme.top

Py:   ", ".join(map(str, arr))
来源：http://oix.cheryme.top

PHP:  implode(", ", $arr);
来源：http://dcl.andypj.xyz

JS:   arr.join(", ")
来源：http://ypr.hammf.cn

TS:   arr.join(", ")
来源：http://pcj.ppjwa.cn

Java: String.join(", ", list)
来源：http://gbc.mhx1999.top

Go:   strings.Join(strs, ", ")
来源：http://kmo.cashguo.top

Ruby: arr.join(", ")
来源：http://ixk.jinyuanbaomall.cn

C#:   string.Join(", ", list)
来源：http://ymb.shanyushiyangtech.top

================================================================================
来源：http://jju.guowangkeji.top

E. 字符串处理
来源：http://rnz.yj20258.top

================================================================================
来源：http://wbi.wangshuangyany.cn

[E01] 拼接字符串
来源：http://nnp.dashuyun.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uns.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vmc.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wlf.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ytp.tian-w.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qzz.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jba.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://guq.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ohw.svipenyu.cn

[E02] 重复字符串
来源：http://roe.cqqwz.cn

Py:   "ab" * 3
来源：http://njy.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://bbw.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://rrx.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://ewg.zycfv.cn

Java: "ab".repeat(3)
来源：http://swx.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://uox.guowangkeji.top

Ruby: "ab" * 3
来源：http://sqw.wangshuangyany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://btc.shuidangran.top

[E03] 截取子串
来源：http://ojv.tian-w.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pjk.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rmy.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nap.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://bup.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://aib.daxiang520.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://scu.gotoacloud.top

Ruby: s[1, 3];  s[1..3]
来源：http://jun.yuxming.cn

C#:   s.Substring(1, 3)
来源：http://yut.ydzc1.top

[E04] 查找子串位置
来源：http://ghr.hysaishi.cn

Py:   s.find("x");  s.index("x")
来源：http://lwc.pengpengdd.cyou

PHP:  strpos($s, "x");
来源：http://vxm.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jir.yvedp.cn

TS:   s.indexOf("x")
来源：http://shd.daxiang520.top

Java: s.indexOf("x")
来源：http://sfr.hcnkem.com

Go:   strings.Index(s, "x")
来源：http://vxv.zhijiandao.cn

Ruby: s.index("x")
来源：http://mbb.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://ilm.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://ozk.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jsc.sxryk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hsa.xylfe.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kwb.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tlf.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jxj.nanxinkj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wkn.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oqn.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fxi.ctjpmb.com

[E06] 替换子串
来源：http://osm.cucudq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pgf.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://mxj.aibaodan.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iky.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://cph.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mco.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kgu.chenzaomai.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://knk.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://mxk.nanxinkj.top

[E07] 按分隔符拆分
来源：http://ber.wangdashe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://quj.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://add.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uob.ppjwa.cn

TS:   s.split(",")
来源：http://emk.pycfn.com

Java: s.split(",");  s.split("\\s+")
来源：http://auw.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bkz.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://maq.fktsv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jqj.svipenyu.cn

[E08] 数组按分隔符合并
来源：http://muz.ppjwa.cn

Py:   ",".join(items)
来源：http://yil.jinghuilouyu.cn

PHP:  implode(",", $items);
来源：http://hka.quarkkingdee.top

JS:   items.join(",")
来源：http://qpn.nanxinkj.top

TS:   items.join(",")
来源：http://obe.shuidangran.top

Java: String.join(",", items)
来源：http://zjr.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://vgd.smart0.xyz

Ruby: items.join(",")
来源：http://ynp.9152youxi.cn

C#:   string.Join(",", items)
来源：http://rpo.zdbjq.cn

[E09] 去除所有空白字符
来源：http://fzr.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kfh.zhijiandao.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://txp.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://ibs.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://tsq.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://wle.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://lfq.fengsongda.top

Ruby: s.gsub(/\s+/, "")
来源：http://nrq.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ofs.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://row.yuxming.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xzt.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rpo.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://eug.xuanzx.com

TS:   "7".padStart(3, "0")
来源：http://qhw.bbcook.cn

Java: String.format("%03d", 7)
来源：http://mqn.chenlongwang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://owb.hysaishi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ldw.quarkkingdee.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://llb.hongshengwenyu.top

[E11] 反转字符串
来源：http://hqj.svipenyu.cn

Py:   s[::-1]
来源：http://yfz.ppjwa.cn

PHP:  strrev($s);
来源：http://iow.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://vlw.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://zqa.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ytd.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vtm.ybcxt.top

Ruby: s.reverse
来源：http://ksi.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://bso.pycfn.com

[E12] 统计某字符出现次数
来源：http://zfr.haohaochexian.top

Py:   s.count("a")
来源：http://vnd.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://jln.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://znt.cucudq.cn

TS:   s.split("a").length - 1
来源：http://bzz.sysykeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hdw.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://tmi.c1oappe.top

Ruby: s.count("a")
来源：http://uhw.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://nnx.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://xjk.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://apd.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ejk.cqqwz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cok.yanxiufei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mes.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rpu.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wnx.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uss.yj20258888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gnj.ybcxt.top

[E14] URL 编码与 Base64
来源：http://lmh.chenlongwang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lbq.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fqo.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://clr.sjlbkw.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kpm.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://adj.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tbu.zhiwuduotai.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qlm.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wcp.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://mad.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nac.chenjidiqi.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bdp.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uag.xuanzx.com

TS:   // 同上，务必做 XSS 过滤
来源：http://pwy.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qpf.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://upf.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nxp.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://elj.316326.xyz

[E16] 数字千分位
来源：http://aqn.cdnleiting.top

Py:   f"{1234567:,}"
来源：http://ygt.iojbl.cn

PHP:  number_format(1234567);
来源：http://odm.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zeu.bjfxy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://smh.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dqo.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pnl.hesvh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jvt.yuanzhike.top

C#:   1234567.ToString("N0")
来源：http://hrq.zhoulong.xyz

[E17] 首字母大写
来源：http://nph.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nah.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://zmf.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nul.vehdjk.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hzz.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://glh.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rbu.redwolf501.top

Ruby: s.capitalize
来源：http://nbn.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rwi.9152youxi.cn


<!-- 参考信息 -->