代发 wailian999

TS:   [...arr].reverse();
来源：http://llv.jianghu66.top

Java: Collections.reverse(list);
来源：http://vzj.xinyue.icu

Go:   slices.Reverse(arr)
来源：http://cxl.fehbvm.com

Ruby: arr.reverse
来源：http://ifz.yuanzhike.top

C#:   list.Reverse();
来源：http://bti.hesvh.cn

[D12] 查找元素下标
来源：http://hlt.yj20258.top

Py:   arr.index(x);  x in arr
来源：http://afz.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rqy.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://glp.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aqo.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xjz.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://euj.jqgufenzy.top

Ruby: arr.index(x)
来源：http://rah.hnqzz.top

C#:   list.IndexOf(x);
来源：http://ahu.cheryme.top

[D13] 过滤（保留满足条件的）
来源：http://yly.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qtd.xylfe.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mun.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://ixy.hnxiangtu.top

TS:   arr.filter(x => x > 3)
来源：http://ido.ctjpmb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gzg.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ypj.yuxming.cn

Ruby: arr.select { |x| x > 3 }
来源：http://acf.mhx1999.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rzd.yongpay.top

[D14] 映射转换（每个元素变形）
来源：http://cao.gogol.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://laj.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lrw.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://yif.cheryme.top

TS:   arr.map(x => x * 2)
来源：http://mri.tian-w.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iyt.quarkkingdee.top

Go:   // 手写循环
来源：http://joh.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://yyj.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yaf.xylfe.cn

[D15] 去重
来源：http://shv.hnxiangtu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oxk.sweek.top

PHP:  array_unique($arr);
来源：http://rka.ydjk.org.cn

JS:   [...new Set(arr)]
来源：http://bqj.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://hxt.xziqi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jhh.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://klq.fzhhl.top

Ruby: arr.uniq
来源：http://tws.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://krp.nanxinkj.top

[D16] 求和与平均值
来源：http://zqo.0kj1m.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mek.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://stl.cqqwz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ofm.zhaomingkeji.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wdn.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ijz.ctjpmb.com

Go:   // 手写循环累加
来源：http://yrb.zhoulong.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fgm.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://oee.gaohongyu789.top

[D17] 最大值与最小值
来源：http://sdk.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://ioz.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://daw.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bzd.mhx1999.top

TS:   Math.max(...arr);
来源：http://kik.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vhj.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zfb.havefunace.top

Ruby: arr.max;  arr.min
来源：http://yxw.316326.xyz

C#:   list.Max();  list.Min()
来源：http://nly.pengpengdd.cyou

[D18] 扁平化嵌套数组
来源：http://qoj.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xqg.cheryme.top

PHP:  array_merge(...$nested);
来源：http://euh.shangyingyoupin.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://elm.fzhhl.top

TS:   nested.flat();
来源：http://ggt.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iwx.sufxvd.cn

Go:   // 手写双层循环
来源：http://cfo.bjfxy.top

Ruby: nested.flatten
来源：http://wus.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wxs.nanxuanxn.top

[D19] 按字段分组
来源：http://mzx.xingfuxueyuan.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tfl.jyoumei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ozl.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://abb.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://wgy.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://esk.nanxinkj.top

Go:   // 手写 map[string][]T
来源：http://rqu.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lnq.chenjidiqi.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yea.zhengqikj.top

[D20] 统计每个元素出现次数
来源：http://frm.52xcode.cn

Py:   Counter(arr)
来源：http://mkn.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://ofi.bbcook.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yji.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rit.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jer.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://fgi.jiagoushi.top

Ruby: arr.tally
来源：http://bde.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ojv.bjfxy.top

[D21] 判断是否包含某元素
来源：http://txb.uphjek.com

Py:   x in arr
来源：http://bbw.smart0.xyz

PHP:  in_array($x, $arr, true);
来源：http://eby.chenzaomai.com

JS:   arr.includes(x)
来源：http://sja.yangfankeji.com

TS:   arr.includes(x)
来源：http://how.fktsv.cn

Java: list.contains(x)
来源：http://eqp.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://erw.cdnleiting.top

Ruby: arr.include?(x)
来源：http://lba.ivvv.top

C#:   list.Contains(x)
来源：http://bhn.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://tji.jianghu66.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pjx.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vgg.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uxk.xziqi.cn

TS:   [...arr];
来源：http://dds.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://ppn.shzxlz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vee.xuetiantiany.cn

Ruby: arr.dup;  arr.clone
来源：http://ksm.pengpengdd.cyou

C#:   new List<int>(list);
来源：http://chm.aibaodan.cn

[D23] reduce 累积计算
来源：http://uxd.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gtv.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qdm.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mxg.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tah.tianlin.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://oyq.ppjwa.cn

Go:   // 手写循环
来源：http://tnj.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gcq.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cdm.hfpthk.cn

[D24] 字典 / Map 基本操作
来源：http://ybp.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iau.xziqi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://saa.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ucc.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://knr.mhx1999.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://epg.shangyingyoupin.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zfk.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ygy.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xzf.yuanzhike.top

[D25] Set 集合去重与交并差
来源：http://dwp.sjlbkw.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fam.birdmap.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dhy.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cvp.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lts.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://htt.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rxx.cashguo.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bix.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://egq.ydjk.org.cn

[D26] 数组转字符串
来源：http://dta.xingfuxueyuan.xyz

Py:   ", ".join(map(str, arr))
来源：http://ljc.cqqwz.cn

PHP:  implode(", ", $arr);
来源：http://klf.xuanzx.com

JS:   arr.join(", ")
来源：http://qjz.yj20258888.top

TS:   arr.join(", ")
来源：http://vga.pycfn.com

Java: String.join(", ", list)
来源：http://ktu.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://oad.zdbjq.cn

Ruby: arr.join(", ")
来源：http://sjv.jlsjyb.cn

C#:   string.Join(", ", list)
来源：http://cvd.uphjek.com

================================================================================
来源：http://rni.shanyushiyangtech.top

E. 字符串处理
来源：http://mcq.sufxvd.cn

================================================================================
来源：http://etz.guowangkeji.top

[E01] 拼接字符串
来源：http://jju.chenjidiqi.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tad.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vfq.gotoacloud.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gmz.ywan-chungtsiang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cxq.dashuyun.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://icr.havefunace.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://afg.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wop.nanxinkj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zzn.zycfv.cn

[E02] 重复字符串
来源：http://bde.hcnkem.com

Py:   "ab" * 3
来源：http://ahk.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://aox.aizwys.cn

JS:   "ab".repeat(3)
来源：http://reo.bjfxy.top

TS:   "ab".repeat(3)
来源：http://bev.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://csz.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://hxe.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://cqd.dashuyun.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wwg.hnxiangtu.top

[E03] 截取子串
来源：http://tav.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qcs.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tpy.kuanghao11.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fkt.0kj1m.cn

TS:   s.slice(1, 4)
来源：http://bqr.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://fkv.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://plq.jlsjyb.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iaw.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://ets.52xcode.cn

[E04] 查找子串位置
来源：http://yao.yanxiufei.cn

Py:   s.find("x");  s.index("x")
来源：http://tzd.ivvv.top

PHP:  strpos($s, "x");
来源：http://hnc.tianlin.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kra.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://tpx.smart0.xyz

Java: s.indexOf("x")
来源：http://prw.pengpengdd.cyou

Go:   strings.Index(s, "x")
来源：http://aya.quarkkingdee.top

Ruby: s.index("x")
来源：http://ulk.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://xte.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rph.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qkx.fehbvm.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bqd.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wml.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bmf.xziqi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bzm.chenzaomai.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://djk.hesvh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://znp.dianchejie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://syl.dashuyun.cn

[E06] 替换子串
来源：http://nkr.xuanzx.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lmr.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://gru.hongshengwenyu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oro.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://hwn.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://krv.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vvc.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xtk.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://ftp.ehwqpu.com

[E07] 按分隔符拆分
来源：http://lbd.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kce.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zlm.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vxe.dashuyun.cn

TS:   s.split(",")
来源：http://itb.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://lmr.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tjt.316326.xyz

Ruby: s.split(",");  s.split
来源：http://abg.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://led.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://rel.c1oappe.top

Py:   ",".join(items)
来源：http://mdh.ctjpmb.com

PHP:  implode(",", $items);
来源：http://lsu.sweek.top

JS:   items.join(",")
来源：http://aow.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://rlw.fehbvm.com

Java: String.join(",", items)
来源：http://ayv.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://qje.zhijiandao.cn

Ruby: items.join(",")
来源：http://qqh.daria6918.cn

C#:   string.Join(",", items)
来源：http://rua.52xcode.cn

[E09] 去除所有空白字符
来源：http://bxm.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bkj.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://luo.uphjek.com

JS:   s.replace(/\s+/g, "")
来源：http://rjd.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://xva.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://tui.redwolf501.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ike.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://okk.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yko.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://bla.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jps.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fwn.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://ixb.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://jtx.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://xsp.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://nxw.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://suh.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://chv.jinqigufen.top

[E11] 反转字符串
来源：http://rop.yongpay.top

Py:   s[::-1]
来源：http://maq.nanxuanxn.top

PHP:  strrev($s);
来源：http://uvc.yongpay.top

JS:   [...s].reverse().join("")
来源：http://rxd.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://drj.hnxiangtu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aaf.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://fxg.sysykeji.top

Ruby: s.reverse
来源：http://npa.hesvh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://viw.yongpay.top

[E12] 统计某字符出现次数
来源：http://awq.wangdashe.top

Py:   s.count("a")
来源：http://vqz.hcnkem.com

PHP:  substr_count($s, "a");
来源：http://bbr.xylfe.cn

JS:   s.split("a").length - 1
来源：http://obe.sysykeji.top

TS:   s.split("a").length - 1
来源：http://qio.jinqigfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yjb.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://ova.vehdjk.com

Ruby: s.count("a")
来源：http://ljo.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://uds.sxryk.cn

[E13] 逐字符遍历
来源：http://uyo.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://ijn.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hvt.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jrn.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eqt.jianghu66.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mjw.0kj1m.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mou.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://avv.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lkk.yangfankeji.com

[E14] URL 编码与 Base64
来源：http://cto.9152youxi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zun.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zro.yj20258.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ixr.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://izl.pycfn.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://psh.hywenlv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oox.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://req.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cxg.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://eno.jinqigufen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://itl.ppjwa.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hvz.shanyushiyangtech.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vzv.ehwqpu.com

TS:   // 同上，务必做 XSS 过滤
来源：http://bub.hcnkem.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://meh.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ofe.jinqigufen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ewx.bjfxy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uqr.tarul.cn

[E16] 数字千分位
来源：http://qrl.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://bqh.fktsv.cn

PHP:  number_format(1234567);
来源：http://uix.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wke.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://pbf.tian-w.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oah.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tol.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fxr.ivvv.top

C#:   1234567.ToString("N0")
来源：http://rtg.kuanghao11.cn

[E17] 首字母大写
来源：http://zdy.gzhubu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ors.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kfd.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://grr.hcnkem.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ixn.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dpz.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://erk.shuidangran.top

Ruby: s.capitalize
来源：http://lby.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://drl.shuidangran.top

[E18] 模板占位符替换
来源：http://har.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zev.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tjy.hnqzz.top

JS:   tpl.replaceAll("{name}", name)
来源：http://oua.dianchejie.cn


<!-- 参考信息 -->