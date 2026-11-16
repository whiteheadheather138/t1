代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vqj.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://cam.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://rjh.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://bmi.c1oappe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wih.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fwv.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://zuv.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://pzx.haohaochexian.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://utu.fktsv.cn

Go:   // 手写循环
来源：http://jvl.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://eqe.xuanzx.com

C#:   list.Select(x => x * 2).ToList()
来源：http://uvc.zhoulong.xyz

[D15] 去重
来源：http://unl.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mzl.ivvv.top

PHP:  array_unique($arr);
来源：http://izy.meibo888.top

JS:   [...new Set(arr)]
来源：http://ict.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://egy.xuanzx.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yxj.bjfxy.top

Go:   // 用 map[T]struct{} 手写
来源：http://hwx.daxiang520.top

Ruby: arr.uniq
来源：http://lxg.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://llo.sufxvd.cn

[D16] 求和与平均值
来源：http://kdn.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ojk.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://etu.aizwys.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://htd.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vzr.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ywk.yongpay.top

Go:   // 手写循环累加
来源：http://vgo.zhoulong.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zsv.shanyushiyangtech.top

C#:   list.Sum();  list.Average()
来源：http://ico.zhixingplan.top

[D17] 最大值与最小值
来源：http://nfm.yj20258.top

Py:   max(arr);  min(arr)
来源：http://zud.jinyuanbaomall.cn

PHP:  max($arr);  min($arr);
来源：http://bnc.feifeiyinyue.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ktj.yongpay.top

TS:   Math.max(...arr);
来源：http://mzb.shuidangran.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bzm.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qlj.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://qyp.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://wxt.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://kec.epnwcf.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qyw.gogol.net.cn

PHP:  array_merge(...$nested);
来源：http://igy.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://puh.feifeiyinyue.top

TS:   nested.flat();
来源：http://uwz.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://job.shanyushiyangtech.top

Go:   // 手写双层循环
来源：http://ntq.daxiang520.top

Ruby: nested.flatten
来源：http://rwy.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://zai.c1oappe.top

[D19] 按字段分组
来源：http://jzu.pengpengdd.cyou

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pbc.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ksg.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uwg.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://azv.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zql.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://wdy.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://htf.bbcook.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bkv.chenzaomai.com

[D20] 统计每个元素出现次数
来源：http://tvo.fehbvm.com

Py:   Counter(arr)
来源：http://lyu.zhoulong.xyz

PHP:  array_count_values($arr);
来源：http://pdo.shanyushiyangtech.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://siw.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dfx.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://brf.gotoacloud.top

Go:   // 手写 map[T]int
来源：http://qfu.xingfuxueyuan.xyz

Ruby: arr.tally
来源：http://ftm.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://msk.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://lek.zycfv.cn

Py:   x in arr
来源：http://zbx.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://bon.hfpthk.cn

JS:   arr.includes(x)
来源：http://aaq.pycfn.com

TS:   arr.includes(x)
来源：http://qnm.sufxvd.cn

Java: list.contains(x)
来源：http://hbm.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://xyz.vehdjk.com

Ruby: arr.include?(x)
来源：http://ymk.epnwcf.com

C#:   list.Contains(x)
来源：http://pfl.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://guj.fehbvm.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oks.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vwy.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dqj.jlsjyb.cn

TS:   [...arr];
来源：http://uss.redwolf501.top

Java: new ArrayList<>(list);
来源：http://lok.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uhe.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://wbh.zhoulong.xyz

C#:   new List<int>(list);
来源：http://iuv.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://mfr.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ifj.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sip.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ydg.jinqigfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bwc.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://sts.ehwqpu.com

Go:   // 手写循环
来源：http://gbk.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xkk.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wgl.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://vlz.xingfuxueyuan.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wwp.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://thv.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ceg.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iux.svipenyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qty.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hfm.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zqw.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ltn.bbcook.cn

[D25] Set 集合去重与交并差
来源：http://dxf.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lme.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fth.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://unh.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sgr.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://adu.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nuz.sxryk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wse.ydjk.org.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qrd.ivvv.top

[D26] 数组转字符串
来源：http://qfy.jinghuilouyu.cn

Py:   ", ".join(map(str, arr))
来源：http://wma.cqqwz.cn

PHP:  implode(", ", $arr);
来源：http://bsu.jinqigfzy.top

JS:   arr.join(", ")
来源：http://uau.fanxiaobao.xyz

TS:   arr.join(", ")
来源：http://unq.yangfankeji.com

Java: String.join(", ", list)
来源：http://slu.zdbjq.cn

Go:   strings.Join(strs, ", ")
来源：http://qhp.cqqwz.cn

Ruby: arr.join(", ")
来源：http://eel.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://qiv.guannengcc.top

================================================================================
来源：http://ctt.shzxlz.cn

E. 字符串处理
来源：http://mlh.redwolf501.top

================================================================================
来源：http://dhw.cashguo.top

[E01] 拼接字符串
来源：http://efh.chenjidiqi.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xaq.daria6918.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eux.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tlz.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sge.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lbt.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fvz.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sib.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gnu.shuidangran.top

[E02] 重复字符串
来源：http://juj.hesvh.cn

Py:   "ab" * 3
来源：http://ska.cashguo.top

PHP:  str_repeat("ab", 3);
来源：http://grr.daxiang520.top

JS:   "ab".repeat(3)
来源：http://wak.hfpthk.cn

TS:   "ab".repeat(3)
来源：http://hau.aibaodan.cn

Java: "ab".repeat(3)
来源：http://slu.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://zgi.ydzc1.top

Ruby: "ab" * 3
来源：http://ywq.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eea.aizwys.cn

[E03] 截取子串
来源：http://tos.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kag.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gcn.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fvr.daxiang520.top

TS:   s.slice(1, 4)
来源：http://luy.ivvv.top

Java: s.substring(1, 4)
来源：http://fsh.jyoumei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dpr.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://bgn.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://czy.tarul.cn

[E04] 查找子串位置
来源：http://syb.yanxiufei.cn

Py:   s.find("x");  s.index("x")
来源：http://kml.jyoumei.cn

PHP:  strpos($s, "x");
来源：http://vhu.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rmc.sweek.top

TS:   s.indexOf("x")
来源：http://hcd.mhx1999.top

Java: s.indexOf("x")
来源：http://sha.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://hmu.fehbvm.com

Ruby: s.index("x")
来源：http://pfz.tian-w.cn

C#:   s.IndexOf("x")
来源：http://jyx.iojbl.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://khc.hywenlv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://skx.hcnkem.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vvl.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kgz.tarul.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://khr.zhixingplan.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://edr.xziqi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ojy.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lqm.yanxiufei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://czc.zhixingplan.top

[E06] 替换子串
来源：http://udm.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oyx.tarul.cn

PHP:  str_replace("a", "b", $s);
来源：http://ljr.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eko.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://vcq.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pit.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rzi.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fgz.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://vny.epnwcf.com

[E07] 按分隔符拆分
来源：http://jkz.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pvl.zhoulong.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qdf.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://zwy.ywan-chungtsiang.top

TS:   s.split(",")
来源：http://qoi.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://kwa.meibo888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rrn.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://mdp.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://crs.yuxming.cn

[E08] 数组按分隔符合并
来源：http://jzj.aibaodan.cn

Py:   ",".join(items)
来源：http://gpq.cucudq.cn

PHP:  implode(",", $items);
来源：http://xdr.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://hij.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://dwq.xylfe.cn

Java: String.join(",", items)
来源：http://pib.zhaomingkeji.xyz

Go:   strings.Join(items, ",")
来源：http://drd.jlsjyb.cn

Ruby: items.join(",")
来源：http://dqa.meibo888.top

C#:   string.Join(",", items)
来源：http://ghv.yuanzhike.top

[E09] 去除所有空白字符
来源：http://lkb.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ogh.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://igy.zdbjq.cn

JS:   s.replace(/\s+/g, "")
来源：http://ppe.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://xkx.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://hui.yuxming.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yll.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://awf.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bji.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://dbl.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sju.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tsn.ivvv.top

JS:   "7".padStart(3, "0")
来源：http://rfp.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://wzl.tarul.cn

Java: String.format("%03d", 7)
来源：http://bxc.52xcode.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fcn.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nnw.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dsh.jinghuilouyu.cn

[E11] 反转字符串
来源：http://cqg.kuanghao11.cn

Py:   s[::-1]
来源：http://nnl.feifeiyinyue.top

PHP:  strrev($s);
来源：http://dlf.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://ywx.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://ghp.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wrz.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cky.zycfv.cn

Ruby: s.reverse
来源：http://ptf.uphjek.com

C#:   new string(s.Reverse().ToArray())
来源：http://puz.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://oie.fehbvm.com

Py:   s.count("a")
来源：http://qgw.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://tsv.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://imy.ivvv.top

TS:   s.split("a").length - 1
来源：http://pin.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sgy.yj20258888.top

Go:   strings.Count(s, "a")
来源：http://uao.zhiwuduotai.top

Ruby: s.count("a")
来源：http://rrd.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://rge.zhengqikj.top

[E13] 逐字符遍历
来源：http://emu.birdmap.top

Py:   for ch in s: print(ch)
来源：http://nes.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qia.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://ptf.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zem.ivvv.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ixj.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://goj.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uzl.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ikg.yj20258.top

[E14] URL 编码与 Base64
来源：http://teu.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xmk.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://gyk.hcnkem.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nto.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mig.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mgu.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wfb.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pfx.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hed.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://ypd.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lnc.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://szu.yj20258.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://azn.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uxi.fktsv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vve.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qbn.xziqi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rzs.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kcm.sweek.top

[E16] 数字千分位
来源：http://coj.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://btd.chenlongwang.top

PHP:  number_format(1234567);
来源：http://hpn.aizwys.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://stc.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vwp.gotoacloud.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xaj.birdmap.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://isv.cqqwz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aqt.yonumen.top

C#:   1234567.ToString("N0")
来源：http://rxf.hcnkem.com

[E17] 首字母大写
来源：http://plo.gzhubu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nvj.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://cah.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dyh.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hah.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wbg.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://evq.andypj.xyz

Ruby: s.capitalize
来源：http://wha.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xdr.c1oappe.top

[E18] 模板占位符替换
来源：http://ygc.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oru.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tzi.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vvy.sweek.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ttq.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://utq.jqgufenzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ecl.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fyv.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xvm.fktsv.cn

[E19] 多行文本按行拆分
来源：http://iym.ctjpmb.com

Py:   s.splitlines()
来源：http://exe.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nvc.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://xht.cdnleiting.top

TS:   s.split(/\r?\n/)
来源：http://ttf.guowangkeji.top

Java: s.lines().toList()
来源：http://pcv.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://nta.vqdsnc.cn

Ruby: s.lines
来源：http://tcq.zdqjudy.top

C#:   s.Split('\n')
来源：http://mrw.52xcode.cn

[E20] 判断字符串是否为空
来源：http://rpq.kuanghao11.cn

Py:   if not s:
来源：http://acd.52xcode.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iwx.zdqjudy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://epe.jlsjyb.cn

TS:   if (s === "") {}
来源：http://tqc.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://vub.nwbrower.top


<!-- 参考信息 -->