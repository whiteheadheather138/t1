代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hqu.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fsq.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kbb.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ifm.shzxlz.cn

[D11] 反转数组
来源：http://ydt.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://msp.havefunace.top

PHP:  array_reverse($arr);
来源：http://zip.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ome.cqqwz.cn

TS:   [...arr].reverse();
来源：http://ggc.ehwqpu.com

Java: Collections.reverse(list);
来源：http://mlq.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://hku.ehwqpu.com

Ruby: arr.reverse
来源：http://wnh.fehbvm.com

C#:   list.Reverse();
来源：http://unf.ehwqpu.com

[D12] 查找元素下标
来源：http://fkp.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://rns.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://umf.zhengqikj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xyt.zhengqikj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xgb.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qzb.cucudq.cn

Go:   slices.Index(arr, x)
来源：http://icz.cucudq.cn

Ruby: arr.index(x)
来源：http://rqw.yvedp.cn

C#:   list.IndexOf(x);
来源：http://xiq.daxiang520.top

[D13] 过滤（保留满足条件的）
来源：http://snt.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rtw.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://asv.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://osb.andypj.xyz

TS:   arr.filter(x => x > 3)
来源：http://cuv.tian-w.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nxj.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cnn.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://kpa.xylfe.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mzk.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://sou.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qya.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kgj.tanke756.top

JS:   arr.map(x => x * 2)
来源：http://xvp.hywenlv.cn

TS:   arr.map(x => x * 2)
来源：http://orw.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://oxn.cucudq.cn

Go:   // 手写循环
来源：http://nwe.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://tpp.cucudq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sjg.tanke756.top

[D15] 去重
来源：http://dfw.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xqa.zycfv.cn

PHP:  array_unique($arr);
来源：http://lou.shzxlz.cn

JS:   [...new Set(arr)]
来源：http://zhz.fktsv.cn

TS:   [...new Set(arr)]
来源：http://rrb.svipenyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pcl.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zme.pengpengdd.cyou

Ruby: arr.uniq
来源：http://fhz.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://wzf.zhoulong.xyz

[D16] 求和与平均值
来源：http://saw.ywan-chungtsiang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jru.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://liu.wangshuangyany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xpc.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bej.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kqz.hcnkem.com

Go:   // 手写循环累加
来源：http://xlp.9152youxi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qlm.xingfuxueyuan.xyz

C#:   list.Sum();  list.Average()
来源：http://hcd.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://fcp.jinghuilouyu.cn

Py:   max(arr);  min(arr)
来源：http://pfu.yuxming.cn

PHP:  max($arr);  min($arr);
来源：http://kjy.sysykeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ydf.cqqwz.cn

TS:   Math.max(...arr);
来源：http://ntd.hesvh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ggg.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://stx.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://uze.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://kqa.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://quo.yj20258888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pmv.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://efx.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bkb.vqdsnc.cn

TS:   nested.flat();
来源：http://lgz.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vad.yj202588.top

Go:   // 手写双层循环
来源：http://top.tianlin.xyz

Ruby: nested.flatten
来源：http://xun.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gxa.chenzaomai.com

[D19] 按字段分组
来源：http://ekg.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://joy.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mkd.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tuf.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://aks.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jfe.ppjwa.cn

Go:   // 手写 map[string][]T
来源：http://pya.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lnz.haohaochexian.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jjb.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://oru.meibo888.top

Py:   Counter(arr)
来源：http://xrb.cashguo.top

PHP:  array_count_values($arr);
来源：http://bxf.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://msm.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cui.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vbo.hammf.cn

Go:   // 手写 map[T]int
来源：http://xpt.jqgufenzy.top

Ruby: arr.tally
来源：http://zuj.zdbjq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ouc.smart0.xyz

[D21] 判断是否包含某元素
来源：http://imf.chenjidiqi.icu

Py:   x in arr
来源：http://zae.hywenlv.cn

PHP:  in_array($x, $arr, true);
来源：http://myv.epnwcf.com

JS:   arr.includes(x)
来源：http://wao.jqgfzy.top

TS:   arr.includes(x)
来源：http://lfd.redwolf501.top

Java: list.contains(x)
来源：http://lvo.bjfxy.top

Go:   slices.Contains(arr, x)
来源：http://fte.tarul.cn

Ruby: arr.include?(x)
来源：http://xts.xingfuxueyuan.xyz

C#:   list.Contains(x)
来源：http://nbr.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://vre.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sxg.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gen.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uzh.hywenlv.cn

TS:   [...arr];
来源：http://imm.yonumen.top

Java: new ArrayList<>(list);
来源：http://jgm.ppjwa.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bup.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://rsl.shuidangran.top

C#:   new List<int>(list);
来源：http://qdj.redwolf501.top

[D23] reduce 累积计算
来源：http://umc.jyoumei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rop.dashuyun.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xzv.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jll.jinghuilouyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vgd.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kgl.iojbl.cn

Go:   // 手写循环
来源：http://cwk.yj20258.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hxo.nanxuanxn.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cuo.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://asw.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jup.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sjw.pycfn.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jlb.zhijiandao.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nkj.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cij.chenlongwang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hom.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cia.redwolf501.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zkh.hysaishi.cn

[D25] Set 集合去重与交并差
来源：http://wzp.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xaf.vehdjk.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kcg.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vkc.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cbh.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vad.yonumen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qgr.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qon.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lic.sufxvd.cn

[D26] 数组转字符串
来源：http://odb.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://hji.sweek.top

PHP:  implode(", ", $arr);
来源：http://vkq.9152youxi.cn

JS:   arr.join(", ")
来源：http://wwe.hysaishi.cn

TS:   arr.join(", ")
来源：http://qfy.nanxuanxn.top

Java: String.join(", ", list)
来源：http://ioz.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://bkf.zhengqikj.top

Ruby: arr.join(", ")
来源：http://ngk.yonumen.top

C#:   string.Join(", ", list)
来源：http://acj.daria6918.cn

================================================================================
来源：http://bjo.dianchejie.cn

E. 字符串处理
来源：http://dvn.dianchejie.cn

================================================================================
来源：http://sbv.yonumen.top

[E01] 拼接字符串
来源：http://apo.sxryk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fsc.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ifn.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ona.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eew.sysykeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kry.hywenlv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ofy.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nte.pycfn.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://osp.meibo888.top

[E02] 重复字符串
来源：http://jny.ivvv.top

Py:   "ab" * 3
来源：http://rwn.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://hhh.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://cbd.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://bod.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://tiu.zycfv.cn

Go:   strings.Repeat("ab", 3)
来源：http://jcs.xylfe.cn

Ruby: "ab" * 3
来源：http://ieg.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://car.vqdsnc.cn

[E03] 截取子串
来源：http://lhw.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zcv.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tlv.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xjg.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://qvc.sweek.top

Java: s.substring(1, 4)
来源：http://qtq.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zje.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://gne.jianghu66.top

[E04] 查找子串位置
来源：http://ylk.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://rua.c1oappe.top

PHP:  strpos($s, "x");
来源：http://qcr.yanxiufei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qsd.yfazqb.com

TS:   s.indexOf("x")
来源：http://twp.jlsjyb.cn

Java: s.indexOf("x")
来源：http://lqp.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://caw.dianchejie.cn

Ruby: s.index("x")
来源：http://ess.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://bgs.cqqwz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://anh.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lcy.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ttg.cucudq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://evi.snrcjt.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://myu.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hgh.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aci.quarkkingdee.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rzm.daxiang520.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vej.guannengcc.top

[E06] 替换子串
来源：http://you.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iuv.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://bon.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ztj.chenjidiqi.icu

TS:   s.replaceAll("a", "b")
来源：http://pdf.yuxming.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mro.zhijiandao.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://avf.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uyv.zhengqikj.top

C#:   s.Replace("a", "b")
来源：http://vzo.ehwqpu.com

[E07] 按分隔符拆分
来源：http://lxh.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://txx.xuetiantiany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pte.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://hcn.tanke756.top

TS:   s.split(",")
来源：http://lfk.ywan-chungtsiang.top

Java: s.split(",");  s.split("\\s+")
来源：http://dxk.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ywp.jinqigufen.top

Ruby: s.split(",");  s.split
来源：http://kop.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ile.tian-w.cn

[E08] 数组按分隔符合并
来源：http://kjs.chenzaomai.com

Py:   ",".join(items)
来源：http://mft.jinghuilouyu.cn

PHP:  implode(",", $items);
来源：http://yat.fengsongda.top

JS:   items.join(",")
来源：http://aug.hysaishi.cn

TS:   items.join(",")
来源：http://nvl.guowangkeji.top

Java: String.join(",", items)
来源：http://usa.yanxiufei.cn

Go:   strings.Join(items, ",")
来源：http://wai.snrcjt.cn

Ruby: items.join(",")
来源：http://bnp.bjfxy.top

C#:   string.Join(",", items)
来源：http://jei.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://atf.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vbl.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vsh.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://njx.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://wqr.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://ujq.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vxb.316326.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://yen.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://osr.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://uvr.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fxx.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ybw.quarkkingdee.top

JS:   "7".padStart(3, "0")
来源：http://gsv.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://lbp.fehbvm.com

Java: String.format("%03d", 7)
来源：http://qpg.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://foh.hysaishi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dhj.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zjm.shanyushiyangkeji.top

[E11] 反转字符串
来源：http://zuq.fktsv.cn

Py:   s[::-1]
来源：http://xcp.sweek.top

PHP:  strrev($s);
来源：http://shl.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://skg.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://yds.yuanzhike.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ldb.cucudq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eyb.zhengqikj.top

Ruby: s.reverse
来源：http://wxn.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://cbu.havefunace.top

[E12] 统计某字符出现次数
来源：http://nmk.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://xqg.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://fat.vehdjk.com

JS:   s.split("a").length - 1
来源：http://kfg.meibo888.top

TS:   s.split("a").length - 1
来源：http://tzf.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ozl.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://idt.ppjwa.cn

Ruby: s.count("a")
来源：http://kfb.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://uyg.vqdsnc.cn

[E13] 逐字符遍历
来源：http://ldt.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://ygh.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rsy.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ubr.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://phs.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gsx.hesvh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rsz.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wic.hammf.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gri.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://zeh.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pwv.shuidangran.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yay.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://osr.jqgfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kll.nanxinkj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vgo.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hoy.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xes.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eqi.shuidangran.top

[E15] HTML 转义 / 反转义
来源：http://doo.haohaochexian.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cyt.yfazqb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nak.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nzx.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zsa.sufxvd.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://unk.yj202588.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://asj.xingfuxueyuan.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nwa.cheryme.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jad.dianchejie.cn

[E16] 数字千分位
来源：http://npi.sysykeji.top

Py:   f"{1234567:,}"
来源：http://ssr.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://hhy.jianghu66.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xua.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://esf.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qvz.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://afx.yj20258.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ogs.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://gkn.xylfe.cn

[E17] 首字母大写
来源：http://gch.sysykeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zit.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ike.nanxuanxn.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sja.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mwe.sweek.top


<!-- 参考信息 -->