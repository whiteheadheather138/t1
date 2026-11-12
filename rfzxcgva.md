代发 wailian999

TS:   [...new Set(arr)]
来源：http://zeo.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oxs.ydjk.org.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zxu.redwolf501.top

Ruby: arr.uniq
来源：http://kzo.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://rpv.fehbvm.com

[D16] 求和与平均值
来源：http://fmn.ywan-chungtsiang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tve.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dxm.ctjpmb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mls.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ohz.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kiu.tarul.cn

Go:   // 手写循环累加
来源：http://dmc.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mjn.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://dri.sxryk.cn

[D17] 最大值与最小值
来源：http://ifi.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://gsu.zycfv.cn

PHP:  max($arr);  min($arr);
来源：http://rja.hcnkem.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gxa.jyoumei.cn

TS:   Math.max(...arr);
来源：http://fuv.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sem.ivvv.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lzc.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://haq.ivvv.top

C#:   list.Max();  list.Min()
来源：http://hxg.shanyushiyangtech.top

[D18] 扁平化嵌套数组
来源：http://twj.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mkd.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://rxo.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://flt.yj202588.top

TS:   nested.flat();
来源：http://eds.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rju.hnxiangtu.top

Go:   // 手写双层循环
来源：http://ivc.jianghu66.top

Ruby: nested.flatten
来源：http://aym.yuxming.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ysb.zhixingplan.top

[D19] 按字段分组
来源：http://gaf.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://azq.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://trh.0kj1m.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tjt.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pba.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vwm.zycfv.cn

Go:   // 手写 map[string][]T
来源：http://zer.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ack.zhijiandao.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ugl.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://whw.cashguo.top

Py:   Counter(arr)
来源：http://rbv.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://ntm.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ddw.zhoulong.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jdm.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wjc.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://kko.redwolf501.top

Ruby: arr.tally
来源：http://pmt.yanxiufei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tio.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://yzq.hnxiangtu.top

Py:   x in arr
来源：http://dtu.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://bpc.bjfxy.top

JS:   arr.includes(x)
来源：http://qqz.meibo888.top

TS:   arr.includes(x)
来源：http://azv.smart0.xyz

Java: list.contains(x)
来源：http://mvl.bjfxy.top

Go:   slices.Contains(arr, x)
来源：http://qlz.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://tjm.zhengqikj.top

C#:   list.Contains(x)
来源：http://qgn.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://leh.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://srt.zhixingplan.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mri.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lfi.shangyingyoupin.top

TS:   [...arr];
来源：http://fch.cashguo.top

Java: new ArrayList<>(list);
来源：http://olk.hysaishi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hov.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://aky.tianlin.xyz

C#:   new List<int>(list);
来源：http://grg.iojbl.cn

[D23] reduce 累积计算
来源：http://jra.jyoumei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aoa.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eei.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jia.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mtv.aibaodan.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hmj.nwbrower.top

Go:   // 手写循环
来源：http://ayd.yuanzhike.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zyp.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kut.yangfankeji.com

[D24] 字典 / Map 基本操作
来源：http://uxu.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hrf.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pnt.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cnl.cheryme.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xwx.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cxt.guowangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zsy.hcnkem.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ngu.xingfuxueyuan.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kcy.yongpay.top

[D25] Set 集合去重与交并差
来源：http://etz.gogol.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ajy.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://irg.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ykv.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fpy.nanxinkj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cgs.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ydu.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yup.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pvn.yongpay.top

[D26] 数组转字符串
来源：http://qpi.epnwcf.com

Py:   ", ".join(map(str, arr))
来源：http://ejd.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://ugp.sjlbkw.cn

JS:   arr.join(", ")
来源：http://opj.hfpthk.cn

TS:   arr.join(", ")
来源：http://ykn.daria6918.cn

Java: String.join(", ", list)
来源：http://evt.nwbrower.top

Go:   strings.Join(strs, ", ")
来源：http://wrn.yvedp.cn

Ruby: arr.join(", ")
来源：http://foz.chenzaomai.com

C#:   string.Join(", ", list)
来源：http://fbl.chenjidiqi.icu

================================================================================
来源：http://lxc.pengpengdd.cyou

E. 字符串处理
来源：http://xmk.sjlbkw.cn

================================================================================
来源：http://ttc.birdmap.top

[E01] 拼接字符串
来源：http://bku.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ali.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://isu.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ssg.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://avf.gotoacloud.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hcd.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fob.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vag.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qka.iojbl.cn

[E02] 重复字符串
来源：http://ycy.nanxinkj.top

Py:   "ab" * 3
来源：http://dpj.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://lbe.mhx1999.top

JS:   "ab".repeat(3)
来源：http://kit.hnxiangtu.top

TS:   "ab".repeat(3)
来源：http://qmu.hnxiangtu.top

Java: "ab".repeat(3)
来源：http://fvz.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://uaq.yonumen.top

Ruby: "ab" * 3
来源：http://csn.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kno.bjfxy.top

[E03] 截取子串
来源：http://aur.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ldp.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tpt.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://chu.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://shz.dashuyun.cn

Java: s.substring(1, 4)
来源：http://xqs.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aib.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://urz.zhengqikj.top

C#:   s.Substring(1, 3)
来源：http://tsr.sjlbkw.cn

[E04] 查找子串位置
来源：http://lgg.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://qhu.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://ove.sufxvd.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wqp.fktsv.cn

TS:   s.indexOf("x")
来源：http://csc.tarul.cn

Java: s.indexOf("x")
来源：http://fla.ctjpmb.com

Go:   strings.Index(s, "x")
来源：http://yfm.cqqwz.cn

Ruby: s.index("x")
来源：http://jka.hnqzz.top

C#:   s.IndexOf("x")
来源：http://gqx.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gni.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wlp.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vcc.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://umq.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ynh.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rde.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rbw.cucudq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ywh.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rzd.uphjek.com

[E06] 替换子串
来源：http://xkx.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dnw.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://wkr.meibo888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://myv.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://une.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bbh.hongshengwenyu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ujo.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lvj.sjlbkw.cn

C#:   s.Replace("a", "b")
来源：http://njm.havefunace.top

[E07] 按分隔符拆分
来源：http://wbe.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wcs.tianlin.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qiy.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://gbb.chenzaomai.com

TS:   s.split(",")
来源：http://cht.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jtt.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ndh.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://bkn.zhoulong.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wzb.svipenyu.cn

[E08] 数组按分隔符合并
来源：http://dnn.sysykeji.top

Py:   ",".join(items)
来源：http://rmz.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://hoe.shanyushiyangkeji.top

JS:   items.join(",")
来源：http://cqu.redwolf501.top

TS:   items.join(",")
来源：http://bgc.aibaodan.cn

Java: String.join(",", items)
来源：http://qgl.52xcode.cn

Go:   strings.Join(items, ",")
来源：http://pub.zdbjq.cn

Ruby: items.join(",")
来源：http://ugm.hongshengwenyu.top

C#:   string.Join(",", items)
来源：http://uzw.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://jpp.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sno.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pio.pycfn.com

JS:   s.replace(/\s+/g, "")
来源：http://sgo.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://smc.zhiwuduotai.top

Java: s.replaceAll("\\s+", "")
来源：http://slv.pycfn.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://npf.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rhv.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yck.aibaodan.cn

[E10] 左侧补零 / 定长填充
来源：http://rzb.nanxinkj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tur.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rdq.guannengcc.top

JS:   "7".padStart(3, "0")
来源：http://mzm.yueranfly.top

TS:   "7".padStart(3, "0")
来源：http://mji.hammf.cn

Java: String.format("%03d", 7)
来源：http://ejb.dianchejie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tee.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iyh.xinyue.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jme.gotoacloud.top

[E11] 反转字符串
来源：http://utw.shzxlz.cn

Py:   s[::-1]
来源：http://hyd.cdnleiting.top

PHP:  strrev($s);
来源：http://rha.jinghuilouyu.cn

JS:   [...s].reverse().join("")
来源：http://kqv.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://svu.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://itd.nanxuanxn.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wpk.guowangkeji.top

Ruby: s.reverse
来源：http://qfz.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://rza.tanke756.top

[E12] 统计某字符出现次数
来源：http://zvt.sxryk.cn

Py:   s.count("a")
来源：http://kxk.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://pgr.zhongyouzk.top

JS:   s.split("a").length - 1
来源：http://srs.ydzc1.top

TS:   s.split("a").length - 1
来源：http://cso.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://enc.hywenlv.cn

Go:   strings.Count(s, "a")
来源：http://yir.chenzaomai.com

Ruby: s.count("a")
来源：http://wbe.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://lju.xinyue.icu

[E13] 逐字符遍历
来源：http://rbc.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://zhx.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ycn.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gdm.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yln.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dpl.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wgf.yueranfly.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yku.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://buq.c1oappe.top

[E14] URL 编码与 Base64
来源：http://tdr.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xoy.yj20258888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tzo.hammf.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xxr.xinyue.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ffy.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sjp.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ncc.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aeu.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://set.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://raw.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://gyc.guowangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cju.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cil.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pep.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mku.ehwqpu.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://raw.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rbx.xuetiantiany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fha.epnwcf.com

[E16] 数字千分位
来源：http://mjk.yj202588.top

Py:   f"{1234567:,}"
来源：http://bow.aibaodan.cn

PHP:  number_format(1234567);
来源：http://mhn.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mjw.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hre.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gqv.svipenyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://obp.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lil.cashguo.top

C#:   1234567.ToString("N0")
来源：http://krl.shuidangran.top

[E17] 首字母大写
来源：http://pyo.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ptg.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://vmr.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fzm.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dco.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rnh.jinyuanbaomall.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aub.ctjpmb.com

Ruby: s.capitalize
来源：http://fil.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tbn.fzhhl.top

[E18] 模板占位符替换
来源：http://zow.yanxiufei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gyj.xziqi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wxp.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uzc.jyoumei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nsb.yvedp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tue.ydzc1.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yff.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fii.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hpb.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://nka.chenjidiqi.icu

Py:   s.splitlines()
来源：http://tgi.ywan-chungtsiang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://daa.hfpthk.cn

JS:   s.split(/\r?\n/)
来源：http://rmz.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://igr.yfazqb.com

Java: s.lines().toList()
来源：http://ccn.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://lyn.hongshengwenyu.top

Ruby: s.lines
来源：http://bdp.yuanzhike.top

C#:   s.Split('\n')
来源：http://ujp.zhaomingkeji.xyz

[E20] 判断字符串是否为空
来源：http://vko.zdbjq.cn

Py:   if not s:
来源：http://opb.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://csn.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vdu.xziqi.cn

TS:   if (s === "") {}
来源：http://jek.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://cod.pycfn.com

Go:   if s == "" {}
来源：http://mqz.xingfuxueyuan.xyz

Ruby: if s.empty?
来源：http://gnc.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ylm.shanyushiyangtech.top

[E21] 超长截断加省略号
来源：http://nle.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fho.ppjwa.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vxm.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ebw.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oal.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vgx.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://kbh.yj20258888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gnl.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sir.gzhubu.top

[E22] 字节长度与字符长度
来源：http://xae.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hqd.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sji.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bjv.dianchejie.cn


<!-- 参考信息 -->