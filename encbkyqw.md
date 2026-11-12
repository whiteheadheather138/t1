代发 wailian999

TS:   [...new Set(arr)]
来源：http://ghb.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cic.shanyushiyangtech.top

Go:   // 用 map[T]struct{} 手写
来源：http://biu.wangshuangyany.cn

Ruby: arr.uniq
来源：http://kym.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://bqp.cqqwz.cn

[D16] 求和与平均值
来源：http://ehz.quarkkingdee.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hfs.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zwf.guowangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ulq.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://apx.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qfs.c1oappe.top

Go:   // 手写循环累加
来源：http://ksq.sjlbkw.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yyo.fktsv.cn

C#:   list.Sum();  list.Average()
来源：http://arg.uphjek.com

[D17] 最大值与最小值
来源：http://xsd.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://xrj.gzhubu.top

PHP:  max($arr);  min($arr);
来源：http://awh.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wnr.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://llp.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lei.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gth.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://ypx.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://suo.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://pom.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tbi.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://bgg.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rvy.chenzaomai.com

TS:   nested.flat();
来源：http://atl.yangfankeji.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jcz.xziqi.cn

Go:   // 手写双层循环
来源：http://fno.yj20258.top

Ruby: nested.flatten
来源：http://nju.uphjek.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ods.feifeiyinyue.top

[D19] 按字段分组
来源：http://rze.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://had.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fmx.ctjpmb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xui.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lif.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xus.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://exw.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mvj.dashuyun.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zlk.yongpay.top

[D20] 统计每个元素出现次数
来源：http://bav.cqqwz.cn

Py:   Counter(arr)
来源：http://zgk.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://mwg.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://onm.hfpthk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://izh.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://orm.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://ztk.chenjidiqi.icu

Ruby: arr.tally
来源：http://xcc.yanxiufei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ppd.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://xwz.jinqigufen.top

Py:   x in arr
来源：http://vyx.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://uda.ydzc1.top

JS:   arr.includes(x)
来源：http://olz.nanxinkj.top

TS:   arr.includes(x)
来源：http://iyl.zhijiandao.cn

Java: list.contains(x)
来源：http://zhl.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://xqv.smart0.xyz

Ruby: arr.include?(x)
来源：http://fgl.jqgfzy.top

C#:   list.Contains(x)
来源：http://jbl.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://era.yj20258888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mks.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hkn.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bcd.yongpay.top

TS:   [...arr];
来源：http://hya.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://bwu.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://tez.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://ohj.jiagoushi.top

C#:   new List<int>(list);
来源：http://anv.daria6918.cn

[D23] reduce 累积计算
来源：http://ney.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://low.sufxvd.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bmr.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://osx.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qmj.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bli.hammf.cn

Go:   // 手写循环
来源：http://jht.yongpay.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xln.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ojd.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://ldu.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fje.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uay.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fba.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xey.ctjpmb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bro.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ooh.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dem.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pno.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://wpt.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rae.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mkr.uphjek.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ftu.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lay.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qzm.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wui.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uoi.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://owx.guowangkeji.top

[D26] 数组转字符串
来源：http://hnk.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://yjf.ydzc1.top

PHP:  implode(", ", $arr);
来源：http://bru.guannengcc.top

JS:   arr.join(", ")
来源：http://dro.yongpay.top

TS:   arr.join(", ")
来源：http://amg.vehdjk.com

Java: String.join(", ", list)
来源：http://ngg.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://qkf.hnxiangtu.top

Ruby: arr.join(", ")
来源：http://hze.shanyushiyangtech.top

C#:   string.Join(", ", list)
来源：http://hdo.quarkkingdee.top

================================================================================
来源：http://zyx.ydjk.org.cn

E. 字符串处理
来源：http://hud.hammf.cn

================================================================================
来源：http://iyk.havefunace.top

[E01] 拼接字符串
来源：http://ygf.birdmap.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pce.sjlbkw.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zja.ppjwa.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zfv.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ksc.aizwys.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mwp.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iwi.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://atc.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gjy.jiagoushi.top

[E02] 重复字符串
来源：http://iqs.ivvv.top

Py:   "ab" * 3
来源：http://ykt.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://zbt.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://inc.fengsongda.top

TS:   "ab".repeat(3)
来源：http://iic.shanyushiyangtech.top

Java: "ab".repeat(3)
来源：http://zeg.yvedp.cn

Go:   strings.Repeat("ab", 3)
来源：http://fbl.ywan-chungtsiang.top

Ruby: "ab" * 3
来源：http://ppo.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hkk.ctjpmb.com

[E03] 截取子串
来源：http://bud.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jcj.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kjv.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ere.yj20258.top

TS:   s.slice(1, 4)
来源：http://ilf.yuxming.cn

Java: s.substring(1, 4)
来源：http://rjj.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://asa.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://oui.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://jpu.zycfv.cn

[E04] 查找子串位置
来源：http://euy.ehwqpu.com

Py:   s.find("x");  s.index("x")
来源：http://uyn.smart0.xyz

PHP:  strpos($s, "x");
来源：http://vjf.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ggh.hysaishi.cn

TS:   s.indexOf("x")
来源：http://ffu.gogol.net.cn

Java: s.indexOf("x")
来源：http://mma.meibo888.top

Go:   strings.Index(s, "x")
来源：http://qvj.yuanzhike.top

Ruby: s.index("x")
来源：http://put.yueranfly.top

C#:   s.IndexOf("x")
来源：http://ahc.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vop.zhoulong.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vtx.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kkb.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mhi.hywenlv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kcz.yongpay.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gvf.ydjk.org.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://abm.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xeo.jyoumei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eku.cdnleiting.top

[E06] 替换子串
来源：http://geo.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mew.nwbrower.top

PHP:  str_replace("a", "b", $s);
来源：http://wcp.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xpp.zhiwuduotai.top

TS:   s.replaceAll("a", "b")
来源：http://isy.shanyushiyangtech.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://igj.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xwm.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sla.tarul.cn

C#:   s.Replace("a", "b")
来源：http://njt.xylfe.cn

[E07] 按分隔符拆分
来源：http://ors.shangyingyoupin.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ylm.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://grr.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yjy.chenlongwang.top

TS:   s.split(",")
来源：http://zws.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://taa.redwolf501.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bhg.sxryk.cn

Ruby: s.split(",");  s.split
来源：http://byk.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://htu.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://qmg.gaohongyu789.top

Py:   ",".join(items)
来源：http://sfn.sysykeji.top

PHP:  implode(",", $items);
来源：http://mjv.jinghuilouyu.cn

JS:   items.join(",")
来源：http://ojy.uphjek.com

TS:   items.join(",")
来源：http://pwm.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://gio.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://mcr.hongshengwenyu.top

Ruby: items.join(",")
来源：http://irn.meibo888.top

C#:   string.Join(",", items)
来源：http://jrt.jianghu66.top

[E09] 去除所有空白字符
来源：http://ffx.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nya.ydzc1.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://heq.jiagoushi.top

JS:   s.replace(/\s+/g, "")
来源：http://epb.cucudq.cn

TS:   s.replace(/\s+/g, "")
来源：http://fqt.fehbvm.com

Java: s.replaceAll("\\s+", "")
来源：http://iny.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gmo.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ljm.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kza.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://ukh.yuxming.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ccj.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uaf.jqgfzy.top

JS:   "7".padStart(3, "0")
来源：http://vep.tanke756.top

TS:   "7".padStart(3, "0")
来源：http://epn.dianchejie.cn

Java: String.format("%03d", 7)
来源：http://vab.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tus.jlsjyb.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kmd.nanxinkj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ruc.yangfankeji.com

[E11] 反转字符串
来源：http://wtk.yfazqb.com

Py:   s[::-1]
来源：http://ouo.xuetiantiany.cn

PHP:  strrev($s);
来源：http://vfb.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://oue.yvedp.cn

TS:   [...s].reverse().join("")
来源：http://ent.9152youxi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ajf.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yyg.vehdjk.com

Ruby: s.reverse
来源：http://xww.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://mmz.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://qvt.gaohongyu789.top

Py:   s.count("a")
来源：http://dpq.zdqjudy.top

PHP:  substr_count($s, "a");
来源：http://wff.jinghuilouyu.cn

JS:   s.split("a").length - 1
来源：http://tjn.cucudq.cn

TS:   s.split("a").length - 1
来源：http://txl.bbcook.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kgw.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://gsv.vehdjk.com

Ruby: s.count("a")
来源：http://sqq.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://cso.hammf.cn

[E13] 逐字符遍历
来源：http://ytc.vqdsnc.cn

Py:   for ch in s: print(ch)
来源：http://hku.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vca.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ihh.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hnj.chenzaomai.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://abu.sufxvd.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uxs.fehbvm.com

Ruby: s.each_char { |ch| puts ch }
来源：http://hge.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qdu.jianghu66.top

[E14] URL 编码与 Base64
来源：http://kyp.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kuo.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xib.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rah.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qqz.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qex.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rzk.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hey.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fpv.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://iar.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://rxz.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://elr.shzxlz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kpw.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ddm.sweek.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kvt.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uaz.chenjidiqi.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vyv.hfpthk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://get.ywan-chungtsiang.top

[E16] 数字千分位
来源：http://ncs.hnqzz.top

Py:   f"{1234567:,}"
来源：http://brz.tarul.cn

PHP:  number_format(1234567);
来源：http://sga.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dkn.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://thj.jyoumei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://byi.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bgd.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://llx.ydzc1.top

C#:   1234567.ToString("N0")
来源：http://vtz.xuetiantiany.cn

[E17] 首字母大写
来源：http://hcd.fanxiaobao.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mbu.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://omw.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yil.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cwm.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kru.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://enp.jianghu66.top

Ruby: s.capitalize
来源：http://bww.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gvm.jqgfzy.top

[E18] 模板占位符替换
来源：http://vlw.daria6918.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://npe.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hgn.0kj1m.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yiv.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://gen.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eye.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sfj.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nfs.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hxk.ivvv.top

[E19] 多行文本按行拆分
来源：http://edu.c1oappe.top

Py:   s.splitlines()
来源：http://oba.nwbrower.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zbv.zdbjq.cn

JS:   s.split(/\r?\n/)
来源：http://nxr.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://vrj.sweek.top

Java: s.lines().toList()
来源：http://eqe.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://aze.yanxiufei.cn

Ruby: s.lines
来源：http://lxf.yj202588.top

C#:   s.Split('\n')
来源：http://lab.chenjidiqi.icu

[E20] 判断字符串是否为空
来源：http://ewu.daxiang520.top

Py:   if not s:
来源：http://mvp.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://npl.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rvg.yj202588.top

TS:   if (s === "") {}
来源：http://zws.yj20258.top

Java: if (s.isEmpty()) {}
来源：http://gyf.tarul.cn

Go:   if s == "" {}
来源：http://ghr.aizwys.cn

Ruby: if s.empty?
来源：http://lcw.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://abx.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://xjv.fehbvm.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://isc.dashuyun.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://crx.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rjj.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zna.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ppp.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://xdu.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sao.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lts.fengsongda.top

[E22] 字节长度与字符长度
来源：http://orz.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://axc.nwbrower.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tvt.hcnkem.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pks.dashuyun.cn


<!-- 参考信息 -->