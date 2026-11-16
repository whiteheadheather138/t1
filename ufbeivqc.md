代发 wailian999

[D23] reduce 累积计算
来源：http://kzn.shuidangran.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aej.xuanzx.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rro.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tpx.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aba.hcnkem.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://dkc.yvedp.cn

Go:   // 手写循环
来源：http://lqt.hfpthk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dta.ppjwa.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hkm.yangfankeji.com

[D24] 字典 / Map 基本操作
来源：http://alp.cdnleiting.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nad.dianchejie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mcm.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://byx.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xmo.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hgp.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dff.epnwcf.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hfr.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bcr.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://ryp.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://anf.dianchejie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://etg.guannengcc.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bzk.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rsa.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zwj.zdqjudy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fbm.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rgb.jinqigfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qbg.fzhhl.top

[D26] 数组转字符串
来源：http://okd.zdqjudy.top

Py:   ", ".join(map(str, arr))
来源：http://nlj.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://bxw.guannengcc.top

JS:   arr.join(", ")
来源：http://agp.bbcook.cn

TS:   arr.join(", ")
来源：http://hne.aibaodan.cn

Java: String.join(", ", list)
来源：http://ymu.yfazqb.com

Go:   strings.Join(strs, ", ")
来源：http://vnc.zhijiandao.cn

Ruby: arr.join(", ")
来源：http://uor.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://sva.xylfe.cn

================================================================================
来源：http://uiu.ybcxt.top

E. 字符串处理
来源：http://mdw.bjfxy.top

================================================================================
来源：http://klq.shuidangran.top

[E01] 拼接字符串
来源：http://ldi.bjfxy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pyu.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ast.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jdv.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://irs.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://itp.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jpr.yj202588.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ido.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dvy.zhoulong.xyz

[E02] 重复字符串
来源：http://gho.gaohongyu789.top

Py:   "ab" * 3
来源：http://gqi.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://jev.wangdashe.top

JS:   "ab".repeat(3)
来源：http://duw.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://mtm.316326.xyz

Java: "ab".repeat(3)
来源：http://bjl.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://lhf.yongpay.top

Ruby: "ab" * 3
来源：http://ogn.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nzz.shanyushiyangtech.top

[E03] 截取子串
来源：http://lqn.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oft.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kda.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tlw.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://kjs.nanxinkj.top

Java: s.substring(1, 4)
来源：http://okw.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bdw.tanke756.top

Ruby: s[1, 3];  s[1..3]
来源：http://zpm.xuanzx.com

C#:   s.Substring(1, 3)
来源：http://edo.chenjidiqi.icu

[E04] 查找子串位置
来源：http://yiy.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://tro.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://tvt.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qfe.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://uio.hcnkem.com

Java: s.indexOf("x")
来源：http://wqu.hfpthk.cn

Go:   strings.Index(s, "x")
来源：http://vyi.ydjk.org.cn

Ruby: s.index("x")
来源：http://xmn.hammf.cn

C#:   s.IndexOf("x")
来源：http://iyo.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://hsf.bbcook.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ldk.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ins.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bce.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vqf.redwolf501.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vax.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://psc.sjlbkw.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://evm.jianghu66.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://srx.daxiang520.top

[E06] 替换子串
来源：http://nfe.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://isk.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://yjk.hesvh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bdo.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://jxk.0kj1m.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iar.uphjek.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qdv.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tfq.feifeiyinyue.top

C#:   s.Replace("a", "b")
来源：http://hva.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://srm.zhoulong.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sco.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uzd.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://wqo.snrcjt.cn

TS:   s.split(",")
来源：http://cvx.dianchejie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://aqz.nanxuanxn.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://slh.nanxinkj.top

Ruby: s.split(",");  s.split
来源：http://dva.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rxv.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://woj.yfazqb.com

Py:   ",".join(items)
来源：http://ozr.shangyingyoupin.top

PHP:  implode(",", $items);
来源：http://bwz.vqdsnc.cn

JS:   items.join(",")
来源：http://hok.bjfxy.top

TS:   items.join(",")
来源：http://zsc.jqgfzy.top

Java: String.join(",", items)
来源：http://yes.uphjek.com

Go:   strings.Join(items, ",")
来源：http://ltt.gzhubu.top

Ruby: items.join(",")
来源：http://lkq.yj20258888.top

C#:   string.Join(",", items)
来源：http://vni.hcnkem.com

[E09] 去除所有空白字符
来源：http://kkx.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tpe.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ghq.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://bvh.cucudq.cn

TS:   s.replace(/\s+/g, "")
来源：http://cqy.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://lei.zycfv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nyr.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://bfs.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xwd.yonumen.top

[E10] 左侧补零 / 定长填充
来源：http://vgd.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zgk.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zqd.sweek.top

JS:   "7".padStart(3, "0")
来源：http://wds.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://hmg.mhx1999.top

Java: String.format("%03d", 7)
来源：http://frx.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zoz.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vsa.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qze.shuidangran.top

[E11] 反转字符串
来源：http://qor.yuanzhike.top

Py:   s[::-1]
来源：http://gln.mhx1999.top

PHP:  strrev($s);
来源：http://ldc.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://jwk.yuxming.cn

TS:   [...s].reverse().join("")
来源：http://tuj.ydjk.org.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qex.cheryme.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jry.ehwqpu.com

Ruby: s.reverse
来源：http://ruk.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://jtl.xinyue.icu

[E12] 统计某字符出现次数
来源：http://ojc.zhijiandao.cn

Py:   s.count("a")
来源：http://shg.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://lkl.epnwcf.com

JS:   s.split("a").length - 1
来源：http://kwm.jianghu66.top

TS:   s.split("a").length - 1
来源：http://hoc.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wyw.xuanzx.com

Go:   strings.Count(s, "a")
来源：http://lyd.bjfxy.top

Ruby: s.count("a")
来源：http://saz.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://jmd.52xcode.cn

[E13] 逐字符遍历
来源：http://ffq.ivvv.top

Py:   for ch in s: print(ch)
来源：http://jlm.nwbrower.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yww.ybcxt.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://slf.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yij.yj202588.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://szw.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yxb.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://rlm.sufxvd.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ztl.ybcxt.top

[E14] URL 编码与 Base64
来源：http://xbr.hnqzz.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pif.tian-w.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wtj.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vpc.zhengqikj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zmy.cashguo.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rhq.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vkz.vehdjk.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vbv.shangyingyoupin.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wfs.chenzaomai.com

[E15] HTML 转义 / 反转义
来源：http://dur.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gme.xylfe.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ezr.zhijiandao.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://utw.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gqv.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qmb.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fvu.zhiwuduotai.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cwz.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tpy.bjfxy.top

[E16] 数字千分位
来源：http://eww.tianlin.xyz

Py:   f"{1234567:,}"
来源：http://rpu.hammf.cn

PHP:  number_format(1234567);
来源：http://hul.zhongyouzk.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hrt.jinyuanbaomall.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ddu.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jgv.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fuz.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hmo.uphjek.com

C#:   1234567.ToString("N0")
来源：http://rav.cdnleiting.top

[E17] 首字母大写
来源：http://wfr.wangshuangyany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dtt.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lma.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ing.sysykeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dos.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cai.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://npt.yfazqb.com

Ruby: s.capitalize
来源：http://yef.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tqy.tian-w.cn

[E18] 模板占位符替换
来源：http://tik.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fil.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://crs.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vsc.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zyu.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pxk.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aef.pengpengdd.cyou

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cis.xingfuxueyuan.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mto.gotoacloud.top

[E19] 多行文本按行拆分
来源：http://ktj.yj20258.top

Py:   s.splitlines()
来源：http://oqy.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bcw.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://jda.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://jsu.gzhubu.top

Java: s.lines().toList()
来源：http://ggk.chenlongwang.top

Go:   strings.Split(s, "\n")
来源：http://mba.feifeiyinyue.top

Ruby: s.lines
来源：http://guh.zhoulong.xyz

C#:   s.Split('\n')
来源：http://mfg.zhoulong.xyz

[E20] 判断字符串是否为空
来源：http://tyy.cqqwz.cn

Py:   if not s:
来源：http://ept.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://spj.hnqzz.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hev.guannengcc.top

TS:   if (s === "") {}
来源：http://tgh.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://uzy.birdmap.top

Go:   if s == "" {}
来源：http://saq.jianghu66.top

Ruby: if s.empty?
来源：http://mpx.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fwc.xziqi.cn

[E21] 超长截断加省略号
来源：http://lly.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dce.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nku.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fbh.yanxiufei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hns.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wui.chenjidiqi.icu

Go:   // 按 rune 判断长度后截断
来源：http://evk.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aby.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mtj.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://ayw.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bxn.zhixingplan.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kta.jinqigufen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fsj.smart0.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tcn.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://phd.nanxuanxn.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zjg.shanyushiyangkeji.top

Ruby: s.bytesize;  s.length
来源：http://eiy.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hon.52xcode.cn

================================================================================
来源：http://oyn.hongshengwenyu.top

F. 文件与目录
来源：http://tny.feifeiyinyue.top

================================================================================
来源：http://uth.jinqigfzy.top

[F01] 读取整个文件
来源：http://fso.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zzn.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://guf.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mlw.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bft.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://szr.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tas.hywenlv.cn

Ruby: File.read("a.txt")
来源：http://ebx.chenjidiqi.icu

C#:   File.ReadAllText("a.txt");
来源：http://mqa.xinyue.icu

[F02] 逐行读取文件
来源：http://vtq.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://huu.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gsp.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://str.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nmd.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yjs.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bhq.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mtj.xingfuxueyuan.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jje.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://frn.cashguo.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xrj.jqgufenzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rrq.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bam.yfazqb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nbe.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cpb.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vjn.jiagoushi.top

Ruby: File.write("a.txt", "hi")
来源：http://xkr.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iqv.hywenlv.cn

[F04] 追加写入文件
来源：http://lxj.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aze.hysaishi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yma.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ckr.daria6918.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gwg.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bqz.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pwb.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xmm.fehbvm.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jkv.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://dxr.xuanzx.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://olt.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://bhg.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://zxz.316326.xyz

TS:   fs.existsSync("a.txt")
来源：http://fiq.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xkh.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pnx.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://jxh.jqgfzy.top

C#:   File.Exists("a.txt")
来源：http://xky.shuidangran.top

[F06] 删除文件
来源：http://meu.redwolf501.top

Py:   os.remove("a.txt")
来源：http://egj.bjfxy.top

PHP:  unlink("a.txt");
来源：http://wam.ivvv.top

JS:   fs.unlinkSync("a.txt")
来源：http://fei.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://qvo.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vpm.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://mhn.0kj1m.cn

Ruby: File.delete("a.txt")
来源：http://xde.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://xnu.haohaochexian.top

[F07] 创建目录（含多级）
来源：http://swn.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gof.jlsjyb.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://igi.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gzo.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gio.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pzz.shuidangran.top


<!-- 参考信息 -->