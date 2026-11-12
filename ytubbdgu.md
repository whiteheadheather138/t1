代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://szh.fengsongda.top

JS:   arr.filter(x => x > 3)
来源：http://ifr.bjfxy.top

TS:   arr.filter(x => x > 3)
来源：http://obb.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jwe.fengsongda.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ztq.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nzl.shanyushiyangtech.top

C#:   list.Where(x => x > 3).ToList()
来源：http://epf.zhengqikj.top

[D14] 映射转换（每个元素变形）
来源：http://jor.quarkkingdee.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zfe.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mnm.jlsjyb.cn

JS:   arr.map(x => x * 2)
来源：http://qyc.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://vfz.daria6918.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fts.fktsv.cn

Go:   // 手写循环
来源：http://sbd.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://uqx.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zhh.ybcxt.top

[D15] 去重
来源：http://leg.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yti.yangfankeji.com

PHP:  array_unique($arr);
来源：http://epx.aizwys.cn

JS:   [...new Set(arr)]
来源：http://nax.smart0.xyz

TS:   [...new Set(arr)]
来源：http://gao.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pxf.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xsd.hongshengwenyu.top

Ruby: arr.uniq
来源：http://tlh.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://kbw.zdbjq.cn

[D16] 求和与平均值
来源：http://bhp.gzhubu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xoe.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://etk.yj20258888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsr.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ecz.zhiwuduotai.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://epi.bbcook.cn

Go:   // 手写循环累加
来源：http://ari.9152youxi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nkb.yfazqb.com

C#:   list.Sum();  list.Average()
来源：http://gji.zhongyouzk.top

[D17] 最大值与最小值
来源：http://xyp.sufxvd.cn

Py:   max(arr);  min(arr)
来源：http://vjn.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://pif.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xla.yfazqb.com

TS:   Math.max(...arr);
来源：http://dvv.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://jgp.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jds.guannengcc.top

Ruby: arr.max;  arr.min
来源：http://sal.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://wyj.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://klf.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mtd.9152youxi.cn

PHP:  array_merge(...$nested);
来源：http://kod.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vkr.redwolf501.top

TS:   nested.flat();
来源：http://csl.xingfuxueyuan.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://biu.jinghuilouyu.cn

Go:   // 手写双层循环
来源：http://ioa.zhiwuduotai.top

Ruby: nested.flatten
来源：http://ovw.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pll.yj202588.top

[D19] 按字段分组
来源：http://pdw.ivvv.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lsk.aizwys.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mky.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xib.yongpay.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lur.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://prw.hcnkem.com

Go:   // 手写 map[string][]T
来源：http://vbr.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://iwj.havefunace.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eom.yvedp.cn

[D20] 统计每个元素出现次数
来源：http://vzx.shuidangran.top

Py:   Counter(arr)
来源：http://tjx.mhx1999.top

PHP:  array_count_values($arr);
来源：http://vqb.iojbl.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://avz.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qvh.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vjm.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://gzh.gotoacloud.top

Ruby: arr.tally
来源：http://dhi.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://luo.chenlongwang.top

[D21] 判断是否包含某元素
来源：http://mni.zhengqikj.top

Py:   x in arr
来源：http://rlc.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://fyq.tian-w.cn

JS:   arr.includes(x)
来源：http://sxu.hfpthk.cn

TS:   arr.includes(x)
来源：http://gnq.yvedp.cn

Java: list.contains(x)
来源：http://xgg.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://wne.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://crl.xinyue.icu

C#:   list.Contains(x)
来源：http://iov.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://cdd.ehwqpu.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://twd.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gxo.zhaomingkeji.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gdc.hnxiangtu.top

TS:   [...arr];
来源：http://fkm.shanyushiyangkeji.top

Java: new ArrayList<>(list);
来源：http://kjy.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://zyl.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://tsr.0kj1m.cn

C#:   new List<int>(list);
来源：http://agh.yangfankeji.com

[D23] reduce 累积计算
来源：http://bve.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bok.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wsy.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dbe.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jnl.9152youxi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://exw.xuetiantiany.cn

Go:   // 手写循环
来源：http://xjr.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nwl.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rfy.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://rfj.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rrc.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cua.dashuyun.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mls.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wwk.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fvc.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fby.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://weu.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wva.zhongyouzk.top

[D25] Set 集合去重与交并差
来源：http://ozw.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lfr.hnqzz.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bau.sxryk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://luu.meibo888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pnr.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fkt.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iil.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ekz.guannengcc.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kmq.yuanzhike.top

[D26] 数组转字符串
来源：http://jzq.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://bwo.birdmap.top

PHP:  implode(", ", $arr);
来源：http://rxs.0kj1m.cn

JS:   arr.join(", ")
来源：http://lou.zhijiandao.cn

TS:   arr.join(", ")
来源：http://tlc.hongshengwenyu.top

Java: String.join(", ", list)
来源：http://hpi.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://vki.kuanghao11.cn

Ruby: arr.join(", ")
来源：http://gks.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://dkq.xinyue.icu

================================================================================
来源：http://wtd.yfazqb.com

E. 字符串处理
来源：http://dkh.yj20258.top

================================================================================
来源：http://wgc.epnwcf.com

[E01] 拼接字符串
来源：http://pde.dashuyun.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gey.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xfu.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wpl.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xkp.yj20258888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://skh.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://utv.cheryme.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vox.jyoumei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dru.zhixingplan.top

[E02] 重复字符串
来源：http://hss.jlsjyb.cn

Py:   "ab" * 3
来源：http://kvu.nwbrower.top

PHP:  str_repeat("ab", 3);
来源：http://wrj.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://opq.tanke756.top

TS:   "ab".repeat(3)
来源：http://sfv.aibaodan.cn

Java: "ab".repeat(3)
来源：http://lom.zhongyouzk.top

Go:   strings.Repeat("ab", 3)
来源：http://kcs.cdnleiting.top

Ruby: "ab" * 3
来源：http://mdv.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ywy.sxryk.cn

[E03] 截取子串
来源：http://ayw.pengpengdd.cyou

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dpo.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dsy.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hij.vehdjk.com

TS:   s.slice(1, 4)
来源：http://pmk.zdqjudy.top

Java: s.substring(1, 4)
来源：http://rxi.ybcxt.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://acf.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://ivx.sjlbkw.cn

C#:   s.Substring(1, 3)
来源：http://aeu.hnqzz.top

[E04] 查找子串位置
来源：http://ldd.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://mgl.hnxiangtu.top

PHP:  strpos($s, "x");
来源：http://uft.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hxu.hesvh.cn

TS:   s.indexOf("x")
来源：http://kdg.ctjpmb.com

Java: s.indexOf("x")
来源：http://zqc.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://txf.chenzaomai.com

Ruby: s.index("x")
来源：http://vql.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://egs.fanxiaobao.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://vmo.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gjw.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nwf.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qcn.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oka.yj20258888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rqj.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oht.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xjb.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xrc.sjlbkw.cn

[E06] 替换子串
来源：http://noa.zhixingplan.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cac.fehbvm.com

PHP:  str_replace("a", "b", $s);
来源：http://aao.zycfv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nge.snrcjt.cn

TS:   s.replaceAll("a", "b")
来源：http://bcx.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nvg.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pgk.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ggo.birdmap.top

C#:   s.Replace("a", "b")
来源：http://lsv.yj202588.top

[E07] 按分隔符拆分
来源：http://dyi.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hsd.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ugq.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://unr.zdqjudy.top

TS:   s.split(",")
来源：http://fbg.xingfuxueyuan.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://jbv.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bog.redwolf501.top

Ruby: s.split(",");  s.split
来源：http://dey.jyoumei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gcj.chenlongwang.top

[E08] 数组按分隔符合并
来源：http://dow.pycfn.com

Py:   ",".join(items)
来源：http://mus.uphjek.com

PHP:  implode(",", $items);
来源：http://lyh.haohaochexian.top

JS:   items.join(",")
来源：http://mjp.shangyingyoupin.top

TS:   items.join(",")
来源：http://xqa.xziqi.cn

Java: String.join(",", items)
来源：http://dmc.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://ltv.kuanghao11.cn

Ruby: items.join(",")
来源：http://dvb.dianchejie.cn

C#:   string.Join(",", items)
来源：http://ylt.9152youxi.cn

[E09] 去除所有空白字符
来源：http://tcy.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ftp.zhijiandao.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dwp.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://cvn.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://uze.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://ooe.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mck.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ipn.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://esc.sysykeji.top

[E10] 左侧补零 / 定长填充
来源：http://ojh.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jzm.jinqigufen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qpu.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://mic.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://uej.daria6918.cn

Java: String.format("%03d", 7)
来源：http://cfr.jinqigfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hhe.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cvp.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mmn.jqgfzy.top

[E11] 反转字符串
来源：http://edh.yuanzhike.top

Py:   s[::-1]
来源：http://jml.yj202588.top

PHP:  strrev($s);
来源：http://nuz.tanke756.top

JS:   [...s].reverse().join("")
来源：http://nsy.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://xah.hongshengwenyu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bzm.sufxvd.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xsh.feifeiyinyue.top

Ruby: s.reverse
来源：http://eza.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zmk.cqqwz.cn

[E12] 统计某字符出现次数
来源：http://nie.sjlbkw.cn

Py:   s.count("a")
来源：http://mwb.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://mdm.zhengqikj.top

JS:   s.split("a").length - 1
来源：http://zkv.ppjwa.cn

TS:   s.split("a").length - 1
来源：http://hfv.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ofj.cashguo.top

Go:   strings.Count(s, "a")
来源：http://qij.fktsv.cn

Ruby: s.count("a")
来源：http://xxo.xziqi.cn

C#:   s.Count(c => c == 'a')
来源：http://efi.cheryme.top

[E13] 逐字符遍历
来源：http://mmb.redwolf501.top

Py:   for ch in s: print(ch)
来源：http://gag.ehwqpu.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://agk.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jjz.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://anh.wangdashe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://afj.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xff.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sdv.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rxc.hongshengwenyu.top

[E14] URL 编码与 Base64
来源：http://iso.cucudq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uke.jyoumei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ldi.nwbrower.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ulx.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hcp.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dtb.ywan-chungtsiang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ius.cqqwz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vnx.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gca.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://bmi.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xds.ppjwa.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vqp.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mob.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://umb.jinghuilouyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://usj.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hbp.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hqb.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aoo.uphjek.com

[E16] 数字千分位
来源：http://ofx.fktsv.cn

Py:   f"{1234567:,}"
来源：http://jyb.cheryme.top

PHP:  number_format(1234567);
来源：http://cto.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://kua.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://try.mhx1999.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rqa.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kqk.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tei.nanxinkj.top

C#:   1234567.ToString("N0")
来源：http://tgj.cdnleiting.top

[E17] 首字母大写
来源：http://oup.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bio.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://umb.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://srp.tarul.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://drf.sufxvd.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fqa.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bgp.jinqigufen.top

Ruby: s.capitalize
来源：http://viu.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iri.jqgufenzy.top

[E18] 模板占位符替换
来源：http://dfh.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uwj.xingfuxueyuan.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://evc.haohaochexian.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sjr.xingfuxueyuan.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://gul.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qoj.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tgn.yj202588.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rok.shanyushiyangtech.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://orx.yuxming.cn

[E19] 多行文本按行拆分
来源：http://fve.daxiang520.top

Py:   s.splitlines()
来源：http://vgg.hnqzz.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jgz.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://nzq.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://vin.ydjk.org.cn

Java: s.lines().toList()
来源：http://pxr.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://qjr.yonumen.top

Ruby: s.lines
来源：http://koa.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://ddd.yvedp.cn

[E20] 判断字符串是否为空
来源：http://kia.dashuyun.cn

Py:   if not s:
来源：http://jtk.pengpengdd.cyou


<!-- 参考信息 -->