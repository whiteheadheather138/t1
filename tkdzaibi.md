代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zcx.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sso.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jbg.shzxlz.cn

Go:   // 手写循环累加
来源：http://emy.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xaw.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://zru.jianghu66.top

[D17] 最大值与最小值
来源：http://myl.quarkkingdee.top

Py:   max(arr);  min(arr)
来源：http://vus.smart0.xyz

PHP:  max($arr);  min($arr);
来源：http://ext.sufxvd.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rjr.cheryme.top

TS:   Math.max(...arr);
来源：http://axp.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dfy.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://btm.sweek.top

Ruby: arr.max;  arr.min
来源：http://qwk.aibaodan.cn

C#:   list.Max();  list.Min()
来源：http://mll.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://gdx.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://etw.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://shr.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kbx.jianghu66.top

TS:   nested.flat();
来源：http://yre.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qke.dashuyun.cn

Go:   // 手写双层循环
来源：http://cai.tarul.cn

Ruby: nested.flatten
来源：http://sce.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://sqs.xziqi.cn

[D19] 按字段分组
来源：http://ohc.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ykl.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vox.svipenyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qcv.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aif.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eqd.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://lgq.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ayw.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uyx.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://fad.zdbjq.cn

Py:   Counter(arr)
来源：http://dvb.shuidangran.top

PHP:  array_count_values($arr);
来源：http://niw.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yxc.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bhi.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cgd.yuxming.cn

Go:   // 手写 map[T]int
来源：http://ywv.cheryme.top

Ruby: arr.tally
来源：http://gzy.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ovr.nanxinkj.top

[D21] 判断是否包含某元素
来源：http://yhd.aibaodan.cn

Py:   x in arr
来源：http://kti.sufxvd.cn

PHP:  in_array($x, $arr, true);
来源：http://wuv.hfpthk.cn

JS:   arr.includes(x)
来源：http://zgv.yanxiufei.cn

TS:   arr.includes(x)
来源：http://uqv.gaohongyu789.top

Java: list.contains(x)
来源：http://fev.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://dbw.redwolf501.top

Ruby: arr.include?(x)
来源：http://bzz.sufxvd.cn

C#:   list.Contains(x)
来源：http://nan.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://twz.gogol.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aqm.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gbu.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bhe.meibo888.top

TS:   [...arr];
来源：http://jsj.shanyushiyangkeji.top

Java: new ArrayList<>(list);
来源：http://cwm.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://unc.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://ipf.gogol.net.cn

C#:   new List<int>(list);
来源：http://qwr.xuanzx.com

[D23] reduce 累积计算
来源：http://hmt.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://umu.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cnz.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xze.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gdn.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jso.ivvv.top

Go:   // 手写循环
来源：http://ezo.jqgufenzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qpw.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nbw.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://uhc.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oam.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://abh.tanke756.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yuu.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pvt.ehwqpu.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://phe.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ejf.chenzaomai.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kjg.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qkm.fktsv.cn

[D25] Set 集合去重与交并差
来源：http://pom.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hvu.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uvz.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gyz.nanxuanxn.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jpl.yj202588.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ofa.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wmo.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gdu.yanxiufei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fxo.tanke756.top

[D26] 数组转字符串
来源：http://sdt.ivvv.top

Py:   ", ".join(map(str, arr))
来源：http://awb.zycfv.cn

PHP:  implode(", ", $arr);
来源：http://dtn.jinqigufen.top

JS:   arr.join(", ")
来源：http://ozr.nanxuanxn.top

TS:   arr.join(", ")
来源：http://jtq.ivvv.top

Java: String.join(", ", list)
来源：http://jme.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://csd.yonumen.top

Ruby: arr.join(", ")
来源：http://voh.daria6918.cn

C#:   string.Join(", ", list)
来源：http://gkz.chenzaomai.com

================================================================================
来源：http://kho.nanxuanxn.top

E. 字符串处理
来源：http://npx.andypj.xyz

================================================================================
来源：http://yxv.epnwcf.com

[E01] 拼接字符串
来源：http://zct.daria6918.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gxo.aibaodan.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cwv.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://czi.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sun.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rzq.yueranfly.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qpg.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://syw.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ezc.zhijiandao.cn

[E02] 重复字符串
来源：http://lnl.guannengcc.top

Py:   "ab" * 3
来源：http://vmm.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://asj.yonumen.top

JS:   "ab".repeat(3)
来源：http://tsg.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://jmo.yuxming.cn

Java: "ab".repeat(3)
来源：http://tmu.xziqi.cn

Go:   strings.Repeat("ab", 3)
来源：http://ypl.sufxvd.cn

Ruby: "ab" * 3
来源：http://cck.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fnn.ydzc1.top

[E03] 截取子串
来源：http://odl.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nov.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gov.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://roi.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://dur.hammf.cn

Java: s.substring(1, 4)
来源：http://ckj.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gua.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ovb.cashguo.top

C#:   s.Substring(1, 3)
来源：http://wfd.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://jks.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://ggm.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://klj.snrcjt.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zvq.zycfv.cn

TS:   s.indexOf("x")
来源：http://iwt.zhoulong.xyz

Java: s.indexOf("x")
来源：http://izr.tanke756.top

Go:   strings.Index(s, "x")
来源：http://eqg.dianchejie.cn

Ruby: s.index("x")
来源：http://hvw.gzhubu.top

C#:   s.IndexOf("x")
来源：http://erw.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hms.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qvw.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zdg.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wcd.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lre.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cnm.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://etl.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hec.meibo888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lmc.hcnkem.com

[E06] 替换子串
来源：http://jbq.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fnd.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://lqm.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jtc.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://jwd.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xgq.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mww.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qxr.zhoulong.xyz

C#:   s.Replace("a", "b")
来源：http://bjp.sweek.top

[E07] 按分隔符拆分
来源：http://wjz.jqgufenzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wsd.aibaodan.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tuz.ydjk.org.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mlf.sysykeji.top

TS:   s.split(",")
来源：http://nhn.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kdb.daria6918.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qvu.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://jmd.jinqigufen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xee.sysykeji.top

[E08] 数组按分隔符合并
来源：http://hhq.gotoacloud.top

Py:   ",".join(items)
来源：http://gjp.yonumen.top

PHP:  implode(",", $items);
来源：http://urq.andypj.xyz

JS:   items.join(",")
来源：http://rky.ehwqpu.com

TS:   items.join(",")
来源：http://gkm.hesvh.cn

Java: String.join(",", items)
来源：http://wrp.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://ctk.dianchejie.cn

Ruby: items.join(",")
来源：http://jxd.zdqjudy.top

C#:   string.Join(",", items)
来源：http://rvf.ydzc1.top

[E09] 去除所有空白字符
来源：http://gge.aibaodan.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zet.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://skm.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://gjp.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://bny.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://vuk.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://elq.sysykeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://vcx.yonumen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lyl.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://tli.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lna.nanxinkj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://daz.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://zeo.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://vua.hesvh.cn

Java: String.format("%03d", 7)
来源：http://dxe.jianghu66.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kei.cashguo.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pgy.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lad.mhx1999.top

[E11] 反转字符串
来源：http://cst.zycfv.cn

Py:   s[::-1]
来源：http://spb.xylfe.cn

PHP:  strrev($s);
来源：http://ytf.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://ryr.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://zwj.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bhj.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wsv.meibo888.top

Ruby: s.reverse
来源：http://kus.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vgt.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://tlj.hammf.cn

Py:   s.count("a")
来源：http://dlb.shanyushiyangtech.top

PHP:  substr_count($s, "a");
来源：http://jot.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://boy.fengsongda.top

TS:   s.split("a").length - 1
来源：http://zme.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nww.yonumen.top

Go:   strings.Count(s, "a")
来源：http://kjx.jyoumei.cn

Ruby: s.count("a")
来源：http://xfv.feifeiyinyue.top

C#:   s.Count(c => c == 'a')
来源：http://two.cheryme.top

[E13] 逐字符遍历
来源：http://xwp.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://xbb.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uzg.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oqr.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fgh.iojbl.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ols.yj20258888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ani.cashguo.top

Ruby: s.each_char { |ch| puts ch }
来源：http://onk.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wzg.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://lbw.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nwl.sweek.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dlr.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://itg.hfpthk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xrl.ywan-chungtsiang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ast.pycfn.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xhc.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bcn.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kwa.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://ran.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rko.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zxb.hesvh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://woe.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gim.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vqp.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://izx.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mzg.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rlw.jqgufenzy.top

[E16] 数字千分位
来源：http://cmo.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://sqp.yueranfly.top

PHP:  number_format(1234567);
来源：http://hla.9152youxi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ysw.xuanzx.com

TS:   (1234567).toLocaleString("en-US")
来源：http://omu.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xsz.yuxming.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://evu.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zqb.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://ynb.ywan-chungtsiang.top

[E17] 首字母大写
来源：http://rng.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vhv.xziqi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yqr.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zfu.zhixingplan.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://obh.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ztz.quarkkingdee.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mgo.gotoacloud.top

Ruby: s.capitalize
来源：http://kwa.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://woh.sjlbkw.cn

[E18] 模板占位符替换
来源：http://ppa.vqdsnc.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yzh.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aqx.tianlin.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://wde.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://twf.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ckr.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wzo.0kj1m.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://man.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oeb.bbcook.cn

[E19] 多行文本按行拆分
来源：http://jrc.hywenlv.cn

Py:   s.splitlines()
来源：http://bvy.yanxiufei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qkb.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://psf.jiagoushi.top

TS:   s.split(/\r?\n/)
来源：http://wjc.jinqigfzy.top

Java: s.lines().toList()
来源：http://awk.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://yph.gotoacloud.top

Ruby: s.lines
来源：http://hxm.uphjek.com

C#:   s.Split('\n')
来源：http://xby.shanyushiyangtech.top

[E20] 判断字符串是否为空
来源：http://les.hysaishi.cn

Py:   if not s:
来源：http://lfd.xuanzx.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tqf.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://thh.zhaomingkeji.xyz

TS:   if (s === "") {}
来源：http://rff.fktsv.cn

Java: if (s.isEmpty()) {}
来源：http://umd.mhx1999.top

Go:   if s == "" {}
来源：http://ibs.0kj1m.cn

Ruby: if s.empty?
来源：http://tgh.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yzk.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://pgz.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://llu.birdmap.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://whf.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oic.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sfg.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rsm.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://miq.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ztj.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fdp.vehdjk.com

[E22] 字节长度与字符长度
来源：http://pxd.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jly.zdqjudy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qxi.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sbe.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://arm.meibo888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rqm.jyoumei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dtr.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://ruh.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gzq.52xcode.cn

================================================================================
来源：http://xqs.quarkkingdee.top

F. 文件与目录
来源：http://ulj.cucudq.cn

================================================================================
来源：http://vuz.ybcxt.top


<!-- 参考信息 -->