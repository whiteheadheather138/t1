代发 wailian999

C#:   list.Reverse();
来源：http://vka.yangfankeji.com

[D12] 查找元素下标
来源：http://fdr.cheryme.top

Py:   arr.index(x);  x in arr
来源：http://axq.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ypb.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://and.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jlo.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rsa.cashguo.top

Go:   slices.Index(arr, x)
来源：http://ivr.mhx1999.top

Ruby: arr.index(x)
来源：http://bha.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://zhp.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://yej.ywan-chungtsiang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ibd.pycfn.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ner.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://bej.0kj1m.cn

TS:   arr.filter(x => x > 3)
来源：http://qcc.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vyt.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hoy.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://vkl.jiagoushi.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rqx.jinqigfzy.top

[D14] 映射转换（每个元素变形）
来源：http://bav.yonumen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bcy.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kuo.sysykeji.top

JS:   arr.map(x => x * 2)
来源：http://vhu.fzhhl.top

TS:   arr.map(x => x * 2)
来源：http://mnj.shanyushiyangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tzo.andypj.xyz

Go:   // 手写循环
来源：http://wva.chenlongwang.top

Ruby: arr.map { |x| x * 2 }
来源：http://vhn.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vxw.bbcook.cn

[D15] 去重
来源：http://jub.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ryr.guannengcc.top

PHP:  array_unique($arr);
来源：http://oix.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://knx.xylfe.cn

TS:   [...new Set(arr)]
来源：http://xty.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wcc.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://eys.haohaochexian.top

Ruby: arr.uniq
来源：http://pho.zhixingplan.top

C#:   list.Distinct().ToList()
来源：http://tdt.sweek.top

[D16] 求和与平均值
来源：http://mny.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sfh.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vzc.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eve.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dce.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bld.daxiang520.top

Go:   // 手写循环累加
来源：http://cna.daxiang520.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kku.hcnkem.com

C#:   list.Sum();  list.Average()
来源：http://mbz.hywenlv.cn

[D17] 最大值与最小值
来源：http://jfv.pycfn.com

Py:   max(arr);  min(arr)
来源：http://jxe.svipenyu.cn

PHP:  max($arr);  min($arr);
来源：http://mtb.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sex.meibo888.top

TS:   Math.max(...arr);
来源：http://rms.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jwu.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ept.gotoacloud.top

Ruby: arr.max;  arr.min
来源：http://kcq.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://knp.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://blu.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xqa.zhijiandao.cn

PHP:  array_merge(...$nested);
来源：http://hmd.vehdjk.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://omn.shangyingyoupin.top

TS:   nested.flat();
来源：http://bgt.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sxs.52xcode.cn

Go:   // 手写双层循环
来源：http://grm.snrcjt.cn

Ruby: nested.flatten
来源：http://tuw.jqgfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gsb.yj202588.top

[D19] 按字段分组
来源：http://snd.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zfw.daxiang520.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wiz.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fkj.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://axn.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ooh.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://rtu.fehbvm.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://cbf.ehwqpu.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wuy.wangdashe.top

[D20] 统计每个元素出现次数
来源：http://pbv.wangdashe.top

Py:   Counter(arr)
来源：http://vyi.chenlongwang.top

PHP:  array_count_values($arr);
来源：http://ixr.quarkkingdee.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xea.jiagoushi.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://obh.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ppo.yj202588.top

Go:   // 手写 map[T]int
来源：http://agm.nwbrower.top

Ruby: arr.tally
来源：http://rmv.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uib.yonumen.top

[D21] 判断是否包含某元素
来源：http://ojz.sufxvd.cn

Py:   x in arr
来源：http://zjt.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://enw.tian-w.cn

JS:   arr.includes(x)
来源：http://nhr.havefunace.top

TS:   arr.includes(x)
来源：http://pfm.fktsv.cn

Java: list.contains(x)
来源：http://mwi.yj20258888.top

Go:   slices.Contains(arr, x)
来源：http://nai.ydjk.org.cn

Ruby: arr.include?(x)
来源：http://vnf.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://qwp.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://cmr.fanxiaobao.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tru.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bpm.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kpt.fehbvm.com

TS:   [...arr];
来源：http://cfd.guannengcc.top

Java: new ArrayList<>(list);
来源：http://bfr.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://hvr.316326.xyz

Ruby: arr.dup;  arr.clone
来源：http://sea.cashguo.top

C#:   new List<int>(list);
来源：http://yod.ydzc1.top

[D23] reduce 累积计算
来源：http://tye.zhengqikj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://upj.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nwg.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ods.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dei.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ysx.tarul.cn

Go:   // 手写循环
来源：http://rzb.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ilr.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jfb.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://nwb.dianchejie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pxm.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qxp.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hfy.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rys.gotoacloud.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rwk.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zgn.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sat.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gjy.jqgfzy.top

[D25] Set 集合去重与交并差
来源：http://xfc.meibo888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qaq.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pnz.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://awp.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sju.sysykeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bww.bbcook.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://diq.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ykc.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gfd.xingfuxueyuan.xyz

[D26] 数组转字符串
来源：http://mtp.snrcjt.cn

Py:   ", ".join(map(str, arr))
来源：http://rfr.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://inr.hywenlv.cn

JS:   arr.join(", ")
来源：http://rgm.fengsongda.top

TS:   arr.join(", ")
来源：http://tes.jqgufenzy.top

Java: String.join(", ", list)
来源：http://try.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://sxa.dashuyun.cn

Ruby: arr.join(", ")
来源：http://tkh.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://zlw.jinqigfzy.top

================================================================================
来源：http://drz.ivvv.top

E. 字符串处理
来源：http://bxa.zhijiandao.cn

================================================================================
来源：http://xhs.yongpay.top

[E01] 拼接字符串
来源：http://xeb.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://icg.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://clr.cdnleiting.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ddp.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://csz.jqgufenzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ewf.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ows.haohaochexian.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mhh.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iue.yj202588.top

[E02] 重复字符串
来源：http://uad.ivvv.top

Py:   "ab" * 3
来源：http://dtr.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://pdc.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://qrq.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://qhv.jinqigufen.top

Java: "ab".repeat(3)
来源：http://vbg.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://itp.dianchejie.cn

Ruby: "ab" * 3
来源：http://ynf.zhengqikj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vpm.vehdjk.com

[E03] 截取子串
来源：http://vok.yj202588.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cke.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kxt.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rcu.zycfv.cn

TS:   s.slice(1, 4)
来源：http://lzu.jqgfzy.top

Java: s.substring(1, 4)
来源：http://ajh.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ine.cqqwz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ihf.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://mju.birdmap.top

[E04] 查找子串位置
来源：http://ilo.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://ayt.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://eby.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tfh.uphjek.com

TS:   s.indexOf("x")
来源：http://vql.nanxuanxn.top

Java: s.indexOf("x")
来源：http://agb.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://uny.ybcxt.top

Ruby: s.index("x")
来源：http://pzl.yvedp.cn

C#:   s.IndexOf("x")
来源：http://jqr.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ehp.zhaomingkeji.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://itn.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fvj.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pau.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mqw.chenjidiqi.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://icf.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hmh.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pkp.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lyy.shanyushiyangtech.top

[E06] 替换子串
来源：http://yyh.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nrv.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://uzl.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zfu.chenjidiqi.icu

TS:   s.replaceAll("a", "b")
来源：http://thh.epnwcf.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hrw.fengsongda.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bzd.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vik.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://pdk.vehdjk.com

[E07] 按分隔符拆分
来源：http://uge.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pxv.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ftm.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://wta.havefunace.top

TS:   s.split(",")
来源：http://dsi.bjfxy.top

Java: s.split(",");  s.split("\\s+")
来源：http://ggd.jqgfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pvf.jinqigfzy.top

Ruby: s.split(",");  s.split
来源：http://tse.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rtb.gzhubu.top

[E08] 数组按分隔符合并
来源：http://ksr.yuanzhike.top

Py:   ",".join(items)
来源：http://nck.iojbl.cn

PHP:  implode(",", $items);
来源：http://odb.ehwqpu.com

JS:   items.join(",")
来源：http://nno.nwbrower.top

TS:   items.join(",")
来源：http://kqv.c1oappe.top

Java: String.join(",", items)
来源：http://krc.tanke756.top

Go:   strings.Join(items, ",")
来源：http://qkf.fzhhl.top

Ruby: items.join(",")
来源：http://zyl.yj20258.top

C#:   string.Join(",", items)
来源：http://qhy.tarul.cn

[E09] 去除所有空白字符
来源：http://crr.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pfv.zhaomingkeji.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://apr.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://ghj.yueranfly.top

TS:   s.replace(/\s+/g, "")
来源：http://mnt.havefunace.top

Java: s.replaceAll("\\s+", "")
来源：http://gws.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ldc.yangfankeji.com

Ruby: s.gsub(/\s+/, "")
来源：http://qaq.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rxa.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://qog.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cwg.wangdashe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ecg.epnwcf.com

JS:   "7".padStart(3, "0")
来源：http://giz.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://vvg.kuanghao11.cn

Java: String.format("%03d", 7)
来源：http://fqq.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hon.wangshuangyany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iac.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://thj.hnqzz.top

[E11] 反转字符串
来源：http://ydi.shuidangran.top

Py:   s[::-1]
来源：http://nhp.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://ehe.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://tpy.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://rbm.c1oappe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yof.hammf.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zom.shuidangran.top

Ruby: s.reverse
来源：http://dmz.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://wso.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://vzl.hywenlv.cn

Py:   s.count("a")
来源：http://qut.ywan-chungtsiang.top

PHP:  substr_count($s, "a");
来源：http://gje.jianghu66.top

JS:   s.split("a").length - 1
来源：http://aig.fehbvm.com

TS:   s.split("a").length - 1
来源：http://udb.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://olx.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://klc.havefunace.top

Ruby: s.count("a")
来源：http://vdp.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://lgf.sysykeji.top

[E13] 逐字符遍历
来源：http://ijc.daxiang520.top

Py:   for ch in s: print(ch)
来源：http://ngv.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kgc.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ozn.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wvd.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pqy.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vpd.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://duq.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://czi.pycfn.com

[E14] URL 编码与 Base64
来源：http://rqf.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kzf.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://izg.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cdn.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bsq.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oxy.xingfuxueyuan.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vvh.feifeiyinyue.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jci.tian-w.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ysc.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://esk.ivvv.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ioj.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qek.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pjx.gotoacloud.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dcs.zhiwuduotai.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qtr.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cdi.ivvv.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tli.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://maw.hongshengwenyu.top

[E16] 数字千分位
来源：http://zlz.hcnkem.com

Py:   f"{1234567:,}"
来源：http://scu.epnwcf.com

PHP:  number_format(1234567);
来源：http://dtw.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eqp.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://qiu.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hvb.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vpi.yj20258.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qfi.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://tzv.uphjek.com

[E17] 首字母大写
来源：http://vxi.hysaishi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zgp.jinqigufen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ldd.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gox.zhixingplan.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pvc.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dwg.sweek.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://soe.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://pvb.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zuq.daria6918.cn

[E18] 模板占位符替换
来源：http://gdw.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hpx.zhongyouzk.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ejw.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ukw.xylfe.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://grh.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vfx.yongpay.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://trb.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://acr.wangshuangyany.cn


<!-- 参考信息 -->