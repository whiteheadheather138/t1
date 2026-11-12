代发 wailian999

TS:   [...new Set(arr)]
来源：http://bsx.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pqc.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yhh.dianchejie.cn

Ruby: arr.uniq
来源：http://gzf.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://tjc.chenlongwang.top

[D16] 求和与平均值
来源：http://bhg.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dpk.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://djk.ywan-chungtsiang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yrg.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://grx.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kba.zhixingplan.top

Go:   // 手写循环累加
来源：http://kdw.daria6918.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gsh.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://cri.yuanzhike.top

[D17] 最大值与最小值
来源：http://zdn.zycfv.cn

Py:   max(arr);  min(arr)
来源：http://kdu.gaohongyu789.top

PHP:  max($arr);  min($arr);
来源：http://ort.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vfv.jianghu66.top

TS:   Math.max(...arr);
来源：http://rsq.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zif.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://svf.cucudq.cn

Ruby: arr.max;  arr.min
来源：http://zgw.xziqi.cn

C#:   list.Max();  list.Min()
来源：http://zgy.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://fdc.shanyushiyangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://brz.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://xhv.guowangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xqs.yuanzhike.top

TS:   nested.flat();
来源：http://qwx.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://snc.sjlbkw.cn

Go:   // 手写双层循环
来源：http://pjv.yongpay.top

Ruby: nested.flatten
来源：http://ptf.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qbb.nanxuanxn.top

[D19] 按字段分组
来源：http://imy.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cqd.yuanzhike.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mvr.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mwn.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wrv.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://epp.jinyuanbaomall.cn

Go:   // 手写 map[string][]T
来源：http://uae.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jgv.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gct.vqdsnc.cn

[D20] 统计每个元素出现次数
来源：http://viy.quarkkingdee.top

Py:   Counter(arr)
来源：http://oqu.shanyushiyangtech.top

PHP:  array_count_values($arr);
来源：http://pnq.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lgv.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nmd.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vkx.fehbvm.com

Go:   // 手写 map[T]int
来源：http://maf.pengpengdd.cyou

Ruby: arr.tally
来源：http://ofg.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nsz.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://cdj.yj20258.top

Py:   x in arr
来源：http://nxq.wangshuangyany.cn

PHP:  in_array($x, $arr, true);
来源：http://wth.daxiang520.top

JS:   arr.includes(x)
来源：http://hxu.hywenlv.cn

TS:   arr.includes(x)
来源：http://kwy.jyoumei.cn

Java: list.contains(x)
来源：http://ohw.nanxuanxn.top

Go:   slices.Contains(arr, x)
来源：http://imi.aibaodan.cn

Ruby: arr.include?(x)
来源：http://rsn.cucudq.cn

C#:   list.Contains(x)
来源：http://fsd.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://vcc.kuanghao11.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jsq.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zeq.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fji.0kj1m.cn

TS:   [...arr];
来源：http://rzn.yongpay.top

Java: new ArrayList<>(list);
来源：http://mbk.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qhs.iojbl.cn

Ruby: arr.dup;  arr.clone
来源：http://xja.andypj.xyz

C#:   new List<int>(list);
来源：http://ubc.xinyue.icu

[D23] reduce 累积计算
来源：http://ahd.sweek.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rqk.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ayz.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lvk.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nea.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cbq.smart0.xyz

Go:   // 手写循环
来源：http://unr.ydzc1.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sps.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pgr.hongshengwenyu.top

[D24] 字典 / Map 基本操作
来源：http://mdt.sysykeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nzf.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mic.wangshuangyany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://daz.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://awp.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rww.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mxm.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yfa.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ena.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://qvl.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rxa.haohaochexian.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ctc.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qul.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aiw.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dty.jlsjyb.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://smj.meibo888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xvj.jqgufenzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sxg.yfazqb.com

[D26] 数组转字符串
来源：http://sos.shuidangran.top

Py:   ", ".join(map(str, arr))
来源：http://rqb.yangfankeji.com

PHP:  implode(", ", $arr);
来源：http://fib.yuxming.cn

JS:   arr.join(", ")
来源：http://jjn.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://lla.yueranfly.top

Java: String.join(", ", list)
来源：http://dmr.bbcook.cn

Go:   strings.Join(strs, ", ")
来源：http://rul.fanxiaobao.xyz

Ruby: arr.join(", ")
来源：http://cgu.hcnkem.com

C#:   string.Join(", ", list)
来源：http://brc.wangdashe.top

================================================================================
来源：http://etb.vqdsnc.cn

E. 字符串处理
来源：http://adc.guowangkeji.top

================================================================================
来源：http://yxs.gotoacloud.top

[E01] 拼接字符串
来源：http://jiy.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uun.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kuk.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mqm.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://foy.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://taz.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://obw.jinghuilouyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://giv.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tgv.tanke756.top

[E02] 重复字符串
来源：http://vxv.bbcook.cn

Py:   "ab" * 3
来源：http://fss.chenzaomai.com

PHP:  str_repeat("ab", 3);
来源：http://zco.chenjidiqi.icu

JS:   "ab".repeat(3)
来源：http://dkf.cqqwz.cn

TS:   "ab".repeat(3)
来源：http://bem.daxiang520.top

Java: "ab".repeat(3)
来源：http://jea.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://kow.gogol.net.cn

Ruby: "ab" * 3
来源：http://tlc.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zod.cqqwz.cn

[E03] 截取子串
来源：http://vku.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vri.zhoulong.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bkv.ybcxt.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ikn.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://epz.tianlin.xyz

Java: s.substring(1, 4)
来源：http://bqg.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cpp.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dns.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://ana.yj202588.top

[E04] 查找子串位置
来源：http://cqk.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://tzw.svipenyu.cn

PHP:  strpos($s, "x");
来源：http://apm.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ylw.shanyushiyangtech.top

TS:   s.indexOf("x")
来源：http://drr.gzhubu.top

Java: s.indexOf("x")
来源：http://tnp.bjfxy.top

Go:   strings.Index(s, "x")
来源：http://buu.yj20258888.top

Ruby: s.index("x")
来源：http://rcq.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://zgh.cdnleiting.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vhc.zhongyouzk.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nrq.yueranfly.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gbg.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cua.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ksb.hywenlv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dxg.hnxiangtu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wep.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cfs.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wvf.yuxming.cn

[E06] 替换子串
来源：http://vpq.bjfxy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ehw.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://hsi.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cgf.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://nyt.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wxj.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ztr.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ult.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://tef.epnwcf.com

[E07] 按分隔符拆分
来源：http://jmj.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://drm.nanxuanxn.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qud.hywenlv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ygx.hysaishi.cn

TS:   s.split(",")
来源：http://cpi.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wik.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yjb.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://vzc.gzhubu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jll.fengsongda.top

[E08] 数组按分隔符合并
来源：http://lmt.hongshengwenyu.top

Py:   ",".join(items)
来源：http://cot.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://tip.zhiwuduotai.top

JS:   items.join(",")
来源：http://huo.xuetiantiany.cn

TS:   items.join(",")
来源：http://ajs.ctjpmb.com

Java: String.join(",", items)
来源：http://qjt.sweek.top

Go:   strings.Join(items, ",")
来源：http://dde.yj202588.top

Ruby: items.join(",")
来源：http://mwa.hysaishi.cn

C#:   string.Join(",", items)
来源：http://zzq.yj20258.top

[E09] 去除所有空白字符
来源：http://qwv.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kgg.hfpthk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eaq.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://yip.havefunace.top

TS:   s.replace(/\s+/g, "")
来源：http://uhy.svipenyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://ezv.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ber.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://iun.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yuj.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://oua.cheryme.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xnt.yfazqb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pda.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://keg.jinqigufen.top

TS:   "7".padStart(3, "0")
来源：http://bbk.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://hkh.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://twr.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hkx.daxiang520.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dhe.hnxiangtu.top

[E11] 反转字符串
来源：http://keh.yuxming.cn

Py:   s[::-1]
来源：http://kqy.shuidangran.top

PHP:  strrev($s);
来源：http://qyv.ybcxt.top

JS:   [...s].reverse().join("")
来源：http://ojz.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://sef.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://szp.cqqwz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ifj.yj20258.top

Ruby: s.reverse
来源：http://skh.ydjk.org.cn

C#:   new string(s.Reverse().ToArray())
来源：http://swb.tarul.cn

[E12] 统计某字符出现次数
来源：http://sxl.haohaochexian.top

Py:   s.count("a")
来源：http://faf.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://lsn.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://yjf.fanxiaobao.xyz

TS:   s.split("a").length - 1
来源：http://ixq.hnxiangtu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ltz.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://wbd.hysaishi.cn

Ruby: s.count("a")
来源：http://rjq.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://ush.xziqi.cn

[E13] 逐字符遍历
来源：http://tan.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://awa.aizwys.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gpy.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pzs.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ihj.pengpengdd.cyou

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blw.gotoacloud.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nii.c1oappe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zgy.chenjidiqi.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vcr.sxryk.cn

[E14] URL 编码与 Base64
来源：http://tpm.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vjx.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eqs.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qza.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://unj.yonumen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pbo.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zup.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kwa.tarul.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kny.bjfxy.top

[E15] HTML 转义 / 反转义
来源：http://skh.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://orw.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ikn.pycfn.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rvq.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pce.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jrh.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qna.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nby.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nmz.sysykeji.top

[E16] 数字千分位
来源：http://jxl.meibo888.top

Py:   f"{1234567:,}"
来源：http://ffz.svipenyu.cn

PHP:  number_format(1234567);
来源：http://wth.ppjwa.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sse.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://fel.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xyl.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://snq.jinqigufen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dme.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://yay.sxryk.cn

[E17] 首字母大写
来源：http://pnf.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://scw.chenzaomai.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://mgb.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tdr.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hns.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lxj.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lec.yanxiufei.cn

Ruby: s.capitalize
来源：http://yfy.jiagoushi.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ifg.c1oappe.top

[E18] 模板占位符替换
来源：http://wzy.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hsv.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ahk.jiagoushi.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vvn.zhoulong.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://jrq.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qza.jyoumei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cer.aibaodan.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dox.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ujx.havefunace.top

[E19] 多行文本按行拆分
来源：http://jgp.yanxiufei.cn

Py:   s.splitlines()
来源：http://vmm.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cnq.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://omw.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://sqw.nanxinkj.top

Java: s.lines().toList()
来源：http://jam.jlsjyb.cn

Go:   strings.Split(s, "\n")
来源：http://uxl.hongshengwenyu.top

Ruby: s.lines
来源：http://wmf.havefunace.top

C#:   s.Split('\n')
来源：http://iqs.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://uld.hongshengwenyu.top

Py:   if not s:
来源：http://azt.svipenyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://run.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://umw.bbcook.cn

TS:   if (s === "") {}
来源：http://eiz.xinyue.icu

Java: if (s.isEmpty()) {}
来源：http://uvf.hfpthk.cn

Go:   if s == "" {}
来源：http://zoi.daxiang520.top

Ruby: if s.empty?
来源：http://axd.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ebx.yvedp.cn

[E21] 超长截断加省略号
来源：http://rne.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zdp.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ziy.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://olq.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hek.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wmx.xziqi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ggd.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pfn.jinyuanbaomall.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gcn.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://lfs.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hkp.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bmy.feifeiyinyue.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://scn.c1oappe.top


<!-- 参考信息 -->