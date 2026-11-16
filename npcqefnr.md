代发 wailian999

[D11] 反转数组
来源：http://cao.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://gph.fengsongda.top

PHP:  array_reverse($arr);
来源：http://mbb.hfpthk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qoz.bbcook.cn

TS:   [...arr].reverse();
来源：http://nvz.316326.xyz

Java: Collections.reverse(list);
来源：http://vfe.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://vck.0kj1m.cn

Ruby: arr.reverse
来源：http://fuz.jinqigufen.top

C#:   list.Reverse();
来源：http://sil.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://etg.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://hzd.jinqigufen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nff.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yjk.hfpthk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pvr.svipenyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qzg.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://gzs.aibaodan.cn

Ruby: arr.index(x)
来源：http://run.yonumen.top

C#:   list.IndexOf(x);
来源：http://obk.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://rlc.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dti.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://whg.9152youxi.cn

JS:   arr.filter(x => x > 3)
来源：http://hfa.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://kby.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vzo.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uyf.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jsu.pengpengdd.cyou

C#:   list.Where(x => x > 3).ToList()
来源：http://dft.gogol.net.cn

[D14] 映射转换（每个元素变形）
来源：http://ymd.haohaochexian.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vvr.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zoa.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://hzx.svipenyu.cn

TS:   arr.map(x => x * 2)
来源：http://fwn.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zoy.hysaishi.cn

Go:   // 手写循环
来源：http://aru.c1oappe.top

Ruby: arr.map { |x| x * 2 }
来源：http://bqg.guowangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vfx.cqqwz.cn

[D15] 去重
来源：http://lfa.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jif.haohaochexian.top

PHP:  array_unique($arr);
来源：http://vdn.daria6918.cn

JS:   [...new Set(arr)]
来源：http://ttc.yuxming.cn

TS:   [...new Set(arr)]
来源：http://zpu.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dgw.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bdq.ivvv.top

Ruby: arr.uniq
来源：http://tbv.aizwys.cn

C#:   list.Distinct().ToList()
来源：http://zsd.yanxiufei.cn

[D16] 求和与平均值
来源：http://mqc.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yev.yuxming.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baz.dashuyun.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uul.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lxd.sysykeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://twk.gaohongyu789.top

Go:   // 手写循环累加
来源：http://taj.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://niu.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://pee.feifeiyinyue.top

[D17] 最大值与最小值
来源：http://spd.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://mlm.iojbl.cn

PHP:  max($arr);  min($arr);
来源：http://mie.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zxg.hesvh.cn

TS:   Math.max(...arr);
来源：http://brk.ehwqpu.com

Java: Collections.max(list);  Collections.min(list);
来源：http://zml.smart0.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tgx.ydzc1.top

Ruby: arr.max;  arr.min
来源：http://kqu.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://brf.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://csj.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kgc.jianghu66.top

PHP:  array_merge(...$nested);
来源：http://ymy.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fsp.jlsjyb.cn

TS:   nested.flat();
来源：http://cbl.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uaf.smart0.xyz

Go:   // 手写双层循环
来源：http://mbb.redwolf501.top

Ruby: nested.flatten
来源：http://iki.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://odb.sxryk.cn

[D19] 按字段分组
来源：http://rtf.jinyuanbaomall.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://atg.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vpo.c1oappe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jwd.ppjwa.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qxk.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xlz.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://soi.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wdg.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nzz.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://kco.quarkkingdee.top

Py:   Counter(arr)
来源：http://fwi.pycfn.com

PHP:  array_count_values($arr);
来源：http://vrc.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ssc.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://clr.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kfl.svipenyu.cn

Go:   // 手写 map[T]int
来源：http://noq.zhijiandao.cn

Ruby: arr.tally
来源：http://csp.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wta.kuanghao11.cn

[D21] 判断是否包含某元素
来源：http://weh.daria6918.cn

Py:   x in arr
来源：http://jkr.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://aey.yuxming.cn

JS:   arr.includes(x)
来源：http://ynp.zhixingplan.top

TS:   arr.includes(x)
来源：http://rxj.vehdjk.com

Java: list.contains(x)
来源：http://chh.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://ryh.yongpay.top

Ruby: arr.include?(x)
来源：http://uot.dashuyun.cn

C#:   list.Contains(x)
来源：http://vso.tanke756.top

[D22] 复制数组（避免共享引用）
来源：http://ofl.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://akp.hnxiangtu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ghv.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zzw.gaohongyu789.top

TS:   [...arr];
来源：http://klq.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://lsf.zhengqikj.top

Go:   copied := append([]int(nil), arr...)
来源：http://xmu.cdnleiting.top

Ruby: arr.dup;  arr.clone
来源：http://tbq.cheryme.top

C#:   new List<int>(list);
来源：http://qer.smart0.xyz

[D23] reduce 累积计算
来源：http://wlr.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bcm.jqgfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jji.daria6918.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yaz.cdnleiting.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rjl.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bys.hongshengwenyu.top

Go:   // 手写循环
来源：http://ynn.yj20258.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ulg.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wui.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://rlq.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cwk.uphjek.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pef.gzhubu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ewn.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dao.tanke756.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yri.yuxming.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hxg.jlsjyb.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rkr.hnxiangtu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lyh.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://rdz.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fgx.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ega.tianlin.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dty.ppjwa.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hxm.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dpq.yangfankeji.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ytk.cashguo.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ajz.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qag.fengsongda.top

[D26] 数组转字符串
来源：http://lbj.kuanghao11.cn

Py:   ", ".join(map(str, arr))
来源：http://fvm.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://pjs.fzhhl.top

JS:   arr.join(", ")
来源：http://civ.andypj.xyz

TS:   arr.join(", ")
来源：http://rrw.tanke756.top

Java: String.join(", ", list)
来源：http://uof.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://nan.yfazqb.com

Ruby: arr.join(", ")
来源：http://akj.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://uol.yj20258.top

================================================================================
来源：http://jdd.nanxuanxn.top

E. 字符串处理
来源：http://fxt.chenjidiqi.icu

================================================================================
来源：http://gog.hongshengwenyu.top

[E01] 拼接字符串
来源：http://ven.jqgufenzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yvl.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jar.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qof.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xkx.tian-w.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://itj.tanke756.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://znk.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jog.ybcxt.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jbc.fktsv.cn

[E02] 重复字符串
来源：http://ini.9152youxi.cn

Py:   "ab" * 3
来源：http://lxt.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://hcs.tian-w.cn

JS:   "ab".repeat(3)
来源：http://vcg.zdbjq.cn

TS:   "ab".repeat(3)
来源：http://gpx.9152youxi.cn

Java: "ab".repeat(3)
来源：http://rfl.ywan-chungtsiang.top

Go:   strings.Repeat("ab", 3)
来源：http://yfp.haohaochexian.top

Ruby: "ab" * 3
来源：http://hzn.aizwys.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vly.fktsv.cn

[E03] 截取子串
来源：http://fxe.yuanzhike.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gbr.nwbrower.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oag.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xdk.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://fuy.cucudq.cn

Java: s.substring(1, 4)
来源：http://zbr.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fzd.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://fil.hnqzz.top

C#:   s.Substring(1, 3)
来源：http://cyx.52xcode.cn

[E04] 查找子串位置
来源：http://iwh.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://xtb.xinyue.icu

PHP:  strpos($s, "x");
来源：http://epa.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kqw.fengsongda.top

TS:   s.indexOf("x")
来源：http://hxm.kuanghao11.cn

Java: s.indexOf("x")
来源：http://xsh.tarul.cn

Go:   strings.Index(s, "x")
来源：http://hap.yfazqb.com

Ruby: s.index("x")
来源：http://kyz.cheryme.top

C#:   s.IndexOf("x")
来源：http://vwk.hnqzz.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ejt.zycfv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xry.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://des.9152youxi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bct.xinyue.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://mgg.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hkd.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bzi.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lay.dashuyun.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pvn.andypj.xyz

[E06] 替换子串
来源：http://dqo.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hzh.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://xer.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qxt.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://teq.chenlongwang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gdu.jqgufenzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tok.sjlbkw.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gis.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://wbi.wangshuangyany.cn

[E07] 按分隔符拆分
来源：http://vpo.tanke756.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wex.gotoacloud.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rdf.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xjx.shangyingyoupin.top

TS:   s.split(",")
来源：http://qpx.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://all.shanyushiyangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gml.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://ylr.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kuj.yonumen.top

[E08] 数组按分隔符合并
来源：http://rdj.andypj.xyz

Py:   ",".join(items)
来源：http://hti.yfazqb.com

PHP:  implode(",", $items);
来源：http://khk.hcnkem.com

JS:   items.join(",")
来源：http://uee.ctjpmb.com

TS:   items.join(",")
来源：http://pct.xziqi.cn

Java: String.join(",", items)
来源：http://vaz.xuetiantiany.cn

Go:   strings.Join(items, ",")
来源：http://gph.iojbl.cn

Ruby: items.join(",")
来源：http://xen.jiagoushi.top

C#:   string.Join(",", items)
来源：http://ing.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://iar.shuidangran.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://huj.xziqi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sjb.fehbvm.com

JS:   s.replace(/\s+/g, "")
来源：http://clf.feifeiyinyue.top

TS:   s.replace(/\s+/g, "")
来源：http://flx.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://aqe.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://csw.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://utm.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ueo.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://wiz.tian-w.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aoz.cdnleiting.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ucb.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://wtt.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://ulc.sweek.top

Java: String.format("%03d", 7)
来源：http://bpd.9152youxi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yex.jianghu66.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tem.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zfk.c1oappe.top

[E11] 反转字符串
来源：http://dik.yongpay.top

Py:   s[::-1]
来源：http://xhp.tian-w.cn

PHP:  strrev($s);
来源：http://ckr.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://vfx.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://lmx.sysykeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rtq.epnwcf.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://bgu.chenzaomai.com

Ruby: s.reverse
来源：http://rkm.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://neq.zhixingplan.top

[E12] 统计某字符出现次数
来源：http://xlk.hnqzz.top

Py:   s.count("a")
来源：http://rhe.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://qkj.zhengqikj.top

JS:   s.split("a").length - 1
来源：http://tei.aizwys.cn

TS:   s.split("a").length - 1
来源：http://eya.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nqq.vqdsnc.cn

Go:   strings.Count(s, "a")
来源：http://jjy.zhiwuduotai.top

Ruby: s.count("a")
来源：http://oye.kuanghao11.cn

C#:   s.Count(c => c == 'a')
来源：http://hlz.shuidangran.top

[E13] 逐字符遍历
来源：http://thf.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://yhb.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wbl.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jxy.shzxlz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pbp.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hgm.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qqc.shanyushiyangtech.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wkk.guannengcc.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://whp.fzhhl.top

[E14] URL 编码与 Base64
来源：http://goh.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jva.c1oappe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zak.xziqi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rig.yfazqb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rxj.hnqzz.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vvo.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fpi.zhongyouzk.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wjl.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tck.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://ktx.wangshuangyany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wlm.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kyq.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rlz.kuanghao11.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gpm.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://thf.nanxuanxn.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jas.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iva.shanyushiyangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jmo.ivvv.top

[E16] 数字千分位
来源：http://zai.wangdashe.top

Py:   f"{1234567:,}"
来源：http://afw.sweek.top

PHP:  number_format(1234567);
来源：http://dsy.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wyu.guowangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wic.316326.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bzf.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vec.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jsk.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://lzs.jinqigufen.top

[E17] 首字母大写
来源：http://bhs.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cgw.52xcode.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zgb.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xdq.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mye.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jmp.jianghu66.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cqo.aizwys.cn

Ruby: s.capitalize
来源：http://aun.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yqy.kuanghao11.cn


<!-- 参考信息 -->