代发 wailian999

Java: new ArrayList<>(list);
来源：http://rbc.ctjpmb.com

Go:   copied := append([]int(nil), arr...)
来源：http://efp.xylfe.cn

Ruby: arr.dup;  arr.clone
来源：http://vgh.cashguo.top

C#:   new List<int>(list);
来源：http://yro.snrcjt.cn

[D23] reduce 累积计算
来源：http://pnk.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wjo.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jtj.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ikt.52xcode.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://faw.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cjy.yonumen.top

Go:   // 手写循环
来源：http://izu.xuanzx.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gjm.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hpd.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://xef.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uwi.fktsv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dbg.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ayc.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qgl.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vqr.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bau.zhixingplan.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pwk.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gpr.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://tdj.fanxiaobao.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sok.yueranfly.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mti.guowangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qos.shuidangran.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://woj.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://irc.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://olx.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://keh.aibaodan.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://frm.tanke756.top

[D26] 数组转字符串
来源：http://xwg.hongshengwenyu.top

Py:   ", ".join(map(str, arr))
来源：http://waq.yj202588.top

PHP:  implode(", ", $arr);
来源：http://kuk.zhaomingkeji.xyz

JS:   arr.join(", ")
来源：http://afk.jiagoushi.top

TS:   arr.join(", ")
来源：http://hlj.sweek.top

Java: String.join(", ", list)
来源：http://fqq.fktsv.cn

Go:   strings.Join(strs, ", ")
来源：http://asr.cdnleiting.top

Ruby: arr.join(", ")
来源：http://kui.iojbl.cn

C#:   string.Join(", ", list)
来源：http://kmi.guowangkeji.top

================================================================================
来源：http://owz.yvedp.cn

E. 字符串处理
来源：http://qup.vqdsnc.cn

================================================================================
来源：http://kpp.gotoacloud.top

[E01] 拼接字符串
来源：http://iwg.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xbt.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vuv.nwbrower.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tfk.0kj1m.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://itx.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ayj.yvedp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ffe.316326.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://muq.havefunace.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://anl.zhengqikj.top

[E02] 重复字符串
来源：http://yvc.fengsongda.top

Py:   "ab" * 3
来源：http://mfb.zhijiandao.cn

PHP:  str_repeat("ab", 3);
来源：http://aqj.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://oww.tian-w.cn

TS:   "ab".repeat(3)
来源：http://wwc.cucudq.cn

Java: "ab".repeat(3)
来源：http://mib.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://cbv.yuxming.cn

Ruby: "ab" * 3
来源：http://yoj.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eem.birdmap.top

[E03] 截取子串
来源：http://nbw.shanyushiyangtech.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://brb.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vam.shanyushiyangtech.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qrr.ywan-chungtsiang.top

TS:   s.slice(1, 4)
来源：http://fnh.ydjk.org.cn

Java: s.substring(1, 4)
来源：http://mzh.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xnl.yangfankeji.com

Ruby: s[1, 3];  s[1..3]
来源：http://cwj.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://lxc.316326.xyz

[E04] 查找子串位置
来源：http://zho.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://kln.smart0.xyz

PHP:  strpos($s, "x");
来源：http://dsr.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ysc.snrcjt.cn

TS:   s.indexOf("x")
来源：http://khy.gaohongyu789.top

Java: s.indexOf("x")
来源：http://vwk.havefunace.top

Go:   strings.Index(s, "x")
来源：http://juv.xylfe.cn

Ruby: s.index("x")
来源：http://tgu.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://lft.jinghuilouyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pmf.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iqe.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pnj.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tvc.gzhubu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cwg.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://alj.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nik.nanxinkj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hqi.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uie.9152youxi.cn

[E06] 替换子串
来源：http://qds.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bhr.yangfankeji.com

PHP:  str_replace("a", "b", $s);
来源：http://hwc.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://urj.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://fqo.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ynv.andypj.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bkp.mhx1999.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ecx.jqgfzy.top

C#:   s.Replace("a", "b")
来源：http://qip.cashguo.top

[E07] 按分隔符拆分
来源：http://ela.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rin.nanxinkj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jze.zhengqikj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://acj.zhixingplan.top

TS:   s.split(",")
来源：http://els.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://gor.52xcode.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lxq.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://iap.guannengcc.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pgv.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://hqv.redwolf501.top

Py:   ",".join(items)
来源：http://rer.wangdashe.top

PHP:  implode(",", $items);
来源：http://aoj.mhx1999.top

JS:   items.join(",")
来源：http://iup.yuanzhike.top

TS:   items.join(",")
来源：http://rvw.hysaishi.cn

Java: String.join(",", items)
来源：http://hdj.bbcook.cn

Go:   strings.Join(items, ",")
来源：http://hqy.vehdjk.com

Ruby: items.join(",")
来源：http://pbe.yueranfly.top

C#:   string.Join(",", items)
来源：http://cjg.tian-w.cn

[E09] 去除所有空白字符
来源：http://lak.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tho.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qof.hesvh.cn

JS:   s.replace(/\s+/g, "")
来源：http://cko.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://yxb.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://ozz.smart0.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://hka.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nkd.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://obo.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://cpo.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gfj.yfazqb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jau.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://slh.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://omm.aizwys.cn

Java: String.format("%03d", 7)
来源：http://kbr.ppjwa.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mim.hammf.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fwt.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bjf.nanxuanxn.top

[E11] 反转字符串
来源：http://nod.hesvh.cn

Py:   s[::-1]
来源：http://svl.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://jml.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://adk.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://gbv.dianchejie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mnh.nanxuanxn.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zor.jianghu66.top

Ruby: s.reverse
来源：http://fuk.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://cwr.fzhhl.top

[E12] 统计某字符出现次数
来源：http://dkl.cashguo.top

Py:   s.count("a")
来源：http://mlb.zdqjudy.top

PHP:  substr_count($s, "a");
来源：http://nro.yj20258.top

JS:   s.split("a").length - 1
来源：http://zzy.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://edn.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mis.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://vyn.tanke756.top

Ruby: s.count("a")
来源：http://xry.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://yud.9152youxi.cn

[E13] 逐字符遍历
来源：http://qqm.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://ftz.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qmb.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://yor.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://akc.yueranfly.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lty.cashguo.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eda.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lcy.chenjidiqi.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://klz.epnwcf.com

[E14] URL 编码与 Base64
来源：http://hzy.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zbo.zhengqikj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lfi.tanke756.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://css.9152youxi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iiw.zdqjudy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pei.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kwv.nwbrower.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rzn.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://onb.xuanzx.com

[E15] HTML 转义 / 反转义
来源：http://isb.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://svh.zhaomingkeji.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uzc.chenjidiqi.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xbu.mhx1999.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kxf.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dih.hcnkem.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vec.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xee.sufxvd.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cwi.gotoacloud.top

[E16] 数字千分位
来源：http://wcj.nanxuanxn.top

Py:   f"{1234567:,}"
来源：http://uub.hnqzz.top

PHP:  number_format(1234567);
来源：http://zye.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tcm.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://dqr.shuidangran.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://otp.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://was.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pmi.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://uhj.ybcxt.top

[E17] 首字母大写
来源：http://krc.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mgw.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://bin.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://stk.sxryk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bul.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nhl.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pxp.zhengqikj.top

Ruby: s.capitalize
来源：http://fie.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jac.yuxming.cn

[E18] 模板占位符替换
来源：http://ked.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wrc.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vev.ivvv.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cfe.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://vym.jinyuanbaomall.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jnk.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qgq.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ybj.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bsy.yueranfly.top

[E19] 多行文本按行拆分
来源：http://vgu.hywenlv.cn

Py:   s.splitlines()
来源：http://vgm.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jkf.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://fkc.bjfxy.top

TS:   s.split(/\r?\n/)
来源：http://oni.dianchejie.cn

Java: s.lines().toList()
来源：http://fpw.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://nox.dashuyun.cn

Ruby: s.lines
来源：http://ixz.hywenlv.cn

C#:   s.Split('\n')
来源：http://hkw.jiagoushi.top

[E20] 判断字符串是否为空
来源：http://qxa.bbcook.cn

Py:   if not s:
来源：http://geb.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fev.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://opa.sysykeji.top

TS:   if (s === "") {}
来源：http://pni.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://cjq.pycfn.com

Go:   if s == "" {}
来源：http://ean.ydjk.org.cn

Ruby: if s.empty?
来源：http://vnm.snrcjt.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vyk.316326.xyz

[E21] 超长截断加省略号
来源：http://wuh.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zpn.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://clt.sweek.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wtf.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://srw.cqqwz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ofn.cqqwz.cn

Go:   // 按 rune 判断长度后截断
来源：http://efx.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gou.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://trh.cheryme.top

[E22] 字节长度与字符长度
来源：http://wnj.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mnm.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hmz.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dnp.fehbvm.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hyw.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sgi.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jws.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://wxb.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pvm.shanyushiyangkeji.top

================================================================================
来源：http://mrv.svipenyu.cn

F. 文件与目录
来源：http://ire.quarkkingdee.top

================================================================================
来源：http://fgy.9152youxi.cn

[F01] 读取整个文件
来源：http://xca.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mpg.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://ekn.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uos.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ced.sysykeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zaz.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hjm.cucudq.cn

Ruby: File.read("a.txt")
来源：http://acc.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://gxf.ybcxt.top

[F02] 逐行读取文件
来源：http://geg.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lje.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vzh.daxiang520.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yqh.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hxo.316326.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jpa.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vzr.tian-w.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nwj.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://amn.tian-w.cn

[F03] 写入文件（覆盖）
来源：http://pyz.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gea.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://skg.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://duc.xylfe.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ben.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ssu.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kes.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://nsl.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ctb.vqdsnc.cn

[F04] 追加写入文件
来源：http://owu.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://odd.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ybm.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kgr.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mcy.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://thm.cdnleiting.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dlv.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://suu.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ago.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://hdf.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://idj.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://xjk.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://wvc.dashuyun.cn

TS:   fs.existsSync("a.txt")
来源：http://uvf.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ltw.zhijiandao.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rua.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://itj.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://gmd.redwolf501.top

[F06] 删除文件
来源：http://usu.sweek.top

Py:   os.remove("a.txt")
来源：http://kkf.yangfankeji.com

PHP:  unlink("a.txt");
来源：http://jar.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wdh.ydjk.org.cn

TS:   fs.unlinkSync("a.txt")
来源：http://isr.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nak.52xcode.cn

Go:   os.Remove("a.txt")
来源：http://szl.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://dvq.yj202588.top

C#:   File.Delete("a.txt");
来源：http://xih.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://ztd.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://knv.jinqigfzy.top


<!-- 参考信息 -->