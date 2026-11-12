代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mts.svipenyu.cn

Ruby: arr.max;  arr.min
来源：http://jeq.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://ikg.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://wlz.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rnv.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://vth.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lef.yfazqb.com

TS:   nested.flat();
来源：http://khl.vqdsnc.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zre.hysaishi.cn

Go:   // 手写双层循环
来源：http://wms.c1oappe.top

Ruby: nested.flatten
来源：http://zyv.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jlf.sxryk.cn

[D19] 按字段分组
来源：http://hpc.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vro.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zmg.fzhhl.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uou.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://koo.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wyk.meibo888.top

Go:   // 手写 map[string][]T
来源：http://aod.fktsv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hxg.cdnleiting.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mtm.havefunace.top

[D20] 统计每个元素出现次数
来源：http://ezl.jqgfzy.top

Py:   Counter(arr)
来源：http://rzh.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://dhx.0kj1m.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jlj.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://klo.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://axl.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://vls.chenjidiqi.icu

Ruby: arr.tally
来源：http://tbt.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://onf.c1oappe.top

[D21] 判断是否包含某元素
来源：http://bsd.guowangkeji.top

Py:   x in arr
来源：http://twk.nwbrower.top

PHP:  in_array($x, $arr, true);
来源：http://ewb.gzhubu.top

JS:   arr.includes(x)
来源：http://qjg.xinyue.icu

TS:   arr.includes(x)
来源：http://dbx.wangshuangyany.cn

Java: list.contains(x)
来源：http://dnw.daxiang520.top

Go:   slices.Contains(arr, x)
来源：http://xix.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://jrx.shanyushiyangtech.top

C#:   list.Contains(x)
来源：http://akh.meibo888.top

[D22] 复制数组（避免共享引用）
来源：http://amv.kuanghao11.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hvp.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hfs.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://slp.guowangkeji.top

TS:   [...arr];
来源：http://byw.hesvh.cn

Java: new ArrayList<>(list);
来源：http://dmj.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jvf.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://kdb.jqgufenzy.top

C#:   new List<int>(list);
来源：http://xig.nanxinkj.top

[D23] reduce 累积计算
来源：http://wzo.jiagoushi.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qct.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iix.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jqx.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xkv.guannengcc.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mox.zhongyouzk.top

Go:   // 手写循环
来源：http://evq.nanxinkj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kpr.tanke756.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vdp.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://tzh.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sry.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bqu.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gmd.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fsr.mhx1999.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lll.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ewc.pengpengdd.cyou

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iau.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oye.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://lgq.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zzw.vehdjk.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fzp.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://beu.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kad.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ytw.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mdi.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zqw.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://huu.xingfuxueyuan.xyz

[D26] 数组转字符串
来源：http://xac.mhx1999.top

Py:   ", ".join(map(str, arr))
来源：http://hzc.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://juj.hcnkem.com

JS:   arr.join(", ")
来源：http://kus.c1oappe.top

TS:   arr.join(", ")
来源：http://tcx.pycfn.com

Java: String.join(", ", list)
来源：http://hhf.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://cvp.tian-w.cn

Ruby: arr.join(", ")
来源：http://dff.ydjk.org.cn

C#:   string.Join(", ", list)
来源：http://nxs.hesvh.cn

================================================================================
来源：http://tom.mhx1999.top

E. 字符串处理
来源：http://kmk.jqgufenzy.top

================================================================================
来源：http://qqj.vehdjk.com

[E01] 拼接字符串
来源：http://noy.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sds.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hgd.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vpm.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xfo.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mfj.sufxvd.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bnj.feifeiyinyue.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xms.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cxk.chenlongwang.top

[E02] 重复字符串
来源：http://zxx.jqgfzy.top

Py:   "ab" * 3
来源：http://qwb.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://wlt.tian-w.cn

JS:   "ab".repeat(3)
来源：http://xkn.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://bgn.hywenlv.cn

Java: "ab".repeat(3)
来源：http://yrh.snrcjt.cn

Go:   strings.Repeat("ab", 3)
来源：http://rhm.cqqwz.cn

Ruby: "ab" * 3
来源：http://xuq.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xge.snrcjt.cn

[E03] 截取子串
来源：http://jto.tanke756.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mqz.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://njo.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aip.meibo888.top

TS:   s.slice(1, 4)
来源：http://vov.hfpthk.cn

Java: s.substring(1, 4)
来源：http://two.havefunace.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gxy.yuxming.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zfy.redwolf501.top

C#:   s.Substring(1, 3)
来源：http://xye.jianghu66.top

[E04] 查找子串位置
来源：http://oli.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://ajq.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://uwo.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rai.hammf.cn

TS:   s.indexOf("x")
来源：http://sfd.ppjwa.cn

Java: s.indexOf("x")
来源：http://wid.jinqigfzy.top

Go:   strings.Index(s, "x")
来源：http://wro.xziqi.cn

Ruby: s.index("x")
来源：http://nby.mhx1999.top

C#:   s.IndexOf("x")
来源：http://wzi.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gvg.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://grt.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wbu.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mlc.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://bzt.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://spu.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://big.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vpx.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sro.jiagoushi.top

[E06] 替换子串
来源：http://awy.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zvz.hesvh.cn

PHP:  str_replace("a", "b", $s);
来源：http://ijf.zhijiandao.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dxb.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://zbi.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hro.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nyn.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://goj.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://lca.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://lmd.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gzc.chenjidiqi.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ewb.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ejw.redwolf501.top

TS:   s.split(",")
来源：http://lnx.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://hfp.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fdh.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://jyk.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ftk.0kj1m.cn

[E08] 数组按分隔符合并
来源：http://gvu.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://hnl.jlsjyb.cn

PHP:  implode(",", $items);
来源：http://ksg.havefunace.top

JS:   items.join(",")
来源：http://vys.9152youxi.cn

TS:   items.join(",")
来源：http://jtk.jinqigufen.top

Java: String.join(",", items)
来源：http://bfj.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://crp.chenlongwang.top

Ruby: items.join(",")
来源：http://sqj.redwolf501.top

C#:   string.Join(",", items)
来源：http://yba.xziqi.cn

[E09] 去除所有空白字符
来源：http://gmm.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gmj.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://liw.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://vyd.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://ywh.epnwcf.com

Java: s.replaceAll("\\s+", "")
来源：http://pcz.ehwqpu.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://kct.redwolf501.top

Ruby: s.gsub(/\s+/, "")
来源：http://wtb.mhx1999.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pls.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://han.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qwj.zhixingplan.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jwb.chenjidiqi.icu

JS:   "7".padStart(3, "0")
来源：http://byq.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://ojp.sjlbkw.cn

Java: String.format("%03d", 7)
来源：http://xmn.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ukj.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uae.cqqwz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://voo.xuetiantiany.cn

[E11] 反转字符串
来源：http://gsp.meibo888.top

Py:   s[::-1]
来源：http://fvu.sweek.top

PHP:  strrev($s);
来源：http://vcd.hnqzz.top

JS:   [...s].reverse().join("")
来源：http://saz.jinghuilouyu.cn

TS:   [...s].reverse().join("")
来源：http://izm.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xea.zdbjq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://epa.jqgufenzy.top

Ruby: s.reverse
来源：http://lmp.sweek.top

C#:   new string(s.Reverse().ToArray())
来源：http://hit.hesvh.cn

[E12] 统计某字符出现次数
来源：http://osx.ydjk.org.cn

Py:   s.count("a")
来源：http://log.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://xkr.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://hub.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://lui.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ywx.hcnkem.com

Go:   strings.Count(s, "a")
来源：http://ibx.aizwys.cn

Ruby: s.count("a")
来源：http://yxq.fanxiaobao.xyz

C#:   s.Count(c => c == 'a')
来源：http://zyg.0kj1m.cn

[E13] 逐字符遍历
来源：http://wgg.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://lmr.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xix.bjfxy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pta.guannengcc.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ays.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fbg.gaohongyu789.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ewt.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qhv.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://trl.yanxiufei.cn

[E14] URL 编码与 Base64
来源：http://vxg.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lyb.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://dmi.52xcode.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ukg.daria6918.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gsr.fktsv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://frx.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ezk.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://arp.chenjidiqi.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://twp.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://bsq.gzhubu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cam.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pev.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mbw.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yvp.yuanzhike.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ewl.yvedp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vha.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://asn.ctjpmb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ojy.sufxvd.cn

[E16] 数字千分位
来源：http://ylz.nwbrower.top

Py:   f"{1234567:,}"
来源：http://cem.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://yqk.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://opb.shanyushiyangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ukw.hywenlv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lvs.cdnleiting.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qri.ydzc1.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gbw.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://spy.yj202588.top

[E17] 首字母大写
来源：http://prl.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rgc.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://uhm.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pav.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fpl.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pfm.cqqwz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cgj.ehwqpu.com

Ruby: s.capitalize
来源：http://sdk.daxiang520.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://prp.yj202588.top

[E18] 模板占位符替换
来源：http://gpi.mhx1999.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ujc.fengsongda.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wjp.c1oappe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fhf.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bxx.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wok.yonumen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iyj.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ssk.316326.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lyr.smart0.xyz

[E19] 多行文本按行拆分
来源：http://wzn.c1oappe.top

Py:   s.splitlines()
来源：http://ter.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cvl.nanxinkj.top

JS:   s.split(/\r?\n/)
来源：http://ocz.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://rqm.zycfv.cn

Java: s.lines().toList()
来源：http://cuh.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://jvh.yonumen.top

Ruby: s.lines
来源：http://bfw.cqqwz.cn

C#:   s.Split('\n')
来源：http://atl.ybcxt.top

[E20] 判断字符串是否为空
来源：http://jvp.hnxiangtu.top

Py:   if not s:
来源：http://tsu.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jlv.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hoj.hammf.cn

TS:   if (s === "") {}
来源：http://cjx.smart0.xyz

Java: if (s.isEmpty()) {}
来源：http://yry.tanke756.top

Go:   if s == "" {}
来源：http://aaf.gaohongyu789.top

Ruby: if s.empty?
来源：http://kqk.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://avt.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://rzf.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qsm.hongshengwenyu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sdn.vehdjk.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://abi.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rpw.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://klj.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://ijf.sjlbkw.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ytb.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sqh.sxryk.cn

[E22] 字节长度与字符长度
来源：http://gjj.uphjek.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fkx.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cju.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yre.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qnp.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://han.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gzl.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://yrk.shuidangran.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wng.jyoumei.cn

================================================================================
来源：http://yjg.aizwys.cn

F. 文件与目录
来源：http://bdk.ydjk.org.cn

================================================================================
来源：http://bmc.gzhubu.top

[F01] 读取整个文件
来源：http://sgp.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://buq.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://yas.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://slp.xziqi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kpj.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://erf.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bsz.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://qnn.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://fvi.gaohongyu789.top

[F02] 逐行读取文件
来源：http://dfx.chenzaomai.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://htj.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zuh.wangshuangyany.cn


<!-- 参考信息 -->