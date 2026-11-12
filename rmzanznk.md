代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sgf.hywenlv.cn

JS:   arr.filter(x => x > 3)
来源：http://pce.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://dvm.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oqy.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://igy.dashuyun.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zik.vqdsnc.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://iiw.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://iik.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://alv.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://viz.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://nbo.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://okx.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://vnm.xziqi.cn

Go:   // 手写循环
来源：http://izr.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://cpr.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://eup.cucudq.cn

[D15] 去重
来源：http://xna.andypj.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qfm.gaohongyu789.top

PHP:  array_unique($arr);
来源：http://bjb.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://qwn.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://frh.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jyi.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://all.xingfuxueyuan.xyz

Ruby: arr.uniq
来源：http://uzz.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://ryg.jqgufenzy.top

[D16] 求和与平均值
来源：http://brv.jinqigfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cke.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ecv.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zvl.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iky.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rdh.ivvv.top

Go:   // 手写循环累加
来源：http://guv.xuetiantiany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hdr.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://mwa.hcnkem.com

[D17] 最大值与最小值
来源：http://ufr.zhiwuduotai.top

Py:   max(arr);  min(arr)
来源：http://ssb.zhaomingkeji.xyz

PHP:  max($arr);  min($arr);
来源：http://evi.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gdh.yueranfly.top

TS:   Math.max(...arr);
来源：http://mtw.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tyz.jqgfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sbl.9152youxi.cn

Ruby: arr.max;  arr.min
来源：http://cpk.pengpengdd.cyou

C#:   list.Max();  list.Min()
来源：http://uxv.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://yrm.ybcxt.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dxc.316326.xyz

PHP:  array_merge(...$nested);
来源：http://anm.ydjk.org.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fxk.yuanzhike.top

TS:   nested.flat();
来源：http://ndm.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yvy.jinqigfzy.top

Go:   // 手写双层循环
来源：http://syw.meibo888.top

Ruby: nested.flatten
来源：http://okw.jlsjyb.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ytd.ppjwa.cn

[D19] 按字段分组
来源：http://kat.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wik.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uea.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cbq.zhengqikj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wkq.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tkk.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://gux.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cvm.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gbv.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://zwy.fktsv.cn

Py:   Counter(arr)
来源：http://qwk.vehdjk.com

PHP:  array_count_values($arr);
来源：http://bqh.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://evn.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kfk.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xgk.dashuyun.cn

Go:   // 手写 map[T]int
来源：http://xjm.fehbvm.com

Ruby: arr.tally
来源：http://iye.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jao.hammf.cn

[D21] 判断是否包含某元素
来源：http://oyk.jinghuilouyu.cn

Py:   x in arr
来源：http://hym.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://afy.cqqwz.cn

JS:   arr.includes(x)
来源：http://dtl.xuanzx.com

TS:   arr.includes(x)
来源：http://vrr.shangyingyoupin.top

Java: list.contains(x)
来源：http://njy.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://rzf.ctjpmb.com

Ruby: arr.include?(x)
来源：http://wqc.jlsjyb.cn

C#:   list.Contains(x)
来源：http://drh.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://kmy.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bsv.uphjek.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://leg.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nvv.iojbl.cn

TS:   [...arr];
来源：http://vdf.yj20258.top

Java: new ArrayList<>(list);
来源：http://ofp.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://abw.xylfe.cn

Ruby: arr.dup;  arr.clone
来源：http://zdg.c1oappe.top

C#:   new List<int>(list);
来源：http://rsa.iojbl.cn

[D23] reduce 累积计算
来源：http://ufz.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://moi.aizwys.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oaa.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vpc.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://goo.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qoy.daxiang520.top

Go:   // 手写循环
来源：http://zlb.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nzz.vehdjk.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dow.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://nyf.fzhhl.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://krf.uphjek.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ttg.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ndo.52xcode.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hkb.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xfy.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mko.xinyue.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rlh.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ptb.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://cja.c1oappe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://abc.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vwe.sxryk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vyq.aizwys.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iwy.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://whl.dashuyun.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://drg.sweek.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://faw.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rph.c1oappe.top

[D26] 数组转字符串
来源：http://tsd.bjfxy.top

Py:   ", ".join(map(str, arr))
来源：http://zqo.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://jqv.dashuyun.cn

JS:   arr.join(", ")
来源：http://gkl.sufxvd.cn

TS:   arr.join(", ")
来源：http://bmo.redwolf501.top

Java: String.join(", ", list)
来源：http://hkd.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://yta.shuidangran.top

Ruby: arr.join(", ")
来源：http://glb.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://mrd.shanyushiyangtech.top

================================================================================
来源：http://dcj.gotoacloud.top

E. 字符串处理
来源：http://fum.yonumen.top

================================================================================
来源：http://xdb.zhixingplan.top

[E01] 拼接字符串
来源：http://ovm.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mhr.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://opc.bjfxy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bai.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://giq.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wgk.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fan.yonumen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dxm.yanxiufei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://azm.ydzc1.top

[E02] 重复字符串
来源：http://opi.zdbjq.cn

Py:   "ab" * 3
来源：http://kmn.tanke756.top

PHP:  str_repeat("ab", 3);
来源：http://wip.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://ttc.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://pyc.aizwys.cn

Java: "ab".repeat(3)
来源：http://eta.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://chi.smart0.xyz

Ruby: "ab" * 3
来源：http://pvu.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ncr.epnwcf.com

[E03] 截取子串
来源：http://jel.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aaj.uphjek.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bqw.ydzc1.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ypc.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://qtq.yangfankeji.com

Java: s.substring(1, 4)
来源：http://vfe.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pnc.ppjwa.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ugp.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://fqz.ybcxt.top

[E04] 查找子串位置
来源：http://lni.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://tsu.yj20258.top

PHP:  strpos($s, "x");
来源：http://xrm.iojbl.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ywa.gogol.net.cn

TS:   s.indexOf("x")
来源：http://zsu.jyoumei.cn

Java: s.indexOf("x")
来源：http://dtw.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://hmj.hammf.cn

Ruby: s.index("x")
来源：http://kzw.9152youxi.cn

C#:   s.IndexOf("x")
来源：http://gic.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cjk.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://umf.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://byd.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jrw.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xag.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nzh.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zun.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dmu.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bbr.tianlin.xyz

[E06] 替换子串
来源：http://dus.zdqjudy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rlu.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://dxn.yonumen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gsp.yueranfly.top

TS:   s.replaceAll("a", "b")
来源：http://ibv.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ogp.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://syk.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dsx.xingfuxueyuan.xyz

C#:   s.Replace("a", "b")
来源：http://rdq.guowangkeji.top

[E07] 按分隔符拆分
来源：http://ovc.yanxiufei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rkc.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mxt.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://jvp.sweek.top

TS:   s.split(",")
来源：http://rtu.hywenlv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tzd.ydzc1.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pxb.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://vqz.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hxa.sjlbkw.cn

[E08] 数组按分隔符合并
来源：http://qya.hesvh.cn

Py:   ",".join(items)
来源：http://hrj.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://gjt.zdqjudy.top

JS:   items.join(",")
来源：http://tzf.zdqjudy.top

TS:   items.join(",")
来源：http://dst.uphjek.com

Java: String.join(",", items)
来源：http://szn.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://nuz.jlsjyb.cn

Ruby: items.join(",")
来源：http://zxr.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://bmh.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://ggg.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dqu.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kwu.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://gxs.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://nsz.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://uhq.quarkkingdee.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://emj.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hnh.daria6918.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wxz.fktsv.cn

[E10] 左侧补零 / 定长填充
来源：http://zqz.yuanzhike.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cbh.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://viw.tian-w.cn

JS:   "7".padStart(3, "0")
来源：http://cpe.yuxming.cn

TS:   "7".padStart(3, "0")
来源：http://ybl.guannengcc.top

Java: String.format("%03d", 7)
来源：http://ygy.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://fxj.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kzg.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nod.jqgfzy.top

[E11] 反转字符串
来源：http://erm.quarkkingdee.top

Py:   s[::-1]
来源：http://kxm.epnwcf.com

PHP:  strrev($s);
来源：http://jzp.yj20258.top

JS:   [...s].reverse().join("")
来源：http://glb.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://tjc.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hlh.sweek.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://bcg.quarkkingdee.top

Ruby: s.reverse
来源：http://dhv.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ein.xziqi.cn

[E12] 统计某字符出现次数
来源：http://lyv.smart0.xyz

Py:   s.count("a")
来源：http://pne.smart0.xyz

PHP:  substr_count($s, "a");
来源：http://oew.jqgufenzy.top

JS:   s.split("a").length - 1
来源：http://dey.yfazqb.com

TS:   s.split("a").length - 1
来源：http://pur.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hsl.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://psa.zycfv.cn

Ruby: s.count("a")
来源：http://jla.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://kni.hnxiangtu.top

[E13] 逐字符遍历
来源：http://dqc.9152youxi.cn

Py:   for ch in s: print(ch)
来源：http://mrl.ehwqpu.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vkm.redwolf501.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ekz.0kj1m.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kyh.hnqzz.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://miq.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wiy.haohaochexian.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yeb.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mkx.gaohongyu789.top

[E14] URL 编码与 Base64
来源：http://oov.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bzb.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://umy.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vsi.xuetiantiany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cnc.daxiang520.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ptz.wangdashe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fpp.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dst.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dsh.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://kzs.dashuyun.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://aaw.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yom.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eyg.ydjk.org.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bmn.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tou.aibaodan.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://urq.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aug.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mxb.quarkkingdee.top

[E16] 数字千分位
来源：http://yqw.jianghu66.top

Py:   f"{1234567:,}"
来源：http://rjc.ydzc1.top

PHP:  number_format(1234567);
来源：http://pnd.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yfb.quarkkingdee.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hpx.iojbl.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ofg.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rop.xylfe.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://owz.ybcxt.top

C#:   1234567.ToString("N0")
来源：http://yzt.aibaodan.cn

[E17] 首字母大写
来源：http://vax.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://npz.aibaodan.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pgx.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tht.zycfv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xug.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aeg.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://slr.smart0.xyz

Ruby: s.capitalize
来源：http://tod.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vwf.pycfn.com

[E18] 模板占位符替换
来源：http://tta.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wlt.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qqu.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://udu.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tog.svipenyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mmb.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fzv.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://red.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uze.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://iam.xuanzx.com

Py:   s.splitlines()
来源：http://dde.hfpthk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fis.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://vhc.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://cmz.ehwqpu.com

Java: s.lines().toList()
来源：http://jpy.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://uek.nwbrower.top

Ruby: s.lines
来源：http://gzz.dashuyun.cn

C#:   s.Split('\n')
来源：http://rcp.fktsv.cn

[E20] 判断字符串是否为空
来源：http://rtw.nanxuanxn.top

Py:   if not s:
来源：http://tne.hysaishi.cn


<!-- 参考信息 -->