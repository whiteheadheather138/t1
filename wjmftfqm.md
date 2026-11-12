代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://qfg.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gdr.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://gxz.vehdjk.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jlx.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://efi.svipenyu.cn

Ruby: arr.max;  arr.min
来源：http://nmy.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://ddn.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://gmr.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hzz.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://txw.ydjk.org.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xjd.snrcjt.cn

TS:   nested.flat();
来源：http://rch.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uno.tarul.cn

Go:   // 手写双层循环
来源：http://knj.xuetiantiany.cn

Ruby: nested.flatten
来源：http://xlp.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wbs.c1oappe.top

[D19] 按字段分组
来源：http://bky.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vjz.yj20258888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lvf.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fke.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cnu.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://loy.sufxvd.cn

Go:   // 手写 map[string][]T
来源：http://pfu.yj202588.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cts.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ryk.pycfn.com

[D20] 统计每个元素出现次数
来源：http://hcz.wangdashe.top

Py:   Counter(arr)
来源：http://vck.zycfv.cn

PHP:  array_count_values($arr);
来源：http://niu.jqgufenzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zyq.hammf.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dxv.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xca.zhongyouzk.top

Go:   // 手写 map[T]int
来源：http://ucd.svipenyu.cn

Ruby: arr.tally
来源：http://cvl.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hev.ybcxt.top

[D21] 判断是否包含某元素
来源：http://zep.gaohongyu789.top

Py:   x in arr
来源：http://bri.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://hie.hfpthk.cn

JS:   arr.includes(x)
来源：http://lpw.tanke756.top

TS:   arr.includes(x)
来源：http://fmm.yangfankeji.com

Java: list.contains(x)
来源：http://viv.yj20258.top

Go:   slices.Contains(arr, x)
来源：http://mdj.haohaochexian.top

Ruby: arr.include?(x)
来源：http://kfq.yangfankeji.com

C#:   list.Contains(x)
来源：http://gky.zhoulong.xyz

[D22] 复制数组（避免共享引用）
来源：http://rtg.feifeiyinyue.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://clr.xingfuxueyuan.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kvd.yonumen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fxp.9152youxi.cn

TS:   [...arr];
来源：http://iqg.tanke756.top

Java: new ArrayList<>(list);
来源：http://oeh.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://yrk.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://ldc.jianghu66.top

C#:   new List<int>(list);
来源：http://zxv.ybcxt.top

[D23] reduce 累积计算
来源：http://pub.gogol.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fml.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fsc.jinghuilouyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dkw.yueranfly.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yva.xylfe.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qle.tanke756.top

Go:   // 手写循环
来源：http://uzq.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jrh.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dqs.yj202588.top

[D24] 字典 / Map 基本操作
来源：http://kof.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://npx.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hwk.tianlin.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fyq.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jda.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xau.andypj.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://air.sjlbkw.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ecv.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lav.tanke756.top

[D25] Set 集合去重与交并差
来源：http://tbq.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rzc.aibaodan.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pmn.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ena.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://efq.0kj1m.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ije.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hid.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cnx.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ojx.pycfn.com

[D26] 数组转字符串
来源：http://uua.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://bwa.yvedp.cn

PHP:  implode(", ", $arr);
来源：http://wwx.gotoacloud.top

JS:   arr.join(", ")
来源：http://mys.yvedp.cn

TS:   arr.join(", ")
来源：http://whr.hysaishi.cn

Java: String.join(", ", list)
来源：http://qbo.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://fdl.fehbvm.com

Ruby: arr.join(", ")
来源：http://tax.hysaishi.cn

C#:   string.Join(", ", list)
来源：http://rvn.zhengqikj.top

================================================================================
来源：http://vlr.bbcook.cn

E. 字符串处理
来源：http://nil.yj20258888.top

================================================================================
来源：http://kbc.yonumen.top

[E01] 拼接字符串
来源：http://esb.jiagoushi.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rru.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://djp.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aso.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yks.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fbx.hnqzz.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nzn.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://obd.haohaochexian.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zld.tanke756.top

[E02] 重复字符串
来源：http://hzd.svipenyu.cn

Py:   "ab" * 3
来源：http://ipe.316326.xyz

PHP:  str_repeat("ab", 3);
来源：http://zxr.cdnleiting.top

JS:   "ab".repeat(3)
来源：http://cla.iojbl.cn

TS:   "ab".repeat(3)
来源：http://qxc.gzhubu.top

Java: "ab".repeat(3)
来源：http://dgl.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://fjp.guowangkeji.top

Ruby: "ab" * 3
来源：http://wqe.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tex.ydzc1.top

[E03] 截取子串
来源：http://uqy.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yae.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nfj.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xrn.yj20258888.top

TS:   s.slice(1, 4)
来源：http://bqk.fanxiaobao.xyz

Java: s.substring(1, 4)
来源：http://hog.tianlin.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kgh.sxryk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fjl.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://gav.quarkkingdee.top

[E04] 查找子串位置
来源：http://lmo.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://ano.daria6918.cn

PHP:  strpos($s, "x");
来源：http://mfk.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iod.nanxinkj.top

TS:   s.indexOf("x")
来源：http://cig.yj20258.top

Java: s.indexOf("x")
来源：http://zlo.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://jsp.0kj1m.cn

Ruby: s.index("x")
来源：http://ehk.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://swz.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jdc.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rwj.yueranfly.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eea.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yhv.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wvh.zycfv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ief.chenzaomai.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rry.gogol.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vhu.fanxiaobao.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lgz.fengsongda.top

[E06] 替换子串
来源：http://hhq.yonumen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kcj.zhongyouzk.top

PHP:  str_replace("a", "b", $s);
来源：http://vzn.yvedp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ksh.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://ouu.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://udz.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tes.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kct.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://vay.chenjidiqi.icu

[E07] 按分隔符拆分
来源：http://adn.shangyingyoupin.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qwn.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zvi.gotoacloud.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://aho.jqgufenzy.top

TS:   s.split(",")
来源：http://xjv.yanxiufei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kbr.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aog.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://bgv.gogol.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wka.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://mve.zhaomingkeji.xyz

Py:   ",".join(items)
来源：http://dtn.jinqigufen.top

PHP:  implode(",", $items);
来源：http://rvy.wangshuangyany.cn

JS:   items.join(",")
来源：http://flv.cheryme.top

TS:   items.join(",")
来源：http://cei.dianchejie.cn

Java: String.join(",", items)
来源：http://far.xinyue.icu

Go:   strings.Join(items, ",")
来源：http://koj.cashguo.top

Ruby: items.join(",")
来源：http://uls.hnqzz.top

C#:   string.Join(",", items)
来源：http://bef.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://uzq.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yuk.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xdv.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://hec.vehdjk.com

TS:   s.replace(/\s+/g, "")
来源：http://efb.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://yki.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://koq.redwolf501.top

Ruby: s.gsub(/\s+/, "")
来源：http://cvo.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dlv.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://fqf.nwbrower.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ytm.jinqigufen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://svm.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://pek.c1oappe.top

TS:   "7".padStart(3, "0")
来源：http://lff.cashguo.top

Java: String.format("%03d", 7)
来源：http://fkj.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ije.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ieo.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uqa.tarul.cn

[E11] 反转字符串
来源：http://hon.tianlin.xyz

Py:   s[::-1]
来源：http://swp.sufxvd.cn

PHP:  strrev($s);
来源：http://jdz.zdbjq.cn

JS:   [...s].reverse().join("")
来源：http://vvh.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://vqw.xuanzx.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ymi.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jpb.ybcxt.top

Ruby: s.reverse
来源：http://gpk.yj20258888.top

C#:   new string(s.Reverse().ToArray())
来源：http://icv.yvedp.cn

[E12] 统计某字符出现次数
来源：http://ano.bbcook.cn

Py:   s.count("a")
来源：http://ysd.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://lyu.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://eyv.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://mzt.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eks.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://iro.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://sta.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://nct.kuanghao11.cn

[E13] 逐字符遍历
来源：http://miq.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://hxj.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gfg.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wma.yanxiufei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zqc.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mkv.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fiy.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://eoi.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lvr.ctjpmb.com

[E14] URL 编码与 Base64
来源：http://upi.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://viy.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lpn.shanyushiyangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yxj.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ijj.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rwh.zhijiandao.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zzp.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rcb.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pin.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://pfh.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://spf.vqdsnc.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zss.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://szw.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://glc.nanxinkj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tys.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gsp.xuetiantiany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gwj.wangshuangyany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ten.9152youxi.cn

[E16] 数字千分位
来源：http://aqa.yj20258.top

Py:   f"{1234567:,}"
来源：http://giv.yfazqb.com

PHP:  number_format(1234567);
来源：http://kdj.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://aqn.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xdz.xylfe.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jyu.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eor.aibaodan.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yrd.smart0.xyz

C#:   1234567.ToString("N0")
来源：http://knn.gogol.net.cn

[E17] 首字母大写
来源：http://apk.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wqn.316326.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://iky.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://evt.zhiwuduotai.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://low.ctjpmb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qka.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://izy.yfazqb.com

Ruby: s.capitalize
来源：http://awg.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://das.sufxvd.cn

[E18] 模板占位符替换
来源：http://fmu.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wrg.yanxiufei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lzr.jianghu66.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rlt.zhijiandao.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://frd.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zvn.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://brj.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://moj.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uzw.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://gii.cqqwz.cn

Py:   s.splitlines()
来源：http://ilz.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dhr.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://mmm.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://pwm.zhaomingkeji.xyz

Java: s.lines().toList()
来源：http://cmc.guowangkeji.top

Go:   strings.Split(s, "\n")
来源：http://zhx.jinyuanbaomall.cn

Ruby: s.lines
来源：http://dic.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://iod.hesvh.cn

[E20] 判断字符串是否为空
来源：http://azt.hywenlv.cn

Py:   if not s:
来源：http://jfr.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ada.mhx1999.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://plk.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://vrg.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://ybd.jinghuilouyu.cn

Go:   if s == "" {}
来源：http://xsu.hongshengwenyu.top

Ruby: if s.empty?
来源：http://eqe.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cbl.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://pov.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fsa.guannengcc.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dat.zhiwuduotai.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fyy.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://utj.vqdsnc.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xva.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://hyw.52xcode.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://agd.sufxvd.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://csd.nanxuanxn.top

[E22] 字节长度与字符长度
来源：http://umj.gotoacloud.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hjn.zhoulong.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xah.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bff.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yci.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://opc.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oxj.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://teo.zhengqikj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yow.nwbrower.top

================================================================================
来源：http://xaw.hesvh.cn

F. 文件与目录
来源：http://xdc.cheryme.top

================================================================================
来源：http://klx.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://zzk.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oav.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://lai.hcnkem.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tng.316326.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xua.chenlongwang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kdv.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wjz.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://rkl.wangshuangyany.cn


<!-- 参考信息 -->