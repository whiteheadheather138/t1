代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://sbe.wangshuangyany.cn

Go:   // 手写循环
来源：http://ldv.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fxs.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ygw.zhoulong.xyz

[D15] 去重
来源：http://vkp.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qzb.cashguo.top

PHP:  array_unique($arr);
来源：http://czl.fzhhl.top

JS:   [...new Set(arr)]
来源：http://hvp.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://lgj.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sbb.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://edx.ctjpmb.com

Ruby: arr.uniq
来源：http://hry.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://eng.cdnleiting.top

[D16] 求和与平均值
来源：http://iez.fktsv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://shp.aibaodan.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uhi.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qpo.aizwys.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://krp.guannengcc.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://unt.hammf.cn

Go:   // 手写循环累加
来源：http://guf.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yty.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://zwb.ehwqpu.com

[D17] 最大值与最小值
来源：http://ncq.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://rxs.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://hkl.hcnkem.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bql.hcnkem.com

TS:   Math.max(...arr);
来源：http://wqv.wangdashe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://eut.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ppm.zhijiandao.cn

Ruby: arr.max;  arr.min
来源：http://hoi.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://ngy.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://bwi.smart0.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mvg.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://vwr.bjfxy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ruj.ppjwa.cn

TS:   nested.flat();
来源：http://kis.snrcjt.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ffm.svipenyu.cn

Go:   // 手写双层循环
来源：http://sql.mhx1999.top

Ruby: nested.flatten
来源：http://cmy.wangdashe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ukz.dashuyun.cn

[D19] 按字段分组
来源：http://vte.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gkl.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://web.haohaochexian.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zws.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qwb.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://egy.meibo888.top

Go:   // 手写 map[string][]T
来源：http://oba.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hpr.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gtj.ivvv.top

[D20] 统计每个元素出现次数
来源：http://ggw.fehbvm.com

Py:   Counter(arr)
来源：http://tuv.haohaochexian.top

PHP:  array_count_values($arr);
来源：http://tde.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kxq.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xgx.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nff.fanxiaobao.xyz

Go:   // 手写 map[T]int
来源：http://yso.jqgfzy.top

Ruby: arr.tally
来源：http://nst.52xcode.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tyb.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://pgc.xinyue.icu

Py:   x in arr
来源：http://avo.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://kmh.havefunace.top

JS:   arr.includes(x)
来源：http://eng.yangfankeji.com

TS:   arr.includes(x)
来源：http://rpu.gzhubu.top

Java: list.contains(x)
来源：http://gme.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://cox.zdqjudy.top

Ruby: arr.include?(x)
来源：http://jks.haohaochexian.top

C#:   list.Contains(x)
来源：http://sgm.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://qps.fzhhl.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nwn.uphjek.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qir.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zmy.zdbjq.cn

TS:   [...arr];
来源：http://utk.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://cls.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://avi.nwbrower.top

Ruby: arr.dup;  arr.clone
来源：http://agw.uphjek.com

C#:   new List<int>(list);
来源：http://dmu.yj202588.top

[D23] reduce 累积计算
来源：http://ada.xylfe.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xlr.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zmb.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://obz.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tpg.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bqq.haohaochexian.top

Go:   // 手写循环
来源：http://epw.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kgi.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://afd.aibaodan.cn

[D24] 字典 / Map 基本操作
来源：http://qtv.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jiz.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pyg.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tuo.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ppn.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xdu.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hqt.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://twq.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://orj.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://qws.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gxi.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qae.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://agq.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vgi.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pyt.chenjidiqi.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vkq.tanke756.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://swd.xingfuxueyuan.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bsv.mhx1999.top

[D26] 数组转字符串
来源：http://wqm.jyoumei.cn

Py:   ", ".join(map(str, arr))
来源：http://yio.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://tmt.sjlbkw.cn

JS:   arr.join(", ")
来源：http://pbl.hnqzz.top

TS:   arr.join(", ")
来源：http://evm.ybcxt.top

Java: String.join(", ", list)
来源：http://ick.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://jkl.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://knh.yuanzhike.top

C#:   string.Join(", ", list)
来源：http://kag.quarkkingdee.top

================================================================================
来源：http://ypl.iojbl.cn

E. 字符串处理
来源：http://rvg.c1oappe.top

================================================================================
来源：http://teo.ivvv.top

[E01] 拼接字符串
来源：http://awr.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zqc.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xqq.ydjk.org.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://grc.jiagoushi.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tee.hnxiangtu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rtk.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://enf.pycfn.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zhh.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://aco.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://bpe.bbcook.cn

Py:   "ab" * 3
来源：http://liu.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://ifr.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://oio.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://zit.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://fun.chenjidiqi.icu

Go:   strings.Repeat("ab", 3)
来源：http://hnx.gotoacloud.top

Ruby: "ab" * 3
来源：http://gzt.yuanzhike.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xrc.ctjpmb.com

[E03] 截取子串
来源：http://qsb.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uzk.zhoulong.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hiq.shuidangran.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lvn.hysaishi.cn

TS:   s.slice(1, 4)
来源：http://zno.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://zso.jianghu66.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qbv.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://jts.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://pvo.xziqi.cn

[E04] 查找子串位置
来源：http://ysm.jiagoushi.top

Py:   s.find("x");  s.index("x")
来源：http://szd.uphjek.com

PHP:  strpos($s, "x");
来源：http://iqe.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mvu.cqqwz.cn

TS:   s.indexOf("x")
来源：http://mqa.dashuyun.cn

Java: s.indexOf("x")
来源：http://wsz.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://occ.dianchejie.cn

Ruby: s.index("x")
来源：http://kbl.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://jqx.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cwe.havefunace.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://frm.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wxk.gzhubu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://srl.guowangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://unm.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tqs.sysykeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bmd.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rqq.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://asv.hywenlv.cn

[E06] 替换子串
来源：http://fue.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xrd.yangfankeji.com

PHP:  str_replace("a", "b", $s);
来源：http://wku.guannengcc.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pjj.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://jbp.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bky.tian-w.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eti.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pmu.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://cfl.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://nqr.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://axj.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://itg.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://xcj.ppjwa.cn

TS:   s.split(",")
来源：http://bmp.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://pfl.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zzu.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://pff.ctjpmb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tzw.jianghu66.top

[E08] 数组按分隔符合并
来源：http://vrp.cdnleiting.top

Py:   ",".join(items)
来源：http://idm.gotoacloud.top

PHP:  implode(",", $items);
来源：http://igg.xingfuxueyuan.xyz

JS:   items.join(",")
来源：http://hda.cucudq.cn

TS:   items.join(",")
来源：http://yyp.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://vdd.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://dya.tianlin.xyz

Ruby: items.join(",")
来源：http://eyn.andypj.xyz

C#:   string.Join(",", items)
来源：http://vot.epnwcf.com

[E09] 去除所有空白字符
来源：http://jdm.shzxlz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kag.aizwys.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bnu.guannengcc.top

JS:   s.replace(/\s+/g, "")
来源：http://nka.yongpay.top

TS:   s.replace(/\s+/g, "")
来源：http://czu.chenzaomai.com

Java: s.replaceAll("\\s+", "")
来源：http://our.chenlongwang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cjh.ctjpmb.com

Ruby: s.gsub(/\s+/, "")
来源：http://bov.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zqg.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://arn.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ces.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://occ.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://kzg.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://jvq.316326.xyz

Java: String.format("%03d", 7)
来源：http://rqz.cheryme.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qml.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://msv.meibo888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://heg.jqgufenzy.top

[E11] 反转字符串
来源：http://xeh.dianchejie.cn

Py:   s[::-1]
来源：http://awi.yonumen.top

PHP:  strrev($s);
来源：http://dxy.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://qad.guowangkeji.top

TS:   [...s].reverse().join("")
来源：http://dot.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://obi.yongpay.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yzb.hammf.cn

Ruby: s.reverse
来源：http://iat.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://eif.zhijiandao.cn

[E12] 统计某字符出现次数
来源：http://fuc.yvedp.cn

Py:   s.count("a")
来源：http://uqr.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://vnd.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://bdw.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://fmh.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ovk.cashguo.top

Go:   strings.Count(s, "a")
来源：http://neu.vqdsnc.cn

Ruby: s.count("a")
来源：http://nkg.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://bgp.yueranfly.top

[E13] 逐字符遍历
来源：http://uop.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://yku.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rwc.hnxiangtu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wpc.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://plb.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://npc.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://had.fehbvm.com

Ruby: s.each_char { |ch| puts ch }
来源：http://skg.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bsv.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://elx.smart0.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://muo.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vsp.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xkd.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zjn.vehdjk.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cdo.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pdg.zhoulong.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wyu.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lay.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://scl.fzhhl.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lto.gogol.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ffa.nanxuanxn.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ula.daria6918.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lay.nanxinkj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xew.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oib.chenjidiqi.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rte.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wcy.zhijiandao.cn

[E16] 数字千分位
来源：http://wro.yj202588.top

Py:   f"{1234567:,}"
来源：http://dmv.gotoacloud.top

PHP:  number_format(1234567);
来源：http://cxt.svipenyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hbd.yuxming.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xnv.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baz.yfazqb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wzt.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://agk.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://lkc.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://heu.zhixingplan.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eah.shanyushiyangtech.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fti.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zqb.hammf.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xsb.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://plj.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hfq.guannengcc.top

Ruby: s.capitalize
来源：http://wvm.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wvo.ydzc1.top

[E18] 模板占位符替换
来源：http://rdy.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://urw.yangfankeji.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://anc.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://zro.ppjwa.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nmj.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zjx.yongpay.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uol.andypj.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xmf.shanyushiyangtech.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://via.hesvh.cn

[E19] 多行文本按行拆分
来源：http://zxo.bjfxy.top

Py:   s.splitlines()
来源：http://rvc.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qmw.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://sox.cucudq.cn

TS:   s.split(/\r?\n/)
来源：http://nyy.daxiang520.top

Java: s.lines().toList()
来源：http://vts.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://mqy.kuanghao11.cn

Ruby: s.lines
来源：http://ett.meibo888.top

C#:   s.Split('\n')
来源：http://kqt.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://kil.vqdsnc.cn

Py:   if not s:
来源：http://ipj.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ass.wangshuangyany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iew.zycfv.cn

TS:   if (s === "") {}
来源：http://jjt.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://hlz.havefunace.top

Go:   if s == "" {}
来源：http://kna.vehdjk.com

Ruby: if s.empty?
来源：http://ixm.snrcjt.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yco.ybcxt.top

[E21] 超长截断加省略号
来源：http://yha.snrcjt.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ovh.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qaw.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ypd.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yby.ywan-chungtsiang.top


<!-- 参考信息 -->