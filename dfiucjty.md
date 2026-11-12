代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uhx.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://dxd.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://dbv.sxryk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vsw.c1oappe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nbv.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://kek.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qbo.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://jwu.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hfa.hfpthk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qaa.ctjpmb.com

JS:   arr.map(x => x * 2)
来源：http://wbf.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://njt.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uqy.zycfv.cn

Go:   // 手写循环
来源：http://zaj.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fsd.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nmv.mhx1999.top

[D15] 去重
来源：http://heo.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hgt.gogol.net.cn

PHP:  array_unique($arr);
来源：http://vgw.fzhhl.top

JS:   [...new Set(arr)]
来源：http://iij.aizwys.cn

TS:   [...new Set(arr)]
来源：http://bze.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pdk.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dcy.shuidangran.top

Ruby: arr.uniq
来源：http://gzc.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://okw.yanxiufei.cn

[D16] 求和与平均值
来源：http://hss.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://deq.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eyg.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zfd.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mcn.zdbjq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zlz.tianlin.xyz

Go:   // 手写循环累加
来源：http://yqi.vqdsnc.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jgk.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://hhz.shzxlz.cn

[D17] 最大值与最小值
来源：http://spy.sweek.top

Py:   max(arr);  min(arr)
来源：http://agq.havefunace.top

PHP:  max($arr);  min($arr);
来源：http://rfw.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dpm.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://scq.quarkkingdee.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tmt.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gas.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://lhi.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://tcj.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://jem.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vzq.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://luw.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mtr.svipenyu.cn

TS:   nested.flat();
来源：http://aai.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vzw.haohaochexian.top

Go:   // 手写双层循环
来源：http://dqj.nwbrower.top

Ruby: nested.flatten
来源：http://vxq.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nnj.daria6918.cn

[D19] 按字段分组
来源：http://dfd.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vdy.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fwu.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xzy.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eyd.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mbc.cucudq.cn

Go:   // 手写 map[string][]T
来源：http://aip.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ycy.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fgd.hammf.cn

[D20] 统计每个元素出现次数
来源：http://yfb.aibaodan.cn

Py:   Counter(arr)
来源：http://rnw.tarul.cn

PHP:  array_count_values($arr);
来源：http://mup.chenlongwang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ubn.ybcxt.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cxs.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pcr.redwolf501.top

Go:   // 手写 map[T]int
来源：http://ydy.redwolf501.top

Ruby: arr.tally
来源：http://okz.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xgr.zhijiandao.cn

[D21] 判断是否包含某元素
来源：http://wno.xuetiantiany.cn

Py:   x in arr
来源：http://hqw.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://gzy.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://ewe.andypj.xyz

TS:   arr.includes(x)
来源：http://tpd.zhixingplan.top

Java: list.contains(x)
来源：http://lxd.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://yon.pengpengdd.cyou

Ruby: arr.include?(x)
来源：http://xdl.havefunace.top

C#:   list.Contains(x)
来源：http://tvk.zhaomingkeji.xyz

[D22] 复制数组（避免共享引用）
来源：http://nfi.bbcook.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pqj.xinyue.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bbd.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vxo.xinyue.icu

TS:   [...arr];
来源：http://nsz.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://oqr.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://pxe.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://xgk.fktsv.cn

C#:   new List<int>(list);
来源：http://gxp.xziqi.cn

[D23] reduce 累积计算
来源：http://yzr.yuanzhike.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qki.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bos.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wuj.gogol.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ffe.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gnx.yangfankeji.com

Go:   // 手写循环
来源：http://sqf.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vfk.jinghuilouyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tsq.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://mqh.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://siy.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tay.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pis.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mor.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fwj.jinyuanbaomall.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qel.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jde.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zce.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://pqi.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bdv.svipenyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bqs.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://szg.cdnleiting.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zsw.chenjidiqi.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://slu.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rpg.pycfn.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eot.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ear.yueranfly.top

[D26] 数组转字符串
来源：http://jeb.52xcode.cn

Py:   ", ".join(map(str, arr))
来源：http://goa.yj20258.top

PHP:  implode(", ", $arr);
来源：http://jgx.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://lwl.yueranfly.top

TS:   arr.join(", ")
来源：http://agg.nanxuanxn.top

Java: String.join(", ", list)
来源：http://cvp.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://uua.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://ofy.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://uby.xuanzx.com

================================================================================
来源：http://igb.hfpthk.cn

E. 字符串处理
来源：http://jqq.chenzaomai.com

================================================================================
来源：http://xhg.yangfankeji.com

[E01] 拼接字符串
来源：http://afm.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cwb.fengsongda.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tau.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tew.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pyc.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sjs.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kvw.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kfc.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qwm.fanxiaobao.xyz

[E02] 重复字符串
来源：http://gld.guowangkeji.top

Py:   "ab" * 3
来源：http://tnt.xziqi.cn

PHP:  str_repeat("ab", 3);
来源：http://kkr.nwbrower.top

JS:   "ab".repeat(3)
来源：http://chy.fzhhl.top

TS:   "ab".repeat(3)
来源：http://wsy.haohaochexian.top

Java: "ab".repeat(3)
来源：http://ftp.yuanzhike.top

Go:   strings.Repeat("ab", 3)
来源：http://uep.bbcook.cn

Ruby: "ab" * 3
来源：http://wfw.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bej.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://lug.havefunace.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jjc.yfazqb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ika.jianghu66.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zyp.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://hrb.yfazqb.com

Java: s.substring(1, 4)
来源：http://kep.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uwj.yj20258.top

Ruby: s[1, 3];  s[1..3]
来源：http://jyk.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://jyc.gogol.net.cn

[E04] 查找子串位置
来源：http://uth.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://yfb.svipenyu.cn

PHP:  strpos($s, "x");
来源：http://syb.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ayg.chenjidiqi.icu

TS:   s.indexOf("x")
来源：http://dky.tarul.cn

Java: s.indexOf("x")
来源：http://vjn.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://ddc.jqgfzy.top

Ruby: s.index("x")
来源：http://bda.hongshengwenyu.top

C#:   s.IndexOf("x")
来源：http://yhj.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://vbz.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cjc.havefunace.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://crh.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iqq.jinqigufen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lmr.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mjj.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ulj.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mxk.pycfn.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ybu.fzhhl.top

[E06] 替换子串
来源：http://zxz.cqqwz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jia.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://qfk.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tot.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://jwr.tian-w.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rwf.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ezb.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iuz.havefunace.top

C#:   s.Replace("a", "b")
来源：http://nun.zycfv.cn

[E07] 按分隔符拆分
来源：http://ehy.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bsb.yvedp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xqc.pycfn.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://rdc.yuanzhike.top

TS:   s.split(",")
来源：http://ttd.tian-w.cn

Java: s.split(",");  s.split("\\s+")
来源：http://omi.xuanzx.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rjm.jyoumei.cn

Ruby: s.split(",");  s.split
来源：http://mpq.zycfv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nps.zhoulong.xyz

[E08] 数组按分隔符合并
来源：http://tso.hongshengwenyu.top

Py:   ",".join(items)
来源：http://liq.hnqzz.top

PHP:  implode(",", $items);
来源：http://acu.hfpthk.cn

JS:   items.join(",")
来源：http://tyv.sweek.top

TS:   items.join(",")
来源：http://gna.havefunace.top

Java: String.join(",", items)
来源：http://zsz.ywan-chungtsiang.top

Go:   strings.Join(items, ",")
来源：http://izh.zhengqikj.top

Ruby: items.join(",")
来源：http://hsr.hcnkem.com

C#:   string.Join(",", items)
来源：http://dey.hfpthk.cn

[E09] 去除所有空白字符
来源：http://wek.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nzt.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ain.tanke756.top

JS:   s.replace(/\s+/g, "")
来源：http://daq.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://wde.andypj.xyz

Java: s.replaceAll("\\s+", "")
来源：http://jrb.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gam.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://lru.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pkj.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://wii.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xkn.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ers.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://ruf.xuetiantiany.cn

TS:   "7".padStart(3, "0")
来源：http://tta.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://lsx.wangdashe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kxq.gaohongyu789.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yup.sjlbkw.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qyy.chenlongwang.top

[E11] 反转字符串
来源：http://cfr.guannengcc.top

Py:   s[::-1]
来源：http://ysj.yj20258.top

PHP:  strrev($s);
来源：http://oen.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://sgw.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://bnf.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qaa.zdbjq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ase.guannengcc.top

Ruby: s.reverse
来源：http://tgq.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oyp.c1oappe.top

[E12] 统计某字符出现次数
来源：http://znw.redwolf501.top

Py:   s.count("a")
来源：http://xmi.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://oyq.vqdsnc.cn

JS:   s.split("a").length - 1
来源：http://npx.yonumen.top

TS:   s.split("a").length - 1
来源：http://fkf.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oza.yuanzhike.top

Go:   strings.Count(s, "a")
来源：http://naq.xuanzx.com

Ruby: s.count("a")
来源：http://flf.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://jfi.guannengcc.top

[E13] 逐字符遍历
来源：http://cim.fehbvm.com

Py:   for ch in s: print(ch)
来源：http://gku.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kgu.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tmb.andypj.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://ggr.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ads.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cgq.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jca.ybcxt.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iig.daxiang520.top

[E14] URL 编码与 Base64
来源：http://xsd.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pyx.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vbr.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zwg.jianghu66.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cyp.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vmu.jqgufenzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ugu.vehdjk.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uhf.yueranfly.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xrv.nanxuanxn.top

[E15] HTML 转义 / 反转义
来源：http://vdw.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://zlv.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qrm.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sjo.hnxiangtu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://msy.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lwm.sweek.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fzb.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kkx.52xcode.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nxs.iojbl.cn

[E16] 数字千分位
来源：http://vdh.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://vwa.daxiang520.top

PHP:  number_format(1234567);
来源：http://lpm.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eas.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xah.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zop.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oii.52xcode.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dvw.fzhhl.top

C#:   1234567.ToString("N0")
来源：http://wlm.9152youxi.cn

[E17] 首字母大写
来源：http://hbh.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gqe.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ubc.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ooi.jinqigufen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ltf.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wtf.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hnp.yonumen.top

Ruby: s.capitalize
来源：http://lyd.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yiw.ybcxt.top

[E18] 模板占位符替换
来源：http://gpq.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aox.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://isz.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xwy.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://odf.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://atl.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hhm.sxryk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tiy.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gkg.yj202588.top

[E19] 多行文本按行拆分
来源：http://qau.chenlongwang.top

Py:   s.splitlines()
来源：http://bqo.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yyy.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://kaz.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://nfv.redwolf501.top

Java: s.lines().toList()
来源：http://mra.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://hel.tanke756.top

Ruby: s.lines
来源：http://pey.xziqi.cn

C#:   s.Split('\n')
来源：http://eqc.0kj1m.cn

[E20] 判断字符串是否为空
来源：http://jgr.pengpengdd.cyou

Py:   if not s:
来源：http://dhd.aibaodan.cn


<!-- 参考信息 -->