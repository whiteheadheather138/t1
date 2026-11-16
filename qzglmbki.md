代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://prb.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://obp.jiagoushi.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nzk.jyoumei.cn

[D14] 映射转换（每个元素变形）
来源：http://lbs.xuanzx.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mzp.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nde.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://zjh.ybcxt.top

TS:   arr.map(x => x * 2)
来源：http://dsn.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fwd.jqgfzy.top

Go:   // 手写循环
来源：http://yhr.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bur.0kj1m.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ztj.hnqzz.top

[D15] 去重
来源：http://var.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cve.xingfuxueyuan.xyz

PHP:  array_unique($arr);
来源：http://wgj.hnqzz.top

JS:   [...new Set(arr)]
来源：http://umg.xuetiantiany.cn

TS:   [...new Set(arr)]
来源：http://nwh.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://row.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://ckw.jyoumei.cn

Ruby: arr.uniq
来源：http://oii.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://zdg.shangyingyoupin.top

[D16] 求和与平均值
来源：http://wws.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://akj.hfpthk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bmh.andypj.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zey.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nke.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xgm.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://oge.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fir.jinqigufen.top

C#:   list.Sum();  list.Average()
来源：http://huc.guannengcc.top

[D17] 最大值与最小值
来源：http://dqv.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://ofu.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://fcw.sufxvd.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qbv.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://djv.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bmz.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tmg.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://uxs.shanyushiyangkeji.top

C#:   list.Max();  list.Min()
来源：http://eyj.tarul.cn

[D18] 扁平化嵌套数组
来源：http://eph.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mkn.yj20258.top

PHP:  array_merge(...$nested);
来源：http://umn.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qst.uphjek.com

TS:   nested.flat();
来源：http://lme.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kjp.yonumen.top

Go:   // 手写双层循环
来源：http://jhv.birdmap.top

Ruby: nested.flatten
来源：http://nhl.9152youxi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nyu.zdbjq.cn

[D19] 按字段分组
来源：http://qzl.birdmap.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nau.zhongyouzk.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wws.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rex.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://tmw.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pvl.redwolf501.top

Go:   // 手写 map[string][]T
来源：http://wtq.hfpthk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vaz.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pqs.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://tlk.tianlin.xyz

Py:   Counter(arr)
来源：http://xuu.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://een.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nmt.zhaomingkeji.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xsc.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rvz.guannengcc.top

Go:   // 手写 map[T]int
来源：http://ffe.9152youxi.cn

Ruby: arr.tally
来源：http://omv.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wkg.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://pda.dashuyun.cn

Py:   x in arr
来源：http://ygw.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://csr.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://jll.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://puh.jinqigfzy.top

Java: list.contains(x)
来源：http://stx.ivvv.top

Go:   slices.Contains(arr, x)
来源：http://ynp.aizwys.cn

Ruby: arr.include?(x)
来源：http://zzi.yuanzhike.top

C#:   list.Contains(x)
来源：http://rli.hongshengwenyu.top

[D22] 复制数组（避免共享引用）
来源：http://hep.wangshuangyany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vqv.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ugp.xziqi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uev.52xcode.cn

TS:   [...arr];
来源：http://jdy.gzhubu.top

Java: new ArrayList<>(list);
来源：http://ibq.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://ahz.hammf.cn

Ruby: arr.dup;  arr.clone
来源：http://mzp.tianlin.xyz

C#:   new List<int>(list);
来源：http://uxl.uphjek.com

[D23] reduce 累积计算
来源：http://uek.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ttz.jyoumei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://naz.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://icj.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oij.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bfh.andypj.xyz

Go:   // 手写循环
来源：http://ugw.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kjw.sweek.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ucn.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://ggf.9152youxi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xqi.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://upe.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wua.shuidangran.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mjq.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zrz.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wfq.cashguo.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kmq.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mdt.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://lan.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hdu.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bqk.ydjk.org.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://puz.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nax.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ogi.zhaomingkeji.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kqj.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bju.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aen.gotoacloud.top

[D26] 数组转字符串
来源：http://nxp.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://yhz.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://gsu.yanxiufei.cn

JS:   arr.join(", ")
来源：http://aqs.quarkkingdee.top

TS:   arr.join(", ")
来源：http://mkn.zhoulong.xyz

Java: String.join(", ", list)
来源：http://xdw.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://rri.tianlin.xyz

Ruby: arr.join(", ")
来源：http://jeo.fehbvm.com

C#:   string.Join(", ", list)
来源：http://ded.hysaishi.cn

================================================================================
来源：http://ngv.smart0.xyz

E. 字符串处理
来源：http://got.chenzaomai.com

================================================================================
来源：http://jvp.jinqigfzy.top

[E01] 拼接字符串
来源：http://zut.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wrk.shanyushiyangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hic.ivvv.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://emi.yuxming.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yzp.jinghuilouyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sou.sjlbkw.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tgk.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nww.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gwf.yuxming.cn

[E02] 重复字符串
来源：http://daw.cqqwz.cn

Py:   "ab" * 3
来源：http://atk.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://vqy.daxiang520.top

JS:   "ab".repeat(3)
来源：http://bqx.pycfn.com

TS:   "ab".repeat(3)
来源：http://suj.ivvv.top

Java: "ab".repeat(3)
来源：http://san.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://bgk.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://wtv.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hmx.tarul.cn

[E03] 截取子串
来源：http://uyh.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://akw.wangdashe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wwy.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kzl.yonumen.top

TS:   s.slice(1, 4)
来源：http://mnz.aizwys.cn

Java: s.substring(1, 4)
来源：http://qyr.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://amt.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://hbt.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://arh.zhengqikj.top

[E04] 查找子串位置
来源：http://gdc.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://fmh.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://yue.aibaodan.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ltq.zhaomingkeji.xyz

TS:   s.indexOf("x")
来源：http://oqz.xinyue.icu

Java: s.indexOf("x")
来源：http://ivp.nanxinkj.top

Go:   strings.Index(s, "x")
来源：http://wto.0kj1m.cn

Ruby: s.index("x")
来源：http://ouc.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://ibv.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fde.316326.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sdi.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cue.meibo888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sfv.zhaomingkeji.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://bso.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ati.fehbvm.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sij.jqgufenzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lnc.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jda.chenlongwang.top

[E06] 替换子串
来源：http://qgf.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ogv.aizwys.cn

PHP:  str_replace("a", "b", $s);
来源：http://bsn.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qhg.kuanghao11.cn

TS:   s.replaceAll("a", "b")
来源：http://twi.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fdt.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://icq.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dbk.yongpay.top

C#:   s.Replace("a", "b")
来源：http://aqs.fzhhl.top

[E07] 按分隔符拆分
来源：http://exb.tanke756.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ccb.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yti.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ypd.iojbl.cn

TS:   s.split(",")
来源：http://gqm.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://tpq.tian-w.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://knr.fktsv.cn

Ruby: s.split(",");  s.split
来源：http://tew.ydzc1.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yuk.chenzaomai.com

[E08] 数组按分隔符合并
来源：http://yhh.fzhhl.top

Py:   ",".join(items)
来源：http://fha.jqgufenzy.top

PHP:  implode(",", $items);
来源：http://yul.9152youxi.cn

JS:   items.join(",")
来源：http://lqq.sxryk.cn

TS:   items.join(",")
来源：http://mwt.yj20258888.top

Java: String.join(",", items)
来源：http://abe.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://kao.aizwys.cn

Ruby: items.join(",")
来源：http://kht.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://tus.ydjk.org.cn

[E09] 去除所有空白字符
来源：http://zhi.xuanzx.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://atk.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dew.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://dfb.xingfuxueyuan.xyz

TS:   s.replace(/\s+/g, "")
来源：http://nxx.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://efo.birdmap.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kdm.wangdashe.top

Ruby: s.gsub(/\s+/, "")
来源：http://cvk.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lxr.zhongyouzk.top

[E10] 左侧补零 / 定长填充
来源：http://cgm.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://biu.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bfl.gzhubu.top

JS:   "7".padStart(3, "0")
来源：http://edw.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://fgj.shangyingyoupin.top

Java: String.format("%03d", 7)
来源：http://gmb.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rhb.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://npq.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bwn.9152youxi.cn

[E11] 反转字符串
来源：http://phj.shzxlz.cn

Py:   s[::-1]
来源：http://auo.jinyuanbaomall.cn

PHP:  strrev($s);
来源：http://jbz.gogol.net.cn

JS:   [...s].reverse().join("")
来源：http://ybu.jinqigufen.top

TS:   [...s].reverse().join("")
来源：http://gnx.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xjo.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vcp.jinqigufen.top

Ruby: s.reverse
来源：http://mvf.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://rxt.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://uqf.guannengcc.top

Py:   s.count("a")
来源：http://zyn.jinqigfzy.top

PHP:  substr_count($s, "a");
来源：http://szc.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://ald.yj202588.top

TS:   s.split("a").length - 1
来源：http://ric.hnxiangtu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fjp.hammf.cn

Go:   strings.Count(s, "a")
来源：http://ovy.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://raa.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://cxf.shanyushiyangtech.top

[E13] 逐字符遍历
来源：http://wzc.jinqigufen.top

Py:   for ch in s: print(ch)
来源：http://mvd.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mtq.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wio.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fod.vqdsnc.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dem.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pnq.haohaochexian.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lrw.jinghuilouyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tlv.nanxuanxn.top

[E14] URL 编码与 Base64
来源：http://spi.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kgy.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fjy.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jto.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ann.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://krf.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jye.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wdx.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tvt.sweek.top

[E15] HTML 转义 / 反转义
来源：http://xxd.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dta.hammf.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jwt.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gsv.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nmg.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bou.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rhp.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nnd.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dsl.shanyushiyangtech.top

[E16] 数字千分位
来源：http://qio.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://gyk.feifeiyinyue.top

PHP:  number_format(1234567);
来源：http://mhd.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://avq.bjfxy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ggo.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sbr.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://spx.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nlz.daria6918.cn

C#:   1234567.ToString("N0")
来源：http://bvu.zhiwuduotai.top

[E17] 首字母大写
来源：http://iyi.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dso.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jxz.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bpq.nwbrower.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zbc.wangshuangyany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jbm.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://llx.cheryme.top

Ruby: s.capitalize
来源：http://rnu.jqgufenzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wqm.cucudq.cn

[E18] 模板占位符替换
来源：http://mjh.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bor.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gyd.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fdt.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jbp.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ucn.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://czi.gogol.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ick.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yhi.9152youxi.cn

[E19] 多行文本按行拆分
来源：http://els.nanxuanxn.top

Py:   s.splitlines()
来源：http://exy.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fxn.zhengqikj.top

JS:   s.split(/\r?\n/)
来源：http://mht.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://zpw.dianchejie.cn

Java: s.lines().toList()
来源：http://wwr.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://idw.chenlongwang.top

Ruby: s.lines
来源：http://yki.birdmap.top

C#:   s.Split('\n')
来源：http://amw.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://edr.shangyingyoupin.top

Py:   if not s:
来源：http://pju.xylfe.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uih.wangshuangyany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bxs.uphjek.com

TS:   if (s === "") {}
来源：http://pws.sweek.top

Java: if (s.isEmpty()) {}
来源：http://ykk.yueranfly.top


<!-- 参考信息 -->