代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iky.316326.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hyk.chenjidiqi.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qkr.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://giz.tian-w.cn

Ruby: arr.index(x)
来源：http://god.wangdashe.top

C#:   list.IndexOf(x);
来源：http://chf.zhixingplan.top

[D13] 过滤（保留满足条件的）
来源：http://gjo.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jtf.smart0.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qir.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://vxd.ydjk.org.cn

TS:   arr.filter(x => x > 3)
来源：http://udd.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nwh.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bef.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qdm.xziqi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gyf.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://dfj.meibo888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bbb.bbcook.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mct.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://rtm.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://rip.shanyushiyangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://aco.shanyushiyangtech.top

Go:   // 手写循环
来源：http://iej.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://nyi.zhixingplan.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sry.guannengcc.top

[D15] 去重
来源：http://obt.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://olx.ppjwa.cn

PHP:  array_unique($arr);
来源：http://xiy.c1oappe.top

JS:   [...new Set(arr)]
来源：http://jir.52xcode.cn

TS:   [...new Set(arr)]
来源：http://xll.ydjk.org.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ntb.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hwe.hnqzz.top

Ruby: arr.uniq
来源：http://eiu.cheryme.top

C#:   list.Distinct().ToList()
来源：http://ckh.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://big.hywenlv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oga.gotoacloud.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uny.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pnv.wangshuangyany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zoy.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fzi.aizwys.cn

Go:   // 手写循环累加
来源：http://zrv.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ywz.fktsv.cn

C#:   list.Sum();  list.Average()
来源：http://yed.yueranfly.top

[D17] 最大值与最小值
来源：http://ckq.cheryme.top

Py:   max(arr);  min(arr)
来源：http://cpl.ydzc1.top

PHP:  max($arr);  min($arr);
来源：http://mrx.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fet.yuanzhike.top

TS:   Math.max(...arr);
来源：http://gjo.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://euz.jyoumei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lnz.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://zpt.jiagoushi.top

C#:   list.Max();  list.Min()
来源：http://fct.snrcjt.cn

[D18] 扁平化嵌套数组
来源：http://ngj.aizwys.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gkw.ivvv.top

PHP:  array_merge(...$nested);
来源：http://hqf.hammf.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nzc.tianlin.xyz

TS:   nested.flat();
来源：http://mfi.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nkd.fengsongda.top

Go:   // 手写双层循环
来源：http://lrj.hywenlv.cn

Ruby: nested.flatten
来源：http://rxh.yuxming.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://srg.sjlbkw.cn

[D19] 按字段分组
来源：http://pdt.svipenyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://djr.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oqn.nanxinkj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nts.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://npx.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://piy.hcnkem.com

Go:   // 手写 map[string][]T
来源：http://jhs.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://zby.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lug.zhengqikj.top

[D20] 统计每个元素出现次数
来源：http://fhy.9152youxi.cn

Py:   Counter(arr)
来源：http://ypa.haohaochexian.top

PHP:  array_count_values($arr);
来源：http://tqa.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vvo.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rdt.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qdj.yfazqb.com

Go:   // 手写 map[T]int
来源：http://dbm.jqgufenzy.top

Ruby: arr.tally
来源：http://dna.zhoulong.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sta.yfazqb.com

[D21] 判断是否包含某元素
来源：http://dcy.sjlbkw.cn

Py:   x in arr
来源：http://awx.yuanzhike.top

PHP:  in_array($x, $arr, true);
来源：http://kjk.birdmap.top

JS:   arr.includes(x)
来源：http://iri.52xcode.cn

TS:   arr.includes(x)
来源：http://hht.yj202588.top

Java: list.contains(x)
来源：http://iek.zdbjq.cn

Go:   slices.Contains(arr, x)
来源：http://caa.cashguo.top

Ruby: arr.include?(x)
来源：http://mhz.c1oappe.top

C#:   list.Contains(x)
来源：http://cra.cashguo.top

[D22] 复制数组（避免共享引用）
来源：http://lzg.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jhs.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rcv.cucudq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eqc.yj202588.top

TS:   [...arr];
来源：http://nei.wangdashe.top

Java: new ArrayList<>(list);
来源：http://deu.shzxlz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ejs.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://kho.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://tmv.zhijiandao.cn

[D23] reduce 累积计算
来源：http://cke.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kmd.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tlm.vqdsnc.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tfb.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wyy.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://pdo.shzxlz.cn

Go:   // 手写循环
来源：http://qco.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jmv.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kgm.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://hqz.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mjz.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://igc.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ubm.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uyf.tarul.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lph.cashguo.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hod.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ewx.haohaochexian.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yui.havefunace.top

[D25] Set 集合去重与交并差
来源：http://ivc.yangfankeji.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cww.xuanzx.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bsb.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wym.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yvn.sweek.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cmf.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rwr.hongshengwenyu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sff.dashuyun.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eyj.hfpthk.cn

[D26] 数组转字符串
来源：http://rzl.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://qfy.pycfn.com

PHP:  implode(", ", $arr);
来源：http://fod.jyoumei.cn

JS:   arr.join(", ")
来源：http://ydn.jlsjyb.cn

TS:   arr.join(", ")
来源：http://yzp.cheryme.top

Java: String.join(", ", list)
来源：http://cml.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://nuu.chenjidiqi.icu

Ruby: arr.join(", ")
来源：http://kna.hesvh.cn

C#:   string.Join(", ", list)
来源：http://jst.ybcxt.top

================================================================================
来源：http://hvj.epnwcf.com

E. 字符串处理
来源：http://upm.xuetiantiany.cn

================================================================================
来源：http://eux.yvedp.cn

[E01] 拼接字符串
来源：http://jyt.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://idn.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mbf.cucudq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ern.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jex.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dxb.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kgl.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xdw.yj20258.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qxb.uphjek.com

[E02] 重复字符串
来源：http://zas.cashguo.top

Py:   "ab" * 3
来源：http://psm.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://etc.havefunace.top

JS:   "ab".repeat(3)
来源：http://pce.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://odj.yvedp.cn

Java: "ab".repeat(3)
来源：http://fny.hywenlv.cn

Go:   strings.Repeat("ab", 3)
来源：http://avt.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://jdv.jinghuilouyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fyh.chenjidiqi.icu

[E03] 截取子串
来源：http://hxs.jianghu66.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://afs.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pfq.sxryk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aky.hammf.cn

TS:   s.slice(1, 4)
来源：http://cfg.gaohongyu789.top

Java: s.substring(1, 4)
来源：http://xnc.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kmz.jqgfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://sat.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://tns.chenlongwang.top

[E04] 查找子串位置
来源：http://thi.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://hwp.cucudq.cn

PHP:  strpos($s, "x");
来源：http://crc.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tur.birdmap.top

TS:   s.indexOf("x")
来源：http://dlf.vqdsnc.cn

Java: s.indexOf("x")
来源：http://sbg.tanke756.top

Go:   strings.Index(s, "x")
来源：http://jee.pengpengdd.cyou

Ruby: s.index("x")
来源：http://eis.zhiwuduotai.top

C#:   s.IndexOf("x")
来源：http://lef.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mav.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jhx.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://giz.xylfe.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cbk.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://pds.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rdy.gaohongyu789.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gik.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wfi.dianchejie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sew.ybcxt.top

[E06] 替换子串
来源：http://hsh.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fqt.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://tfo.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pwb.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://xdd.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://php.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rxa.yueranfly.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://muz.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://imw.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://sgw.jinqigfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hpp.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vwy.tanke756.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tmf.ppjwa.cn

TS:   s.split(",")
来源：http://foz.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://hpl.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://djk.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://kog.zhijiandao.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lmk.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://ppr.uphjek.com

Py:   ",".join(items)
来源：http://jgn.zhengqikj.top

PHP:  implode(",", $items);
来源：http://xpq.jinqigfzy.top

JS:   items.join(",")
来源：http://rvz.0kj1m.cn

TS:   items.join(",")
来源：http://sac.zdbjq.cn

Java: String.join(",", items)
来源：http://gyh.wangdashe.top

Go:   strings.Join(items, ",")
来源：http://tjq.zhengqikj.top

Ruby: items.join(",")
来源：http://qkx.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://dcv.cucudq.cn

[E09] 去除所有空白字符
来源：http://dex.xuetiantiany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bvu.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lze.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://pjp.tian-w.cn

TS:   s.replace(/\s+/g, "")
来源：http://vre.jqgufenzy.top

Java: s.replaceAll("\\s+", "")
来源：http://zdz.xuanzx.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://vue.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://aqo.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uas.pengpengdd.cyou

[E10] 左侧补零 / 定长填充
来源：http://hti.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ilk.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nty.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://qan.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://zmm.kuanghao11.cn

Java: String.format("%03d", 7)
来源：http://cyz.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://toq.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kim.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://icn.gaohongyu789.top

[E11] 反转字符串
来源：http://trk.andypj.xyz

Py:   s[::-1]
来源：http://udk.snrcjt.cn

PHP:  strrev($s);
来源：http://gyg.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://vyn.tian-w.cn

TS:   [...s].reverse().join("")
来源：http://zly.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://apv.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uzj.bbcook.cn

Ruby: s.reverse
来源：http://zll.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oma.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://vom.shzxlz.cn

Py:   s.count("a")
来源：http://fwr.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://zrk.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://djr.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://nvx.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wju.tarul.cn

Go:   strings.Count(s, "a")
来源：http://png.hywenlv.cn

Ruby: s.count("a")
来源：http://rjw.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://czg.fehbvm.com

[E13] 逐字符遍历
来源：http://uxe.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://des.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sye.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hgd.tarul.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yfn.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hlu.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://osu.wangshuangyany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ivj.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pcv.yfazqb.com

[E14] URL 编码与 Base64
来源：http://ozq.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zmr.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jze.hcnkem.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://csh.xinyue.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://swg.zhiwuduotai.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rhj.smart0.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hiu.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dkc.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ojy.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://nir.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zuw.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mhd.shzxlz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://emb.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lyn.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ked.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pik.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xot.shangyingyoupin.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tii.zycfv.cn

[E16] 数字千分位
来源：http://uml.redwolf501.top

Py:   f"{1234567:,}"
来源：http://nuj.chenjidiqi.icu

PHP:  number_format(1234567);
来源：http://qpv.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://iyk.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://edp.zdqjudy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gxa.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hak.shuidangran.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tmj.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://hvd.tarul.cn

[E17] 首字母大写
来源：http://xwj.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xhp.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nii.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vdb.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lwm.xingfuxueyuan.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://biq.tarul.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wee.9152youxi.cn

Ruby: s.capitalize
来源：http://sei.daxiang520.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bzy.zdbjq.cn

[E18] 模板占位符替换
来源：http://chj.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gsi.andypj.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kdd.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://vwq.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qht.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ttr.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://evj.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fla.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ymz.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://krx.yangfankeji.com

Py:   s.splitlines()
来源：http://qjj.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pdh.nwbrower.top


<!-- 参考信息 -->