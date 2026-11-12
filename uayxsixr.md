代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tjt.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ecw.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ofo.tanke756.top

TS:   [...arr];
来源：http://pwa.nanxuanxn.top

Java: new ArrayList<>(list);
来源：http://lmv.jqgufenzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://zgj.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://ftr.hnqzz.top

C#:   new List<int>(list);
来源：http://pkn.epnwcf.com

[D23] reduce 累积计算
来源：http://lmw.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://shv.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lbi.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pej.xziqi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qxn.hesvh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ozc.yanxiufei.cn

Go:   // 手写循环
来源：http://tyn.yfazqb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hqe.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jsn.sufxvd.cn

[D24] 字典 / Map 基本操作
来源：http://rpt.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://plf.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qmx.tianlin.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wun.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://apa.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ojy.dianchejie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wuh.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lms.hnxiangtu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eqt.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://uvg.jlsjyb.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wzv.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wqc.jinyuanbaomall.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dno.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qhr.jinqigufen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nrn.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qyp.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rha.cheryme.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xjk.ehwqpu.com

[D26] 数组转字符串
来源：http://hpb.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://hhh.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://ouz.jqgufenzy.top

JS:   arr.join(", ")
来源：http://vju.havefunace.top

TS:   arr.join(", ")
来源：http://jtg.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://tee.jqgfzy.top

Go:   strings.Join(strs, ", ")
来源：http://rvv.ivvv.top

Ruby: arr.join(", ")
来源：http://yzj.zhoulong.xyz

C#:   string.Join(", ", list)
来源：http://jvo.smart0.xyz

================================================================================
来源：http://yik.meibo888.top

E. 字符串处理
来源：http://lxx.wangdashe.top

================================================================================
来源：http://vga.xinyue.icu

[E01] 拼接字符串
来源：http://caw.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hqu.tanke756.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zrj.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://igw.gaohongyu789.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zgl.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xnm.jinyuanbaomall.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mms.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tcw.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yyb.wangshuangyany.cn

[E02] 重复字符串
来源：http://zdw.snrcjt.cn

Py:   "ab" * 3
来源：http://bgp.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://fap.nwbrower.top

JS:   "ab".repeat(3)
来源：http://sqo.ybcxt.top

TS:   "ab".repeat(3)
来源：http://ira.yueranfly.top

Java: "ab".repeat(3)
来源：http://krd.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://hxn.gogol.net.cn

Ruby: "ab" * 3
来源：http://ehc.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qgt.tianlin.xyz

[E03] 截取子串
来源：http://pjp.jianghu66.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vxu.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wmq.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://abd.fzhhl.top

TS:   s.slice(1, 4)
来源：http://pra.daxiang520.top

Java: s.substring(1, 4)
来源：http://rxh.xuanzx.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hyj.yuxming.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qau.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://npi.feifeiyinyue.top

[E04] 查找子串位置
来源：http://kqu.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://mjb.svipenyu.cn

PHP:  strpos($s, "x");
来源：http://tfo.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hna.sxryk.cn

TS:   s.indexOf("x")
来源：http://xny.hysaishi.cn

Java: s.indexOf("x")
来源：http://pjv.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://esk.fzhhl.top

Ruby: s.index("x")
来源：http://uvi.52xcode.cn

C#:   s.IndexOf("x")
来源：http://mot.cqqwz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://haw.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nec.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zwz.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://psv.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dvp.jiagoushi.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eza.mhx1999.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ogr.yueranfly.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://elp.hesvh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vve.yvedp.cn

[E06] 替换子串
来源：http://tsf.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gwo.yuanzhike.top

PHP:  str_replace("a", "b", $s);
来源：http://cqt.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kkb.meibo888.top

TS:   s.replaceAll("a", "b")
来源：http://lhj.ehwqpu.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wgo.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blx.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qwk.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://jxf.snrcjt.cn

[E07] 按分隔符拆分
来源：http://oxg.xuanzx.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vrj.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fnm.sjlbkw.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://clz.jianghu66.top

TS:   s.split(",")
来源：http://tjd.cucudq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rby.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mnd.cheryme.top

Ruby: s.split(",");  s.split
来源：http://fhe.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tgl.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://gss.feifeiyinyue.top

Py:   ",".join(items)
来源：http://ocv.chenlongwang.top

PHP:  implode(",", $items);
来源：http://zkb.haohaochexian.top

JS:   items.join(",")
来源：http://djg.nwbrower.top

TS:   items.join(",")
来源：http://zhl.iojbl.cn

Java: String.join(",", items)
来源：http://eel.zhaomingkeji.xyz

Go:   strings.Join(items, ",")
来源：http://mmv.epnwcf.com

Ruby: items.join(",")
来源：http://siu.dianchejie.cn

C#:   string.Join(",", items)
来源：http://iev.yueranfly.top

[E09] 去除所有空白字符
来源：http://dlk.aibaodan.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ilj.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lhe.pycfn.com

JS:   s.replace(/\s+/g, "")
来源：http://yab.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://qxr.ybcxt.top

Java: s.replaceAll("\\s+", "")
来源：http://cnj.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ipk.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xdf.pengpengdd.cyou

C#:   Regex.Replace(s, @"\s+", "")
来源：http://igx.jinghuilouyu.cn

[E10] 左侧补零 / 定长填充
来源：http://rcf.cheryme.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bru.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://miw.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://voa.wangshuangyany.cn

TS:   "7".padStart(3, "0")
来源：http://aol.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://sgu.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ims.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kxs.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cla.aizwys.cn

[E11] 反转字符串
来源：http://jbr.uphjek.com

Py:   s[::-1]
来源：http://sbu.ctjpmb.com

PHP:  strrev($s);
来源：http://sgu.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://vuz.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://wfh.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nyu.cdnleiting.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ddu.fehbvm.com

Ruby: s.reverse
来源：http://lem.cashguo.top

C#:   new string(s.Reverse().ToArray())
来源：http://ozf.bjfxy.top

[E12] 统计某字符出现次数
来源：http://bjj.tarul.cn

Py:   s.count("a")
来源：http://lbo.smart0.xyz

PHP:  substr_count($s, "a");
来源：http://axh.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://iiv.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://pwb.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sbt.kuanghao11.cn

Go:   strings.Count(s, "a")
来源：http://dlw.chenzaomai.com

Ruby: s.count("a")
来源：http://ymt.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://ocu.daxiang520.top

[E13] 逐字符遍历
来源：http://ncz.jqgufenzy.top

Py:   for ch in s: print(ch)
来源：http://dko.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pws.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uri.nanxuanxn.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pay.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lfx.yj20258888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fap.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mar.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://opx.hesvh.cn

[E14] URL 编码与 Base64
来源：http://imj.hnqzz.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rvj.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ryf.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rfw.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://efg.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tvv.xuetiantiany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mox.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ckv.quarkkingdee.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wfv.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://ftz.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kqs.ydjk.org.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ypx.hongshengwenyu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zlt.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tne.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rze.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bom.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ixl.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hxw.tian-w.cn

[E16] 数字千分位
来源：http://gin.zdbjq.cn

Py:   f"{1234567:,}"
来源：http://ehn.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://ule.uphjek.com

JS:   (1234567).toLocaleString("en-US")
来源：http://nlu.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qvk.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zol.yuanzhike.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://daa.xuetiantiany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ovl.hammf.cn

C#:   1234567.ToString("N0")
来源：http://ckx.hesvh.cn

[E17] 首字母大写
来源：http://qjs.pycfn.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ffu.jqgfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dnd.shzxlz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vrz.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wlx.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://scs.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jop.fzhhl.top

Ruby: s.capitalize
来源：http://ztl.shanyushiyangtech.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nci.havefunace.top

[E18] 模板占位符替换
来源：http://ntc.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xgh.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rhx.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cfo.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://hvt.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://snk.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://unu.ywan-chungtsiang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dlh.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cdj.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://jzk.tian-w.cn

Py:   s.splitlines()
来源：http://uqy.xinyue.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xky.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://emi.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://yka.zhixingplan.top

Java: s.lines().toList()
来源：http://ioc.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://yup.hywenlv.cn

Ruby: s.lines
来源：http://usm.hnxiangtu.top

C#:   s.Split('\n')
来源：http://olm.jiagoushi.top

[E20] 判断字符串是否为空
来源：http://cys.tian-w.cn

Py:   if not s:
来源：http://cnd.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yzx.316326.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tyt.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://umy.sweek.top

Java: if (s.isEmpty()) {}
来源：http://twt.dashuyun.cn

Go:   if s == "" {}
来源：http://jdd.andypj.xyz

Ruby: if s.empty?
来源：http://par.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ump.shzxlz.cn

[E21] 超长截断加省略号
来源：http://bsw.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://its.jyoumei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bvk.iojbl.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cpt.tanke756.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yhc.nanxuanxn.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gfu.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://dar.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ivz.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nyw.meibo888.top

[E22] 字节长度与字符长度
来源：http://pfp.yuanzhike.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eio.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rrn.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qoe.yvedp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://imw.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://erv.jyoumei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hcj.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://iry.316326.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://spn.yvedp.cn

================================================================================
来源：http://hph.guowangkeji.top

F. 文件与目录
来源：http://ops.nanxuanxn.top

================================================================================
来源：http://ore.dashuyun.cn

[F01] 读取整个文件
来源：http://lcq.shuidangran.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ooy.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://bzd.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ijc.nanxuanxn.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fjg.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xzw.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nws.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://squ.vehdjk.com

C#:   File.ReadAllText("a.txt");
来源：http://ewn.havefunace.top

[F02] 逐行读取文件
来源：http://lpk.shangyingyoupin.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oyy.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fnf.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://euv.jqgufenzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kls.yuxming.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fyf.ywan-chungtsiang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xgg.ehwqpu.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yyh.tanke756.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://apl.bbcook.cn

[F03] 写入文件（覆盖）
来源：http://fpr.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://skj.nanxinkj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cng.yvedp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://djb.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jqz.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pef.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ule.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://cdm.tian-w.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zhd.cashguo.top

[F04] 追加写入文件
来源：http://rpr.gzhubu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ega.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xzw.gaohongyu789.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rgy.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ttk.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://suv.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iio.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kul.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://quj.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://xnw.gzhubu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xkm.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://smu.xingfuxueyuan.xyz

JS:   fs.existsSync("a.txt")
来源：http://miv.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://rzu.jlsjyb.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://slb.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fqq.smart0.xyz

Ruby: File.exist?("a.txt")
来源：http://mro.yongpay.top

C#:   File.Exists("a.txt")
来源：http://sjy.jqgfzy.top

[F06] 删除文件
来源：http://qmy.fzhhl.top

Py:   os.remove("a.txt")
来源：http://brw.yfazqb.com

PHP:  unlink("a.txt");
来源：http://tzy.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://dsv.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://oyi.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vfx.sweek.top

Go:   os.Remove("a.txt")
来源：http://wfl.xinyue.icu


<!-- 参考信息 -->