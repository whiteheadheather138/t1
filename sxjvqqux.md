代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tpy.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qxt.hywenlv.cn

JS:   arr.map(x => x * 2)
来源：http://vdn.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://tpe.pengpengdd.cyou

Java: list.stream().map(x -> x * 2).toList()
来源：http://qym.cheryme.top

Go:   // 手写循环
来源：http://esi.aizwys.cn

Ruby: arr.map { |x| x * 2 }
来源：http://czo.shzxlz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://avx.ywan-chungtsiang.top

[D15] 去重
来源：http://gaw.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://txf.daxiang520.top

PHP:  array_unique($arr);
来源：http://vds.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://zvu.pycfn.com

TS:   [...new Set(arr)]
来源：http://pux.sufxvd.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lid.shanyushiyangtech.top

Go:   // 用 map[T]struct{} 手写
来源：http://bkb.mhx1999.top

Ruby: arr.uniq
来源：http://inz.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://upp.zhengqikj.top

[D16] 求和与平均值
来源：http://ppx.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hwi.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xfj.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ewd.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qls.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tiw.xuetiantiany.cn

Go:   // 手写循环累加
来源：http://cia.vehdjk.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jfh.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://txu.haohaochexian.top

[D17] 最大值与最小值
来源：http://nmo.fanxiaobao.xyz

Py:   max(arr);  min(arr)
来源：http://gjc.ywan-chungtsiang.top

PHP:  max($arr);  min($arr);
来源：http://taa.nwbrower.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gng.jiagoushi.top

TS:   Math.max(...arr);
来源：http://pmi.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://swp.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mct.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://wah.c1oappe.top

C#:   list.Max();  list.Min()
来源：http://pyo.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://lrl.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wtk.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://zcq.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qsk.snrcjt.cn

TS:   nested.flat();
来源：http://fgk.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bck.chenjidiqi.icu

Go:   // 手写双层循环
来源：http://fhk.yfazqb.com

Ruby: nested.flatten
来源：http://znp.pengpengdd.cyou

C#:   nested.SelectMany(x => x).ToList()
来源：http://kay.jqgufenzy.top

[D19] 按字段分组
来源：http://mfo.fehbvm.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zmv.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cjp.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qhw.ydzc1.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vrx.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pdy.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://aky.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://uma.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eko.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://gxc.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://qrd.ivvv.top

PHP:  array_count_values($arr);
来源：http://eky.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xak.bjfxy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yty.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mao.feifeiyinyue.top

Go:   // 手写 map[T]int
来源：http://zkb.epnwcf.com

Ruby: arr.tally
来源：http://gjj.yueranfly.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tdy.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://qhu.zhijiandao.cn

Py:   x in arr
来源：http://ire.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://yci.52xcode.cn

JS:   arr.includes(x)
来源：http://xcu.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://jbe.zhixingplan.top

Java: list.contains(x)
来源：http://hna.vehdjk.com

Go:   slices.Contains(arr, x)
来源：http://bcf.uphjek.com

Ruby: arr.include?(x)
来源：http://zdg.sxryk.cn

C#:   list.Contains(x)
来源：http://uoc.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://hmv.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tad.dashuyun.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mhm.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lzq.hongshengwenyu.top

TS:   [...arr];
来源：http://vov.aibaodan.cn

Java: new ArrayList<>(list);
来源：http://cut.pengpengdd.cyou

Go:   copied := append([]int(nil), arr...)
来源：http://mlt.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://mli.daxiang520.top

C#:   new List<int>(list);
来源：http://gmk.chenlongwang.top

[D23] reduce 累积计算
来源：http://sda.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kuo.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hxg.andypj.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xcs.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tgs.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://fpp.jiagoushi.top

Go:   // 手写循环
来源：http://glb.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://raz.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nct.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://gav.zhixingplan.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lij.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uxk.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sjv.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iln.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vhw.quarkkingdee.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://waa.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jxs.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://npa.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://pmk.fehbvm.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qcp.hammf.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kgn.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fhw.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hgc.chenlongwang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sdk.nanxinkj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vsr.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lxl.nwbrower.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://egl.uphjek.com

[D26] 数组转字符串
来源：http://nyz.tian-w.cn

Py:   ", ".join(map(str, arr))
来源：http://hpb.ehwqpu.com

PHP:  implode(", ", $arr);
来源：http://emj.hnqzz.top

JS:   arr.join(", ")
来源：http://avo.cheryme.top

TS:   arr.join(", ")
来源：http://wpu.jiagoushi.top

Java: String.join(", ", list)
来源：http://cep.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://xuw.ppjwa.cn

Ruby: arr.join(", ")
来源：http://kje.ctjpmb.com

C#:   string.Join(", ", list)
来源：http://tsw.andypj.xyz

================================================================================
来源：http://emy.yonumen.top

E. 字符串处理
来源：http://nlm.hywenlv.cn

================================================================================
来源：http://abu.ctjpmb.com

[E01] 拼接字符串
来源：http://sap.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dly.hammf.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bhl.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ppa.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pcu.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fia.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xnb.iojbl.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xbv.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zfo.zdqjudy.top

[E02] 重复字符串
来源：http://vli.cqqwz.cn

Py:   "ab" * 3
来源：http://uom.cucudq.cn

PHP:  str_repeat("ab", 3);
来源：http://mhs.uphjek.com

JS:   "ab".repeat(3)
来源：http://hix.ybcxt.top

TS:   "ab".repeat(3)
来源：http://dhf.tian-w.cn

Java: "ab".repeat(3)
来源：http://ycq.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://yma.dianchejie.cn

Ruby: "ab" * 3
来源：http://ldh.hesvh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kga.zhiwuduotai.top

[E03] 截取子串
来源：http://jiy.tarul.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zcz.tarul.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rzl.jlsjyb.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ean.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://tsx.yonumen.top

Java: s.substring(1, 4)
来源：http://ewz.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gdr.zhiwuduotai.top

Ruby: s[1, 3];  s[1..3]
来源：http://vkv.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://dhf.daria6918.cn

[E04] 查找子串位置
来源：http://byc.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://bio.sysykeji.top

PHP:  strpos($s, "x");
来源：http://npb.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wab.jyoumei.cn

TS:   s.indexOf("x")
来源：http://xpz.ybcxt.top

Java: s.indexOf("x")
来源：http://xis.ehwqpu.com

Go:   strings.Index(s, "x")
来源：http://qao.xinyue.icu

Ruby: s.index("x")
来源：http://xvk.yj20258.top

C#:   s.IndexOf("x")
来源：http://qve.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cnh.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://urx.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mzy.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nlw.tarul.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iej.hammf.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zgd.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pvq.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yjt.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sqm.meibo888.top

[E06] 替换子串
来源：http://osy.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://umh.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://emz.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://czc.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://iui.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eyx.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dzu.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qfa.bbcook.cn

C#:   s.Replace("a", "b")
来源：http://mrx.yonumen.top

[E07] 按分隔符拆分
来源：http://oom.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ewn.snrcjt.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wuv.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://afd.hesvh.cn

TS:   s.split(",")
来源：http://vmt.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://cmd.zycfv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ejr.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://uqe.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://njt.zhoulong.xyz

[E08] 数组按分隔符合并
来源：http://slm.fktsv.cn

Py:   ",".join(items)
来源：http://iec.shzxlz.cn

PHP:  implode(",", $items);
来源：http://iuw.vehdjk.com

JS:   items.join(",")
来源：http://ybh.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://xwa.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://szz.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://rqg.snrcjt.cn

Ruby: items.join(",")
来源：http://ryt.yj202588.top

C#:   string.Join(",", items)
来源：http://lmk.guowangkeji.top

[E09] 去除所有空白字符
来源：http://bff.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ucn.guannengcc.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zds.hysaishi.cn

JS:   s.replace(/\s+/g, "")
来源：http://qxg.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://uef.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://gli.xinyue.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://qoi.chenlongwang.top

Ruby: s.gsub(/\s+/, "")
来源：http://kln.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oiq.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://qif.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://shi.52xcode.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aym.birdmap.top

JS:   "7".padStart(3, "0")
来源：http://qza.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://jwr.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://oay.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://exf.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fqm.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kaa.ydjk.org.cn

[E11] 反转字符串
来源：http://qbj.daria6918.cn

Py:   s[::-1]
来源：http://usq.sufxvd.cn

PHP:  strrev($s);
来源：http://jgp.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://slu.tianlin.xyz

TS:   [...s].reverse().join("")
来源：http://dbd.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mef.gogol.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rmt.yongpay.top

Ruby: s.reverse
来源：http://ibh.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ejl.bbcook.cn

[E12] 统计某字符出现次数
来源：http://nbc.mhx1999.top

Py:   s.count("a")
来源：http://guq.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://itb.cucudq.cn

JS:   s.split("a").length - 1
来源：http://cmi.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://wou.sxryk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rav.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://csn.yanxiufei.cn

Ruby: s.count("a")
来源：http://udr.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://vjv.sjlbkw.cn

[E13] 逐字符遍历
来源：http://svi.xziqi.cn

Py:   for ch in s: print(ch)
来源：http://wsl.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vdx.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nhm.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xzz.yvedp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lws.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ebw.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lth.wangshuangyany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wwf.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://wcp.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qck.shzxlz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sau.shuidangran.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jyn.kuanghao11.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xkx.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dre.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ald.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://izw.yonumen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cnc.zycfv.cn

[E15] HTML 转义 / 反转义
来源：http://fjq.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://prb.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ihr.yj20258888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uwd.feifeiyinyue.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ocs.hongshengwenyu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rha.xuanzx.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aaq.ivvv.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ofh.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hhd.ehwqpu.com

[E16] 数字千分位
来源：http://oys.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://vnj.feifeiyinyue.top

PHP:  number_format(1234567);
来源：http://nkj.cashguo.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ogy.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://kvq.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qyn.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iac.chenjidiqi.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hes.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://sxv.jqgufenzy.top

[E17] 首字母大写
来源：http://bav.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vgq.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pmv.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xoj.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lqr.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tkq.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tyx.jqgfzy.top

Ruby: s.capitalize
来源：http://xpq.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jax.iojbl.cn

[E18] 模板占位符替换
来源：http://fvw.wangdashe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gqn.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ztf.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://lqm.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://glx.epnwcf.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pqh.zhijiandao.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ynx.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oqe.sxryk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zrs.svipenyu.cn

[E19] 多行文本按行拆分
来源：http://jgq.pengpengdd.cyou

Py:   s.splitlines()
来源：http://czt.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ydm.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://sfu.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://kdf.yj20258888.top

Java: s.lines().toList()
来源：http://uff.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://cri.52xcode.cn

Ruby: s.lines
来源：http://niu.tian-w.cn

C#:   s.Split('\n')
来源：http://hzo.aizwys.cn

[E20] 判断字符串是否为空
来源：http://mpo.zhiwuduotai.top

Py:   if not s:
来源：http://mzq.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://otk.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qiz.bjfxy.top

TS:   if (s === "") {}
来源：http://dkk.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://enw.gotoacloud.top

Go:   if s == "" {}
来源：http://gcz.tian-w.cn

Ruby: if s.empty?
来源：http://iis.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lmo.nanxuanxn.top

[E21] 超长截断加省略号
来源：http://rvk.andypj.xyz


<!-- 参考信息 -->