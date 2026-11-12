代发 wailian999

[D19] 按字段分组
来源：http://dbb.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xlo.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jlv.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://brw.yuanzhike.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://oog.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ogg.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://mfc.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oyw.sjlbkw.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jpv.sweek.top

[D20] 统计每个元素出现次数
来源：http://zmk.xylfe.cn

Py:   Counter(arr)
来源：http://jjn.fanxiaobao.xyz

PHP:  array_count_values($arr);
来源：http://dzy.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ozz.cqqwz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://clr.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qeh.yueranfly.top

Go:   // 手写 map[T]int
来源：http://imm.yonumen.top

Ruby: arr.tally
来源：http://hqz.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://syy.yj202588.top

[D21] 判断是否包含某元素
来源：http://kff.hcnkem.com

Py:   x in arr
来源：http://ofr.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://hku.jqgufenzy.top

JS:   arr.includes(x)
来源：http://tbw.ppjwa.cn

TS:   arr.includes(x)
来源：http://zfk.sxryk.cn

Java: list.contains(x)
来源：http://hwj.0kj1m.cn

Go:   slices.Contains(arr, x)
来源：http://qla.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://dps.shanyushiyangtech.top

C#:   list.Contains(x)
来源：http://wsp.iojbl.cn

[D22] 复制数组（避免共享引用）
来源：http://zga.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hep.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://snw.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lpe.quarkkingdee.top

TS:   [...arr];
来源：http://frf.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://jvg.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://nqn.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://unc.nwbrower.top

C#:   new List<int>(list);
来源：http://oym.yj20258.top

[D23] reduce 累积计算
来源：http://rfm.epnwcf.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://won.316326.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://quy.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rba.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wcx.epnwcf.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://mxu.hfpthk.cn

Go:   // 手写循环
来源：http://jrj.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ums.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zkb.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://kuv.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cml.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ufq.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://exv.yanxiufei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://drs.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://afp.epnwcf.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xue.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rxv.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uaf.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://ktl.andypj.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://svt.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cgz.jiagoushi.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ihp.ywan-chungtsiang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gan.yongpay.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aqa.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fld.bbcook.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bhr.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ado.tanke756.top

[D26] 数组转字符串
来源：http://tmd.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://zei.epnwcf.com

PHP:  implode(", ", $arr);
来源：http://nhl.zhoulong.xyz

JS:   arr.join(", ")
来源：http://fvc.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://gnt.9152youxi.cn

Java: String.join(", ", list)
来源：http://kka.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://lvc.xylfe.cn

Ruby: arr.join(", ")
来源：http://fnk.shuidangran.top

C#:   string.Join(", ", list)
来源：http://gww.daria6918.cn

================================================================================
来源：http://ulc.xingfuxueyuan.xyz

E. 字符串处理
来源：http://enf.chenjidiqi.icu

================================================================================
来源：http://yhy.hammf.cn

[E01] 拼接字符串
来源：http://dqo.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mhc.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zeb.xuanzx.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://voh.9152youxi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sfb.hesvh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pkh.316326.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iih.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hen.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://shl.nwbrower.top

[E02] 重复字符串
来源：http://voq.vqdsnc.cn

Py:   "ab" * 3
来源：http://lap.gaohongyu789.top

PHP:  str_repeat("ab", 3);
来源：http://ypr.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://svk.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://myl.c1oappe.top

Java: "ab".repeat(3)
来源：http://kqm.ppjwa.cn

Go:   strings.Repeat("ab", 3)
来源：http://wqe.shuidangran.top

Ruby: "ab" * 3
来源：http://jyf.jinyuanbaomall.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bhb.mhx1999.top

[E03] 截取子串
来源：http://cyl.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aca.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xnx.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pgd.redwolf501.top

TS:   s.slice(1, 4)
来源：http://aae.jinqigfzy.top

Java: s.substring(1, 4)
来源：http://ify.sweek.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pwf.hongshengwenyu.top

Ruby: s[1, 3];  s[1..3]
来源：http://tyq.nanxuanxn.top

C#:   s.Substring(1, 3)
来源：http://imz.jlsjyb.cn

[E04] 查找子串位置
来源：http://jtf.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://jbm.nwbrower.top

PHP:  strpos($s, "x");
来源：http://azd.sweek.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wgl.yongpay.top

TS:   s.indexOf("x")
来源：http://hkt.cdnleiting.top

Java: s.indexOf("x")
来源：http://mcg.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://owt.wangshuangyany.cn

Ruby: s.index("x")
来源：http://fbr.ctjpmb.com

C#:   s.IndexOf("x")
来源：http://biy.hnqzz.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bey.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tdo.shanyushiyangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jzy.quarkkingdee.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://igc.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vnh.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uzi.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://joq.ydjk.org.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qiq.bbcook.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mtn.sxryk.cn

[E06] 替换子串
来源：http://uqw.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bet.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://bsr.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ksh.xinyue.icu

TS:   s.replaceAll("a", "b")
来源：http://usq.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fyr.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ier.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://clk.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://chh.ppjwa.cn

[E07] 按分隔符拆分
来源：http://sbi.ybcxt.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mps.cdnleiting.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wgc.quarkkingdee.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xuq.sxryk.cn

TS:   s.split(",")
来源：http://xpg.sysykeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://rxs.fktsv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gpi.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://vee.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://chh.cheryme.top

[E08] 数组按分隔符合并
来源：http://hge.daria6918.cn

Py:   ",".join(items)
来源：http://nub.yj20258888.top

PHP:  implode(",", $items);
来源：http://xkj.daxiang520.top

JS:   items.join(",")
来源：http://zfw.zdqjudy.top

TS:   items.join(",")
来源：http://gel.gaohongyu789.top

Java: String.join(",", items)
来源：http://ype.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://xnj.sysykeji.top

Ruby: items.join(",")
来源：http://hmb.nanxinkj.top

C#:   string.Join(",", items)
来源：http://rzw.sysykeji.top

[E09] 去除所有空白字符
来源：http://kuv.andypj.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kkq.xuanzx.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://scm.ydjk.org.cn

JS:   s.replace(/\s+/g, "")
来源：http://phh.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://nrk.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://znx.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fmv.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://meo.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fpw.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://zsf.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yzm.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zgc.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://xlm.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://jzl.hesvh.cn

Java: String.format("%03d", 7)
来源：http://mno.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://spb.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yzo.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vfr.meibo888.top

[E11] 反转字符串
来源：http://ujx.shzxlz.cn

Py:   s[::-1]
来源：http://ddt.ppjwa.cn

PHP:  strrev($s);
来源：http://rgx.ydjk.org.cn

JS:   [...s].reverse().join("")
来源：http://odw.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://dqo.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qxu.gogol.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oms.jqgfzy.top

Ruby: s.reverse
来源：http://upa.jinghuilouyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tcu.fktsv.cn

[E12] 统计某字符出现次数
来源：http://izd.sxryk.cn

Py:   s.count("a")
来源：http://vxw.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://zqs.c1oappe.top

JS:   s.split("a").length - 1
来源：http://jjt.hesvh.cn

TS:   s.split("a").length - 1
来源：http://mjh.zhengqikj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wdi.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://bpp.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://dws.sysykeji.top

C#:   s.Count(c => c == 'a')
来源：http://vhm.fzhhl.top

[E13] 逐字符遍历
来源：http://rei.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://zxl.hfpthk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cua.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bxy.vehdjk.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://voo.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pqw.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://thh.dashuyun.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vbv.ivvv.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pmy.dashuyun.cn

[E14] URL 编码与 Base64
来源：http://hak.ehwqpu.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mdv.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jlc.ybcxt.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jab.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zoe.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ffa.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hsy.yonumen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://viw.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iwo.gaohongyu789.top

[E15] HTML 转义 / 反转义
来源：http://ukz.cucudq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cpm.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://udg.zhiwuduotai.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nml.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pkg.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xar.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jci.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://brl.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wel.dashuyun.cn

[E16] 数字千分位
来源：http://xvr.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://ail.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://iht.fzhhl.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jac.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://qcp.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bxt.gaohongyu789.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hlk.yj20258.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://syk.hammf.cn

C#:   1234567.ToString("N0")
来源：http://rph.nanxinkj.top

[E17] 首字母大写
来源：http://ugh.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ymz.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hgo.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ros.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lcr.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ejh.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hfh.vqdsnc.cn

Ruby: s.capitalize
来源：http://dug.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bps.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://jgi.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qvq.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cjq.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hll.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://nrc.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kpw.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ttx.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ejv.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cjy.daxiang520.top

[E19] 多行文本按行拆分
来源：http://pwu.xziqi.cn

Py:   s.splitlines()
来源：http://ism.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qdn.gotoacloud.top

JS:   s.split(/\r?\n/)
来源：http://iht.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://nye.hnxiangtu.top

Java: s.lines().toList()
来源：http://jly.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://ftu.hysaishi.cn

Ruby: s.lines
来源：http://cbj.zhiwuduotai.top

C#:   s.Split('\n')
来源：http://mwt.birdmap.top

[E20] 判断字符串是否为空
来源：http://ngm.jinqigufen.top

Py:   if not s:
来源：http://rzg.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dcx.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hgi.xinyue.icu

TS:   if (s === "") {}
来源：http://lcw.jqgufenzy.top

Java: if (s.isEmpty()) {}
来源：http://vbn.ydzc1.top

Go:   if s == "" {}
来源：http://crd.zhengqikj.top

Ruby: if s.empty?
来源：http://rra.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ktx.sweek.top

[E21] 超长截断加省略号
来源：http://iol.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mtu.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pom.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zzc.smart0.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ajk.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wmh.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://tuo.smart0.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ikz.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rtx.yongpay.top

[E22] 字节长度与字符长度
来源：http://ngy.yvedp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bza.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ehi.fanxiaobao.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://riz.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gaq.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ffj.meibo888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kwt.zdbjq.cn

Ruby: s.bytesize;  s.length
来源：http://kxf.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lle.smart0.xyz

================================================================================
来源：http://hvs.jqgufenzy.top

F. 文件与目录
来源：http://cjp.chenzaomai.com

================================================================================
来源：http://lse.cucudq.cn

[F01] 读取整个文件
来源：http://ofe.zhiwuduotai.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ciw.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://hry.nwbrower.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xgb.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rcm.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://viu.havefunace.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kfd.sufxvd.cn

Ruby: File.read("a.txt")
来源：http://mkm.zdbjq.cn

C#:   File.ReadAllText("a.txt");
来源：http://wtx.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://fsn.bbcook.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zja.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pbw.cashguo.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dcl.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://trr.316326.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fmy.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wgo.jqgfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bcs.yueranfly.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jla.tian-w.cn

[F03] 写入文件（覆盖）
来源：http://div.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nda.hnqzz.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kmt.ybcxt.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pyn.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jcy.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zvv.shuidangran.top


<!-- 参考信息 -->