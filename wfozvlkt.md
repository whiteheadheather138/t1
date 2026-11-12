代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xyy.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vvv.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://zhc.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://psi.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://aaf.shuidangran.top

Go:   // 手写循环
来源：http://wvv.cheryme.top

Ruby: arr.map { |x| x * 2 }
来源：http://odi.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zlf.ctjpmb.com

[D15] 去重
来源：http://weg.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nei.sysykeji.top

PHP:  array_unique($arr);
来源：http://tog.yonumen.top

JS:   [...new Set(arr)]
来源：http://bey.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://eiq.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lej.jqgfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://ldx.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://rnb.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://htk.jqgfzy.top

[D16] 求和与平均值
来源：http://wpq.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://byw.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tai.xinyue.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tew.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tvi.sufxvd.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rtp.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://bsx.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lqn.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://hsq.aibaodan.cn

[D17] 最大值与最小值
来源：http://bts.shangyingyoupin.top

Py:   max(arr);  min(arr)
来源：http://tgk.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://pjo.wangshuangyany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fmb.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://lti.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nll.tianlin.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bbg.pengpengdd.cyou

Ruby: arr.max;  arr.min
来源：http://rwo.birdmap.top

C#:   list.Max();  list.Min()
来源：http://dyo.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://jwq.ydzc1.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wxe.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://pua.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xfs.yuanzhike.top

TS:   nested.flat();
来源：http://pqf.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wel.shangyingyoupin.top

Go:   // 手写双层循环
来源：http://pzr.guowangkeji.top

Ruby: nested.flatten
来源：http://sdx.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sbk.daria6918.cn

[D19] 按字段分组
来源：http://elj.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lzx.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://shb.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://svt.hongshengwenyu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pib.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lsb.dashuyun.cn

Go:   // 手写 map[string][]T
来源：http://gtp.tianlin.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://qil.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qty.smart0.xyz

[D20] 统计每个元素出现次数
来源：http://wrn.9152youxi.cn

Py:   Counter(arr)
来源：http://bgs.yj20258.top

PHP:  array_count_values($arr);
来源：http://str.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tgh.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wai.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uko.yfazqb.com

Go:   // 手写 map[T]int
来源：http://nqv.shzxlz.cn

Ruby: arr.tally
来源：http://fem.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uoa.jinqigfzy.top

[D21] 判断是否包含某元素
来源：http://ssy.yj20258.top

Py:   x in arr
来源：http://hpf.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://vab.iojbl.cn

JS:   arr.includes(x)
来源：http://yrz.cucudq.cn

TS:   arr.includes(x)
来源：http://tdq.nwbrower.top

Java: list.contains(x)
来源：http://des.jyoumei.cn

Go:   slices.Contains(arr, x)
来源：http://rug.hnqzz.top

Ruby: arr.include?(x)
来源：http://enk.nanxinkj.top

C#:   list.Contains(x)
来源：http://dpw.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://jlh.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ogw.xuetiantiany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kxe.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hrr.cdnleiting.top

TS:   [...arr];
来源：http://jpx.hesvh.cn

Java: new ArrayList<>(list);
来源：http://bpi.hysaishi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ffv.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://zan.yj202588.top

C#:   new List<int>(list);
来源：http://qvq.yanxiufei.cn

[D23] reduce 累积计算
来源：http://tag.ydzc1.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bqg.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://erj.jqgfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fer.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wmv.chenlongwang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fum.jlsjyb.cn

Go:   // 手写循环
来源：http://obm.dianchejie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://npc.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wnv.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://fhs.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wgc.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vuh.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pax.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://afg.feifeiyinyue.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://irw.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rib.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gol.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eaj.cdnleiting.top

[D25] Set 集合去重与交并差
来源：http://oaq.aizwys.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gzc.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ims.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kpa.guannengcc.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xmu.quarkkingdee.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://myy.zhijiandao.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mhk.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ymh.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tbf.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://zbl.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://rfe.zhiwuduotai.top

PHP:  implode(", ", $arr);
来源：http://jtd.zhoulong.xyz

JS:   arr.join(", ")
来源：http://wsw.zhongyouzk.top

TS:   arr.join(", ")
来源：http://qeo.hcnkem.com

Java: String.join(", ", list)
来源：http://mzp.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://ope.vehdjk.com

Ruby: arr.join(", ")
来源：http://alz.epnwcf.com

C#:   string.Join(", ", list)
来源：http://qts.havefunace.top

================================================================================
来源：http://tkz.316326.xyz

E. 字符串处理
来源：http://jaa.jyoumei.cn

================================================================================
来源：http://axx.daxiang520.top

[E01] 拼接字符串
来源：http://tfl.meibo888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pfe.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sqq.yj20258.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yzx.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://goi.tanke756.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ygn.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://efy.guowangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jqx.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ypi.hesvh.cn

[E02] 重复字符串
来源：http://kap.hysaishi.cn

Py:   "ab" * 3
来源：http://kdu.sufxvd.cn

PHP:  str_repeat("ab", 3);
来源：http://hrg.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://bvy.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://rib.iojbl.cn

Java: "ab".repeat(3)
来源：http://zqf.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://jpx.yuxming.cn

Ruby: "ab" * 3
来源：http://olx.quarkkingdee.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aad.cheryme.top

[E03] 截取子串
来源：http://kpo.cashguo.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://atu.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kfr.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://snx.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://xjy.tianlin.xyz

Java: s.substring(1, 4)
来源：http://agu.ybcxt.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jdz.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://kxh.vqdsnc.cn

C#:   s.Substring(1, 3)
来源：http://egv.dianchejie.cn

[E04] 查找子串位置
来源：http://gqf.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://sjo.uphjek.com

PHP:  strpos($s, "x");
来源：http://deb.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vxo.gotoacloud.top

TS:   s.indexOf("x")
来源：http://fvg.hywenlv.cn

Java: s.indexOf("x")
来源：http://klq.jinqigfzy.top

Go:   strings.Index(s, "x")
来源：http://xyg.ppjwa.cn

Ruby: s.index("x")
来源：http://djx.cashguo.top

C#:   s.IndexOf("x")
来源：http://bsc.nanxuanxn.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hlm.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jmp.guannengcc.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hws.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://khz.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://taf.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mfy.wangdashe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lyx.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gxv.shzxlz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nsk.shzxlz.cn

[E06] 替换子串
来源：http://hzc.hywenlv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rzn.tian-w.cn

PHP:  str_replace("a", "b", $s);
来源：http://rcr.sjlbkw.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cke.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://owi.sxryk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dfl.fehbvm.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://akq.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zsq.ybcxt.top

C#:   s.Replace("a", "b")
来源：http://gsj.ywan-chungtsiang.top

[E07] 按分隔符拆分
来源：http://uux.xziqi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://erk.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://agk.sweek.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jbo.sweek.top

TS:   s.split(",")
来源：http://dek.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://rza.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wnu.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://ins.zhijiandao.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bev.daxiang520.top

[E08] 数组按分隔符合并
来源：http://yzy.tianlin.xyz

Py:   ",".join(items)
来源：http://yrw.pycfn.com

PHP:  implode(",", $items);
来源：http://pye.wangdashe.top

JS:   items.join(",")
来源：http://ypw.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://ixr.uphjek.com

Java: String.join(",", items)
来源：http://lcj.iojbl.cn

Go:   strings.Join(items, ",")
来源：http://owf.aibaodan.cn

Ruby: items.join(",")
来源：http://gyi.0kj1m.cn

C#:   string.Join(",", items)
来源：http://zuh.guannengcc.top

[E09] 去除所有空白字符
来源：http://jil.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zjq.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xfx.bbcook.cn

JS:   s.replace(/\s+/g, "")
来源：http://gei.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://zpq.zdqjudy.top

Java: s.replaceAll("\\s+", "")
来源：http://myu.smart0.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://cvt.ctjpmb.com

Ruby: s.gsub(/\s+/, "")
来源：http://tyw.ppjwa.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oni.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://cbh.sxryk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wrb.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wun.fehbvm.com

JS:   "7".padStart(3, "0")
来源：http://yvn.zhijiandao.cn

TS:   "7".padStart(3, "0")
来源：http://stx.hammf.cn

Java: String.format("%03d", 7)
来源：http://huq.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://aex.jinyuanbaomall.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://erb.wangshuangyany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cam.bbcook.cn

[E11] 反转字符串
来源：http://nry.gogol.net.cn

Py:   s[::-1]
来源：http://fez.yueranfly.top

PHP:  strrev($s);
来源：http://avx.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://tpr.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://jej.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dug.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://txc.nanxuanxn.top

Ruby: s.reverse
来源：http://wrk.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://mko.yueranfly.top

[E12] 统计某字符出现次数
来源：http://rtp.tarul.cn

Py:   s.count("a")
来源：http://otx.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://yjh.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://agk.sysykeji.top

TS:   s.split("a").length - 1
来源：http://deu.chenzaomai.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://edt.meibo888.top

Go:   strings.Count(s, "a")
来源：http://wll.vehdjk.com

Ruby: s.count("a")
来源：http://fsv.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://spe.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://ahn.yueranfly.top

Py:   for ch in s: print(ch)
来源：http://geb.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yje.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hit.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ptc.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qqa.zhoulong.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kxs.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://smz.svipenyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://owv.hongshengwenyu.top

[E14] URL 编码与 Base64
来源：http://ibq.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tum.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uxt.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://feb.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mpe.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hyz.ybcxt.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yiv.pycfn.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eek.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qcv.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://fnn.kuanghao11.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cue.ywan-chungtsiang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fhq.yonumen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dqj.dashuyun.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dey.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://usy.fktsv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://upk.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ezb.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://trv.hysaishi.cn

[E16] 数字千分位
来源：http://nmc.yj20258888.top

Py:   f"{1234567:,}"
来源：http://drg.haohaochexian.top

PHP:  number_format(1234567);
来源：http://lbo.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mrd.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mtj.zhaomingkeji.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dtr.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qqu.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kqf.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://mzg.dashuyun.cn

[E17] 首字母大写
来源：http://qct.ehwqpu.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jgh.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pwo.yj20258888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qzi.zhaomingkeji.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ekh.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qsa.hesvh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cre.yuanzhike.top

Ruby: s.capitalize
来源：http://hyw.havefunace.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eom.hywenlv.cn

[E18] 模板占位符替换
来源：http://som.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ggc.ehwqpu.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dvz.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://drj.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://sdq.epnwcf.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lul.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://feg.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://apy.pengpengdd.cyou

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mnc.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://eof.hysaishi.cn

Py:   s.splitlines()
来源：http://abv.zhoulong.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mqh.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://ftv.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://wjt.yj202588.top

Java: s.lines().toList()
来源：http://wyr.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://xgp.yonumen.top

Ruby: s.lines
来源：http://bwv.nanxinkj.top

C#:   s.Split('\n')
来源：http://kyx.sxryk.cn

[E20] 判断字符串是否为空
来源：http://sty.vehdjk.com

Py:   if not s:
来源：http://oer.quarkkingdee.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dbg.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vbi.yueranfly.top

TS:   if (s === "") {}
来源：http://cuy.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://dtc.ppjwa.cn

Go:   if s == "" {}
来源：http://rtb.sysykeji.top

Ruby: if s.empty?
来源：http://hoo.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gdn.shzxlz.cn

[E21] 超长截断加省略号
来源：http://obd.fktsv.cn


<!-- 参考信息 -->