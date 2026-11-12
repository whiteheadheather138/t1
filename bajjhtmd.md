代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lso.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ezf.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ero.yanxiufei.cn

TS:   [...arr];
来源：http://usz.yfazqb.com

Java: new ArrayList<>(list);
来源：http://vbb.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://zjf.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://ylv.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://tzb.daria6918.cn

[D23] reduce 累积计算
来源：http://fow.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wce.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kcy.shuidangran.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xgf.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zfw.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://uqz.cashguo.top

Go:   // 手写循环
来源：http://pxr.xylfe.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pjn.yfazqb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ukw.yj202588.top

[D24] 字典 / Map 基本操作
来源：http://thf.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ywx.tianlin.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mdv.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qxw.iojbl.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bor.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://khe.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fyn.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aan.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://usz.fehbvm.com

[D25] Set 集合去重与交并差
来源：http://cyw.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pal.haohaochexian.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dub.vqdsnc.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fqz.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rco.kuanghao11.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://isv.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gyy.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://btj.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://spq.ctjpmb.com

[D26] 数组转字符串
来源：http://rrz.epnwcf.com

Py:   ", ".join(map(str, arr))
来源：http://cwr.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://jgs.kuanghao11.cn

JS:   arr.join(", ")
来源：http://faa.ybcxt.top

TS:   arr.join(", ")
来源：http://kvx.xinyue.icu

Java: String.join(", ", list)
来源：http://yzr.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://scu.bjfxy.top

Ruby: arr.join(", ")
来源：http://fhr.cdnleiting.top

C#:   string.Join(", ", list)
来源：http://xso.zhiwuduotai.top

================================================================================
来源：http://pjd.yuxming.cn

E. 字符串处理
来源：http://ozg.hongshengwenyu.top

================================================================================
来源：http://lae.jyoumei.cn

[E01] 拼接字符串
来源：http://xav.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rwk.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wbx.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bqz.ivvv.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jba.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://liv.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pfb.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lwj.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zpt.aizwys.cn

[E02] 重复字符串
来源：http://zjm.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://dmw.guannengcc.top

PHP:  str_repeat("ab", 3);
来源：http://iso.pycfn.com

JS:   "ab".repeat(3)
来源：http://yng.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://vei.zycfv.cn

Java: "ab".repeat(3)
来源：http://xpv.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://zkc.xinyue.icu

Ruby: "ab" * 3
来源：http://ydk.svipenyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sja.cucudq.cn

[E03] 截取子串
来源：http://pnm.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uoe.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jyw.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://old.dashuyun.cn

TS:   s.slice(1, 4)
来源：http://cfc.smart0.xyz

Java: s.substring(1, 4)
来源：http://idy.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cqs.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eju.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://xik.zycfv.cn

[E04] 查找子串位置
来源：http://nrd.andypj.xyz

Py:   s.find("x");  s.index("x")
来源：http://asp.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://yuf.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xxz.hysaishi.cn

TS:   s.indexOf("x")
来源：http://rpu.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://ohc.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://eco.sjlbkw.cn

Ruby: s.index("x")
来源：http://miz.0kj1m.cn

C#:   s.IndexOf("x")
来源：http://mqj.bbcook.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pvg.quarkkingdee.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nxw.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tnl.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://arw.daxiang520.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dlb.jinqigfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vye.chenzaomai.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hjq.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://buv.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hgi.yfazqb.com

[E06] 替换子串
来源：http://kjc.zhijiandao.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://anp.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://fsc.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jem.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://gzr.jyoumei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://chc.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://imp.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rhn.yj202588.top

C#:   s.Replace("a", "b")
来源：http://hgj.vqdsnc.cn

[E07] 按分隔符拆分
来源：http://eis.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://clv.shanyushiyangtech.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iml.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://loo.jlsjyb.cn

TS:   s.split(",")
来源：http://lct.ivvv.top

Java: s.split(",");  s.split("\\s+")
来源：http://vby.guowangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rxj.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://vek.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vbt.cheryme.top

[E08] 数组按分隔符合并
来源：http://kgn.hcnkem.com

Py:   ",".join(items)
来源：http://ggx.ybcxt.top

PHP:  implode(",", $items);
来源：http://jur.sxryk.cn

JS:   items.join(",")
来源：http://xbd.shzxlz.cn

TS:   items.join(",")
来源：http://lpo.aizwys.cn

Java: String.join(",", items)
来源：http://kmd.bbcook.cn

Go:   strings.Join(items, ",")
来源：http://vlq.vqdsnc.cn

Ruby: items.join(",")
来源：http://oxa.shuidangran.top

C#:   string.Join(",", items)
来源：http://krs.nanxinkj.top

[E09] 去除所有空白字符
来源：http://ouw.ivvv.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mhu.pycfn.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mrh.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://dqe.quarkkingdee.top

TS:   s.replace(/\s+/g, "")
来源：http://apo.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://znd.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qju.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://iha.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fur.yongpay.top

[E10] 左侧补零 / 定长填充
来源：http://oha.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tqw.jqgufenzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ngf.jlsjyb.cn

JS:   "7".padStart(3, "0")
来源：http://cwx.yvedp.cn

TS:   "7".padStart(3, "0")
来源：http://xcl.sjlbkw.cn

Java: String.format("%03d", 7)
来源：http://xyc.bjfxy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lps.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sur.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ywp.xylfe.cn

[E11] 反转字符串
来源：http://qvk.sweek.top

Py:   s[::-1]
来源：http://pnl.vqdsnc.cn

PHP:  strrev($s);
来源：http://vox.ppjwa.cn

JS:   [...s].reverse().join("")
来源：http://ggf.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://dgv.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rjd.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://oel.fzhhl.top

Ruby: s.reverse
来源：http://wiv.tianlin.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ndt.hnqzz.top

[E12] 统计某字符出现次数
来源：http://sib.nanxinkj.top

Py:   s.count("a")
来源：http://xgv.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://grs.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://zcv.yj20258888.top

TS:   s.split("a").length - 1
来源：http://hfi.hnxiangtu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kbv.hongshengwenyu.top

Go:   strings.Count(s, "a")
来源：http://ndt.yj202588.top

Ruby: s.count("a")
来源：http://cqy.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://yfe.yj20258.top

[E13] 逐字符遍历
来源：http://gcd.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://dac.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kth.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://qjk.ehwqpu.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://qhl.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kpb.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hdx.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tcc.xuetiantiany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yqf.gzhubu.top

[E14] URL 编码与 Base64
来源：http://khr.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://shz.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wih.bbcook.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ncy.chenlongwang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://foo.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://otx.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yxf.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wis.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jlv.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://jzq.chenjidiqi.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://xvf.iojbl.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pua.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ljy.zhengqikj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jlb.sysykeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://awo.guannengcc.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ejb.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cmj.zhongyouzk.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lqy.yvedp.cn

[E16] 数字千分位
来源：http://yer.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://tuf.gzhubu.top

PHP:  number_format(1234567);
来源：http://egu.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://iwl.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://qap.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://izx.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bbo.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hnu.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://syp.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://dmo.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qov.zdbjq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xso.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bnf.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://prh.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fsh.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iuf.snrcjt.cn

Ruby: s.capitalize
来源：http://bba.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xcy.smart0.xyz

[E18] 模板占位符替换
来源：http://ain.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://luq.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ktq.yangfankeji.com

JS:   tpl.replaceAll("{name}", name)
来源：http://vtb.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yrs.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qgb.smart0.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wuk.tian-w.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ngm.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ity.yueranfly.top

[E19] 多行文本按行拆分
来源：http://jtb.zhengqikj.top

Py:   s.splitlines()
来源：http://ulf.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lls.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://ebb.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://xpp.ctjpmb.com

Java: s.lines().toList()
来源：http://yjc.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://qkw.zdqjudy.top

Ruby: s.lines
来源：http://uip.ctjpmb.com

C#:   s.Split('\n')
来源：http://qxt.tarul.cn

[E20] 判断字符串是否为空
来源：http://uhw.smart0.xyz

Py:   if not s:
来源：http://otr.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ith.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yoe.fanxiaobao.xyz

TS:   if (s === "") {}
来源：http://wis.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://hmb.mhx1999.top

Go:   if s == "" {}
来源：http://yfw.jqgufenzy.top

Ruby: if s.empty?
来源：http://yln.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yby.xuetiantiany.cn

[E21] 超长截断加省略号
来源：http://kyy.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zlz.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blb.jqgfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://efg.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ftm.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vbm.tanke756.top

Go:   // 按 rune 判断长度后截断
来源：http://szd.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pdb.aizwys.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ego.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://die.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cac.ivvv.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sva.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dpw.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vnk.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cbt.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mpc.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://feh.yueranfly.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kyu.yueranfly.top

================================================================================
来源：http://htw.ywan-chungtsiang.top

F. 文件与目录
来源：http://xiq.cucudq.cn

================================================================================
来源：http://elw.yueranfly.top

[F01] 读取整个文件
来源：http://sru.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wwo.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://fly.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wrc.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://itj.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jll.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gww.epnwcf.com

Ruby: File.read("a.txt")
来源：http://mjh.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://gzf.zhixingplan.top

[F02] 逐行读取文件
来源：http://gku.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jor.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://epx.bbcook.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://arv.chenlongwang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lse.shuidangran.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://utz.gaohongyu789.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://znv.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kpx.jiagoushi.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cye.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://lez.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://woh.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nta.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ows.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vzi.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zgy.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wid.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://afw.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zlz.9152youxi.cn

[F04] 追加写入文件
来源：http://daz.gaohongyu789.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uet.ivvv.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ifa.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ctd.quarkkingdee.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zxo.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cgh.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cfo.jiagoushi.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mdo.jinghuilouyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mqv.dashuyun.cn

[F05] 判断文件或目录是否存在
来源：http://vga.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dnm.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://hcc.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://jof.xuetiantiany.cn

TS:   fs.existsSync("a.txt")
来源：http://rsw.0kj1m.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kbj.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fms.daria6918.cn

Ruby: File.exist?("a.txt")
来源：http://orz.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://gpd.aibaodan.cn

[F06] 删除文件
来源：http://oej.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://suv.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://oiw.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vlt.xuetiantiany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xgr.hywenlv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dmz.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://huk.sweek.top


<!-- 参考信息 -->