代发 wailian999

TS:   [...arr].reverse();
来源：http://uos.yj20258.top

Java: Collections.reverse(list);
来源：http://avo.vehdjk.com

Go:   slices.Reverse(arr)
来源：http://wyr.hongshengwenyu.top

Ruby: arr.reverse
来源：http://sco.yj20258.top

C#:   list.Reverse();
来源：http://zun.wangshuangyany.cn

[D12] 查找元素下标
来源：http://ajf.xuanzx.com

Py:   arr.index(x);  x in arr
来源：http://tao.sjlbkw.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ynm.hnxiangtu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vov.cdnleiting.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yrq.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vnf.xinyue.icu

Go:   slices.Index(arr, x)
来源：http://sen.chenlongwang.top

Ruby: arr.index(x)
来源：http://qbp.gogol.net.cn

C#:   list.IndexOf(x);
来源：http://hja.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://cpj.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mby.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cxi.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://qwm.cdnleiting.top

TS:   arr.filter(x => x > 3)
来源：http://yro.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gsy.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://erp.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://vrc.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rjw.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://chm.hongshengwenyu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://axs.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kxt.nanxuanxn.top

JS:   arr.map(x => x * 2)
来源：http://cls.52xcode.cn

TS:   arr.map(x => x * 2)
来源：http://rpb.xingfuxueyuan.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://xdy.snrcjt.cn

Go:   // 手写循环
来源：http://ghw.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://flk.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mtk.chenzaomai.com

[D15] 去重
来源：http://nxq.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ymx.zhiwuduotai.top

PHP:  array_unique($arr);
来源：http://iut.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://kyz.fzhhl.top

TS:   [...new Set(arr)]
来源：http://qpk.sxryk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://izl.gaohongyu789.top

Go:   // 用 map[T]struct{} 手写
来源：http://yqq.guowangkeji.top

Ruby: arr.uniq
来源：http://xox.chenjidiqi.icu

C#:   list.Distinct().ToList()
来源：http://xhw.zhiwuduotai.top

[D16] 求和与平均值
来源：http://bat.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dgc.gotoacloud.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hjh.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cuo.zhijiandao.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ujb.yj20258888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kgi.sysykeji.top

Go:   // 手写循环累加
来源：http://ygu.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ewy.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://nlk.quarkkingdee.top

[D17] 最大值与最小值
来源：http://bbl.hammf.cn

Py:   max(arr);  min(arr)
来源：http://aal.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://ibk.sysykeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jzv.mhx1999.top

TS:   Math.max(...arr);
来源：http://bjy.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://umv.fengsongda.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gxn.meibo888.top

Ruby: arr.max;  arr.min
来源：http://szf.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://ghg.fktsv.cn

[D18] 扁平化嵌套数组
来源：http://kwn.zhiwuduotai.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tys.sufxvd.cn

PHP:  array_merge(...$nested);
来源：http://cas.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hwj.dashuyun.cn

TS:   nested.flat();
来源：http://bfi.yj20258.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ksd.sufxvd.cn

Go:   // 手写双层循环
来源：http://lfm.zhengqikj.top

Ruby: nested.flatten
来源：http://ngt.xingfuxueyuan.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://kks.bbcook.cn

[D19] 按字段分组
来源：http://gyh.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qvy.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vkd.cqqwz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://erw.nanxuanxn.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dlh.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xpp.fehbvm.com

Go:   // 手写 map[string][]T
来源：http://jmt.jianghu66.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wmy.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mus.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://plk.nwbrower.top

Py:   Counter(arr)
来源：http://jts.bbcook.cn

PHP:  array_count_values($arr);
来源：http://kay.uphjek.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://azs.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jsl.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ivi.tanke756.top

Go:   // 手写 map[T]int
来源：http://map.vehdjk.com

Ruby: arr.tally
来源：http://svc.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rnz.smart0.xyz

[D21] 判断是否包含某元素
来源：http://luv.shzxlz.cn

Py:   x in arr
来源：http://yfu.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://tjq.daxiang520.top

JS:   arr.includes(x)
来源：http://oso.bjfxy.top

TS:   arr.includes(x)
来源：http://jib.cqqwz.cn

Java: list.contains(x)
来源：http://dpy.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://may.jiagoushi.top

Ruby: arr.include?(x)
来源：http://mrt.bbcook.cn

C#:   list.Contains(x)
来源：http://lws.c1oappe.top

[D22] 复制数组（避免共享引用）
来源：http://rtw.hywenlv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rhe.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ymb.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://egl.uphjek.com

TS:   [...arr];
来源：http://qua.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://ksb.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nyo.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://csi.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://ygn.zycfv.cn

[D23] reduce 累积计算
来源：http://wdv.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yhg.kuanghao11.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vcf.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pfb.jinqigfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xdo.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bbh.fanxiaobao.xyz

Go:   // 手写循环
来源：http://wyf.hammf.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yjz.9152youxi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xjk.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://wka.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xbk.tianlin.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mji.sweek.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yrz.ctjpmb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://upz.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dje.havefunace.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cpv.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://war.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qol.meibo888.top

[D25] Set 集合去重与交并差
来源：http://sdo.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hwv.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xhu.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qdz.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xrk.hywenlv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rpy.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bht.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tcb.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fny.wangshuangyany.cn

[D26] 数组转字符串
来源：http://gqc.kuanghao11.cn

Py:   ", ".join(map(str, arr))
来源：http://xie.meibo888.top

PHP:  implode(", ", $arr);
来源：http://bht.hnqzz.top

JS:   arr.join(", ")
来源：http://lhm.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://dwf.yanxiufei.cn

Java: String.join(", ", list)
来源：http://lsg.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://jzc.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://fxt.vqdsnc.cn

C#:   string.Join(", ", list)
来源：http://dzy.wangshuangyany.cn

================================================================================
来源：http://mvl.zdbjq.cn

E. 字符串处理
来源：http://nzl.aibaodan.cn

================================================================================
来源：http://vql.zhijiandao.cn

[E01] 拼接字符串
来源：http://jqn.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://riy.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jst.nanxuanxn.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pxu.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://egb.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gep.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eks.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pro.jlsjyb.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://idf.cdnleiting.top

[E02] 重复字符串
来源：http://qqe.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://ioc.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://wwu.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://wka.birdmap.top

TS:   "ab".repeat(3)
来源：http://eqh.hammf.cn

Java: "ab".repeat(3)
来源：http://mwn.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://krb.vehdjk.com

Ruby: "ab" * 3
来源：http://lpm.xinyue.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tnc.yueranfly.top

[E03] 截取子串
来源：http://sre.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pwc.yj20258.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fgo.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hfo.sysykeji.top

TS:   s.slice(1, 4)
来源：http://awf.chenzaomai.com

Java: s.substring(1, 4)
来源：http://aqw.dashuyun.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zxw.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://hsp.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://sui.epnwcf.com

[E04] 查找子串位置
来源：http://lei.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://yde.vehdjk.com

PHP:  strpos($s, "x");
来源：http://xdd.nanxinkj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bmt.daxiang520.top

TS:   s.indexOf("x")
来源：http://hdr.yfazqb.com

Java: s.indexOf("x")
来源：http://jwx.yueranfly.top

Go:   strings.Index(s, "x")
来源：http://qcx.ctjpmb.com

Ruby: s.index("x")
来源：http://zos.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://gdz.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://juq.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mnj.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ujn.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kzm.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bsf.jyoumei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jqh.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aff.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tvv.hysaishi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rid.hysaishi.cn

[E06] 替换子串
来源：http://qwu.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ecv.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://uqz.bjfxy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yjb.yongpay.top

TS:   s.replaceAll("a", "b")
来源：http://yzz.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hlw.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ifi.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vih.ybcxt.top

C#:   s.Replace("a", "b")
来源：http://jzc.tanke756.top

[E07] 按分隔符拆分
来源：http://pex.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://owq.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fwm.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://mvx.guowangkeji.top

TS:   s.split(",")
来源：http://rwc.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://jcm.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rkr.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://jri.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zci.uphjek.com

[E08] 数组按分隔符合并
来源：http://ezi.feifeiyinyue.top

Py:   ",".join(items)
来源：http://yru.52xcode.cn

PHP:  implode(",", $items);
来源：http://ibh.quarkkingdee.top

JS:   items.join(",")
来源：http://sxk.ydzc1.top

TS:   items.join(",")
来源：http://ajx.bbcook.cn

Java: String.join(",", items)
来源：http://xyp.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://nqd.kuanghao11.cn

Ruby: items.join(",")
来源：http://oda.jyoumei.cn

C#:   string.Join(",", items)
来源：http://iwu.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://jjb.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zcc.andypj.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ksw.vqdsnc.cn

JS:   s.replace(/\s+/g, "")
来源：http://afy.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://zho.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://yal.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mme.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://lwj.pengpengdd.cyou

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yfk.shanyushiyangtech.top

[E10] 左侧补零 / 定长填充
来源：http://xpc.sxryk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hwk.sjlbkw.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gdx.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://ftv.shzxlz.cn

TS:   "7".padStart(3, "0")
来源：http://ktv.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://yuo.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pee.hesvh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fza.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aal.yongpay.top

[E11] 反转字符串
来源：http://dsk.jyoumei.cn

Py:   s[::-1]
来源：http://ops.sufxvd.cn

PHP:  strrev($s);
来源：http://hdr.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://wpm.pycfn.com

TS:   [...s].reverse().join("")
来源：http://gnu.redwolf501.top

Java: new StringBuilder(s).reverse().toString()
来源：http://twp.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hqw.ctjpmb.com

Ruby: s.reverse
来源：http://tyv.ydzc1.top

C#:   new string(s.Reverse().ToArray())
来源：http://wmh.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://qph.yongpay.top

Py:   s.count("a")
来源：http://zbc.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://hcu.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://mre.jlsjyb.cn

TS:   s.split("a").length - 1
来源：http://wrn.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wzj.pengpengdd.cyou

Go:   strings.Count(s, "a")
来源：http://tez.316326.xyz

Ruby: s.count("a")
来源：http://mxf.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://yzy.xinyue.icu

[E13] 逐字符遍历
来源：http://ykh.hysaishi.cn

Py:   for ch in s: print(ch)
来源：http://ptg.zhoulong.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vec.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bwj.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zli.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sng.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kal.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nlh.tian-w.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cip.zdqjudy.top

[E14] URL 编码与 Base64
来源：http://yzn.nwbrower.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oqd.c1oappe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mwu.jinghuilouyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nfg.xinyue.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://onb.yangfankeji.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jyq.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cmy.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vrg.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fbj.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://bdg.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://psf.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tir.sjlbkw.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blq.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://tbk.iojbl.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wee.havefunace.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://imc.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mlf.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jfx.xylfe.cn

[E16] 数字千分位
来源：http://szs.pycfn.com

Py:   f"{1234567:,}"
来源：http://psc.hongshengwenyu.top

PHP:  number_format(1234567);
来源：http://kbe.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gxw.hysaishi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hqg.tian-w.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ffr.gzhubu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wis.jqgfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gom.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://pou.c1oappe.top

[E17] 首字母大写
来源：http://ivx.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xsa.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://smi.guowangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jcy.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mni.yuanzhike.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://onr.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pxc.gotoacloud.top

Ruby: s.capitalize
来源：http://eso.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://shc.xinyue.icu

[E18] 模板占位符替换
来源：http://mxn.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xfc.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sux.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vwg.nanxinkj.top


<!-- 参考信息 -->