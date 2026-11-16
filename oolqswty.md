代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qmd.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://xjj.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://imt.hfpthk.cn

[D18] 扁平化嵌套数组
来源：http://gig.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ijf.bjfxy.top

PHP:  array_merge(...$nested);
来源：http://pzh.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yej.zhongyouzk.top

TS:   nested.flat();
来源：http://fim.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tbs.yj20258888.top

Go:   // 手写双层循环
来源：http://cba.vqdsnc.cn

Ruby: nested.flatten
来源：http://dms.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yvl.shzxlz.cn

[D19] 按字段分组
来源：http://ypk.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sfr.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eef.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://izy.iojbl.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jyi.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wzz.ppjwa.cn

Go:   // 手写 map[string][]T
来源：http://ehh.andypj.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://zzz.cheryme.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bbh.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://tso.jinqigfzy.top

Py:   Counter(arr)
来源：http://jsz.haohaochexian.top

PHP:  array_count_values($arr);
来源：http://yam.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bhe.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pcy.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://atb.jinghuilouyu.cn

Go:   // 手写 map[T]int
来源：http://dsv.jyoumei.cn

Ruby: arr.tally
来源：http://xjh.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qep.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://vux.sweek.top

Py:   x in arr
来源：http://azi.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://paf.jinqigfzy.top

JS:   arr.includes(x)
来源：http://rwc.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://yre.shangyingyoupin.top

Java: list.contains(x)
来源：http://rpq.birdmap.top

Go:   slices.Contains(arr, x)
来源：http://cze.daxiang520.top

Ruby: arr.include?(x)
来源：http://zjp.vqdsnc.cn

C#:   list.Contains(x)
来源：http://ryk.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://ggk.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pql.yvedp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qba.meibo888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tcw.zhoulong.xyz

TS:   [...arr];
来源：http://zjf.yvedp.cn

Java: new ArrayList<>(list);
来源：http://grv.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://qzj.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://eki.mhx1999.top

C#:   new List<int>(list);
来源：http://jpk.cdnleiting.top

[D23] reduce 累积计算
来源：http://vhe.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ivz.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cws.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uec.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kdx.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nks.jianghu66.top

Go:   // 手写循环
来源：http://zxw.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zjm.zhijiandao.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jej.pycfn.com

[D24] 字典 / Map 基本操作
来源：http://jis.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dug.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hci.cucudq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uhz.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bwl.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iib.tian-w.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://srx.quarkkingdee.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vqp.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rxo.guowangkeji.top

[D25] Set 集合去重与交并差
来源：http://nhc.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jam.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ltb.52xcode.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kse.haohaochexian.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lbg.chenjidiqi.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yhu.yueranfly.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uis.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nvr.sxryk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://geh.ybcxt.top

[D26] 数组转字符串
来源：http://pla.mhx1999.top

Py:   ", ".join(map(str, arr))
来源：http://qho.jiagoushi.top

PHP:  implode(", ", $arr);
来源：http://wzk.uphjek.com

JS:   arr.join(", ")
来源：http://xmr.gaohongyu789.top

TS:   arr.join(", ")
来源：http://sxy.sxryk.cn

Java: String.join(", ", list)
来源：http://ylc.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://flb.fengsongda.top

Ruby: arr.join(", ")
来源：http://mgu.havefunace.top

C#:   string.Join(", ", list)
来源：http://vvu.redwolf501.top

================================================================================
来源：http://jip.yangfankeji.com

E. 字符串处理
来源：http://tog.sysykeji.top

================================================================================
来源：http://zzj.zycfv.cn

[E01] 拼接字符串
来源：http://qby.jinqigufen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nbf.bbcook.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://axu.sweek.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mvl.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hqs.jinyuanbaomall.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hhc.sjlbkw.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mku.hnxiangtu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rmb.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cfc.jqgufenzy.top

[E02] 重复字符串
来源：http://diu.guowangkeji.top

Py:   "ab" * 3
来源：http://ahj.tanke756.top

PHP:  str_repeat("ab", 3);
来源：http://brw.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://xzo.bbcook.cn

TS:   "ab".repeat(3)
来源：http://reo.yangfankeji.com

Java: "ab".repeat(3)
来源：http://pqd.uphjek.com

Go:   strings.Repeat("ab", 3)
来源：http://yqa.tanke756.top

Ruby: "ab" * 3
来源：http://noi.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hub.cdnleiting.top

[E03] 截取子串
来源：http://kdk.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fve.iojbl.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gpm.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dbj.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://wne.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://wjr.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aar.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://dcb.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://iab.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://roq.zhiwuduotai.top

Py:   s.find("x");  s.index("x")
来源：http://ysc.epnwcf.com

PHP:  strpos($s, "x");
来源：http://lgb.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ftp.sufxvd.cn

TS:   s.indexOf("x")
来源：http://tsb.vehdjk.com

Java: s.indexOf("x")
来源：http://tsf.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://iuu.xuanzx.com

Ruby: s.index("x")
来源：http://mnt.andypj.xyz

C#:   s.IndexOf("x")
来源：http://vbc.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://fwd.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://njf.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aes.cucudq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qir.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nnj.svipenyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fxa.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dlv.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nwy.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fni.0kj1m.cn

[E06] 替换子串
来源：http://usd.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://svi.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://ucx.hongshengwenyu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sto.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://hxf.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hxm.hfpthk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nyo.cashguo.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zws.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://zyz.ydzc1.top

[E07] 按分隔符拆分
来源：http://ort.chenzaomai.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://acv.daria6918.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xjn.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jrn.52xcode.cn

TS:   s.split(",")
来源：http://qlj.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://dyb.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ekc.ivvv.top

Ruby: s.split(",");  s.split
来源：http://uji.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cfi.daxiang520.top

[E08] 数组按分隔符合并
来源：http://thk.guannengcc.top

Py:   ",".join(items)
来源：http://bjb.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://tpl.yj20258.top

JS:   items.join(",")
来源：http://ffn.sweek.top

TS:   items.join(",")
来源：http://ykh.ydjk.org.cn

Java: String.join(",", items)
来源：http://sot.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://cln.ywan-chungtsiang.top

Ruby: items.join(",")
来源：http://khj.svipenyu.cn

C#:   string.Join(",", items)
来源：http://sgq.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://ssj.ehwqpu.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://udb.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nww.xingfuxueyuan.xyz

JS:   s.replace(/\s+/g, "")
来源：http://jbh.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://yql.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://gdt.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fou.hnxiangtu.top

Ruby: s.gsub(/\s+/, "")
来源：http://gqv.feifeiyinyue.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zmc.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://fcb.jyoumei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lcf.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bcu.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://noh.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://ztj.gogol.net.cn

Java: String.format("%03d", 7)
来源：http://zxu.9152youxi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xqz.ctjpmb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fzf.smart0.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tdy.xuanzx.com

[E11] 反转字符串
来源：http://eec.cqqwz.cn

Py:   s[::-1]
来源：http://ebx.tarul.cn

PHP:  strrev($s);
来源：http://gso.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://dcf.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://fgg.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pud.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://btl.yanxiufei.cn

Ruby: s.reverse
来源：http://apy.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://nfv.yj20258.top

[E12] 统计某字符出现次数
来源：http://kgg.wangdashe.top

Py:   s.count("a")
来源：http://tdb.feifeiyinyue.top

PHP:  substr_count($s, "a");
来源：http://eir.gaohongyu789.top

JS:   s.split("a").length - 1
来源：http://biz.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://hhb.hongshengwenyu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jyr.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://kwk.fanxiaobao.xyz

Ruby: s.count("a")
来源：http://uwe.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://tqq.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://qqk.wangshuangyany.cn

Py:   for ch in s: print(ch)
来源：http://tqm.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kqg.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://knt.nwbrower.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qgy.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mri.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pfb.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rrc.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://crv.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://ism.fengsongda.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://akh.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ece.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aab.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ljn.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tyd.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wgy.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qqz.meibo888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pdq.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://zwe.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hux.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eaa.daxiang520.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wmt.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zon.dashuyun.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pgf.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bzc.zdqjudy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yde.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oyb.wangshuangyany.cn

[E16] 数字千分位
来源：http://hlk.jianghu66.top

Py:   f"{1234567:,}"
来源：http://pxu.tanke756.top

PHP:  number_format(1234567);
来源：http://hxe.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hjh.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://sem.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kvc.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rjj.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yak.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://gay.tanke756.top

[E17] 首字母大写
来源：http://nvf.smart0.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hru.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xrk.aibaodan.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zru.zhiwuduotai.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ntf.zhoulong.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rve.fehbvm.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wvc.aibaodan.cn

Ruby: s.capitalize
来源：http://rxi.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gwm.xinyue.icu

[E18] 模板占位符替换
来源：http://qmc.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pzv.gaohongyu789.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dxj.hcnkem.com

JS:   tpl.replaceAll("{name}", name)
来源：http://sjt.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jao.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cer.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ygt.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dmz.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ods.yueranfly.top

[E19] 多行文本按行拆分
来源：http://bvb.sysykeji.top

Py:   s.splitlines()
来源：http://kwm.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wai.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://hhu.shanyushiyangkeji.top

TS:   s.split(/\r?\n/)
来源：http://tzk.xingfuxueyuan.xyz

Java: s.lines().toList()
来源：http://cjf.smart0.xyz

Go:   strings.Split(s, "\n")
来源：http://bfr.yongpay.top

Ruby: s.lines
来源：http://dma.sufxvd.cn

C#:   s.Split('\n')
来源：http://clt.zycfv.cn

[E20] 判断字符串是否为空
来源：http://lfr.nanxuanxn.top

Py:   if not s:
来源：http://ayk.fengsongda.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://phu.shzxlz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://weh.vehdjk.com

TS:   if (s === "") {}
来源：http://xoz.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://xui.aizwys.cn

Go:   if s == "" {}
来源：http://jsl.shzxlz.cn

Ruby: if s.empty?
来源：http://hiz.xingfuxueyuan.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xgm.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://eci.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pvd.xinyue.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wjx.jqgufenzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ryk.ppjwa.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lhi.jiagoushi.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lvj.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://whj.andypj.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vub.xingfuxueyuan.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qib.sxryk.cn

[E22] 字节长度与字符长度
来源：http://fvt.yuanzhike.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://okt.gaohongyu789.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://umb.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ztl.zhaomingkeji.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://scl.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jme.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vpe.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://nne.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rde.hnqzz.top

================================================================================
来源：http://imc.feifeiyinyue.top

F. 文件与目录
来源：http://pac.chenlongwang.top

================================================================================
来源：http://vxe.yj202588.top

[F01] 读取整个文件
来源：http://pni.cdnleiting.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hos.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://nmz.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://icr.vehdjk.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cds.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://dqz.xuetiantiany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oxr.xziqi.cn

Ruby: File.read("a.txt")
来源：http://mzp.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://nfo.dashuyun.cn

[F02] 逐行读取文件
来源：http://vst.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dup.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uym.meibo888.top


<!-- 参考信息 -->