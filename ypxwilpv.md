代发 wailian999

Java: new ArrayList<>(list);
来源：http://goz.shangyingyoupin.top

Go:   copied := append([]int(nil), arr...)
来源：http://amx.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://oim.daxiang520.top

C#:   new List<int>(list);
来源：http://kpk.tian-w.cn

[D23] reduce 累积计算
来源：http://wlz.yongpay.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tca.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nmj.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xhs.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ici.yvedp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yzj.yj202588.top

Go:   // 手写循环
来源：http://nbh.pycfn.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ccf.zhoulong.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yjt.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://jta.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bhw.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kol.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xal.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jtl.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gmg.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wbu.smart0.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ufe.guowangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yng.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://acp.jiagoushi.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xdo.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rqt.yj20258.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://voq.shzxlz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hch.yongpay.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jxw.sysykeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jkm.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vjj.tian-w.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://stu.iojbl.cn

[D26] 数组转字符串
来源：http://zli.wangshuangyany.cn

Py:   ", ".join(map(str, arr))
来源：http://rlz.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://wzx.yj202588.top

JS:   arr.join(", ")
来源：http://sqo.tanke756.top

TS:   arr.join(", ")
来源：http://jnx.zycfv.cn

Java: String.join(", ", list)
来源：http://ocs.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://hul.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://ybc.hammf.cn

C#:   string.Join(", ", list)
来源：http://nwb.meibo888.top

================================================================================
来源：http://koy.xuetiantiany.cn

E. 字符串处理
来源：http://dot.shanyushiyangtech.top

================================================================================
来源：http://bng.jlsjyb.cn

[E01] 拼接字符串
来源：http://hsa.yuanzhike.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baf.cqqwz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tsa.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oty.vehdjk.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zct.yangfankeji.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uls.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ohy.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rmh.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bii.nwbrower.top

[E02] 重复字符串
来源：http://ajs.sysykeji.top

Py:   "ab" * 3
来源：http://fzq.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://tet.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://lij.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://xbl.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://fok.gaohongyu789.top

Go:   strings.Repeat("ab", 3)
来源：http://mty.svipenyu.cn

Ruby: "ab" * 3
来源：http://que.0kj1m.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nem.xuetiantiany.cn

[E03] 截取子串
来源：http://pte.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zhv.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qke.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pjc.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://kgh.xziqi.cn

Java: s.substring(1, 4)
来源：http://ffd.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://juv.hongshengwenyu.top

Ruby: s[1, 3];  s[1..3]
来源：http://gka.sjlbkw.cn

C#:   s.Substring(1, 3)
来源：http://xcj.shanyushiyangtech.top

[E04] 查找子串位置
来源：http://qjn.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://qny.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://gpw.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eeq.zhixingplan.top

TS:   s.indexOf("x")
来源：http://tns.gogol.net.cn

Java: s.indexOf("x")
来源：http://phh.yonumen.top

Go:   strings.Index(s, "x")
来源：http://anu.jinqigufen.top

Ruby: s.index("x")
来源：http://vpl.hesvh.cn

C#:   s.IndexOf("x")
来源：http://uhg.zhaomingkeji.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://pwl.yueranfly.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ydf.gzhubu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rkj.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ymx.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hgx.birdmap.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://emo.chenzaomai.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rdg.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kdb.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vmg.xingfuxueyuan.xyz

[E06] 替换子串
来源：http://jax.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rsx.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://wzf.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://czx.xylfe.cn

TS:   s.replaceAll("a", "b")
来源：http://lel.0kj1m.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://whx.zdbjq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ten.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ubi.wangdashe.top

C#:   s.Replace("a", "b")
来源：http://egi.yuxming.cn

[E07] 按分隔符拆分
来源：http://gzn.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lip.kuanghao11.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aqf.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://huz.ydjk.org.cn

TS:   s.split(",")
来源：http://nhy.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dov.ivvv.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kgx.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://uev.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lxg.hesvh.cn

[E08] 数组按分隔符合并
来源：http://kru.52xcode.cn

Py:   ",".join(items)
来源：http://qxg.jqgfzy.top

PHP:  implode(",", $items);
来源：http://cuq.yueranfly.top

JS:   items.join(",")
来源：http://wor.shzxlz.cn

TS:   items.join(",")
来源：http://gco.kuanghao11.cn

Java: String.join(",", items)
来源：http://xlz.nanxinkj.top

Go:   strings.Join(items, ",")
来源：http://cki.xylfe.cn

Ruby: items.join(",")
来源：http://uub.tian-w.cn

C#:   string.Join(",", items)
来源：http://sei.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://xpz.guowangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://smt.jinghuilouyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nvx.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://oyh.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://lli.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://ipy.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xer.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://bpt.tian-w.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gkb.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://nni.yj202588.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hez.shangyingyoupin.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cny.tanke756.top

JS:   "7".padStart(3, "0")
来源：http://nkw.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://fqp.sysykeji.top

Java: String.format("%03d", 7)
来源：http://eim.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://tkc.chenlongwang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mnm.hongshengwenyu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qlg.pycfn.com

[E11] 反转字符串
来源：http://tsd.0kj1m.cn

Py:   s[::-1]
来源：http://ruz.aibaodan.cn

PHP:  strrev($s);
来源：http://nhz.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://xiz.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://eov.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uyz.nanxinkj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ofq.xylfe.cn

Ruby: s.reverse
来源：http://hmo.aibaodan.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zwn.pengpengdd.cyou

[E12] 统计某字符出现次数
来源：http://cmn.ydjk.org.cn

Py:   s.count("a")
来源：http://eef.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://vwo.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://lig.zycfv.cn

TS:   s.split("a").length - 1
来源：http://ala.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mfw.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://nci.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://vog.shuidangran.top

C#:   s.Count(c => c == 'a')
来源：http://xdn.zhongyouzk.top

[E13] 逐字符遍历
来源：http://dgl.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://bgw.xziqi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hox.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wyo.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kzt.hfpthk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://odf.meibo888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://laq.zhiwuduotai.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jwx.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jru.pycfn.com

[E14] URL 编码与 Base64
来源：http://ngd.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hqz.wangdashe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://for.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ibs.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://drm.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jme.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jlz.zhixingplan.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zvs.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pth.jqgfzy.top

[E15] HTML 转义 / 反转义
来源：http://ncl.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://uxd.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tjj.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://miv.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://vii.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tnz.aibaodan.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cos.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gyt.yj20258.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rzr.gotoacloud.top

[E16] 数字千分位
来源：http://xmu.ivvv.top

Py:   f"{1234567:,}"
来源：http://dbj.cashguo.top

PHP:  number_format(1234567);
来源：http://vpx.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://bxt.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://tmg.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nlv.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qrn.dashuyun.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://frm.gotoacloud.top

C#:   1234567.ToString("N0")
来源：http://gon.feifeiyinyue.top

[E17] 首字母大写
来源：http://wpc.nanxinkj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dka.iojbl.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vbp.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ozx.jinyuanbaomall.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fri.mhx1999.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xqx.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eqw.meibo888.top

Ruby: s.capitalize
来源：http://tat.zdqjudy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://isj.cqqwz.cn

[E18] 模板占位符替换
来源：http://cgk.gaohongyu789.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://syk.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mui.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zso.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yjz.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vmj.fehbvm.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://olt.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mse.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gho.52xcode.cn

[E19] 多行文本按行拆分
来源：http://ixb.dianchejie.cn

Py:   s.splitlines()
来源：http://tnh.haohaochexian.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vsm.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://pvv.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://ezx.52xcode.cn

Java: s.lines().toList()
来源：http://rit.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://qwx.cdnleiting.top

Ruby: s.lines
来源：http://pgo.feifeiyinyue.top

C#:   s.Split('\n')
来源：http://mcw.xuanzx.com

[E20] 判断字符串是否为空
来源：http://wle.gogol.net.cn

Py:   if not s:
来源：http://yal.feifeiyinyue.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cyv.yj20258.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hay.ppjwa.cn

TS:   if (s === "") {}
来源：http://lla.316326.xyz

Java: if (s.isEmpty()) {}
来源：http://ffq.andypj.xyz

Go:   if s == "" {}
来源：http://wcf.0kj1m.cn

Ruby: if s.empty?
来源：http://kvl.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://avs.52xcode.cn

[E21] 超长截断加省略号
来源：http://fis.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ean.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://myz.zhiwuduotai.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eee.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aqc.jianghu66.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qip.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://xrb.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://akv.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xhx.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://otu.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pqj.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ppf.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uxy.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://toa.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tiu.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://egq.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://syd.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://byo.ppjwa.cn

================================================================================
来源：http://yfe.zhengqikj.top

F. 文件与目录
来源：http://szs.jinqigufen.top

================================================================================
来源：http://mvw.xziqi.cn

[F01] 读取整个文件
来源：http://idw.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ssx.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://ajs.meibo888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rdn.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jxi.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://msi.xziqi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cwb.fengsongda.top

Ruby: File.read("a.txt")
来源：http://vis.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://cix.c1oappe.top

[F02] 逐行读取文件
来源：http://koe.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ppu.fehbvm.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cso.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dof.jinqigufen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rny.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bce.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dcl.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ghs.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yit.0kj1m.cn

[F03] 写入文件（覆盖）
来源：http://bdc.cheryme.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fsw.sweek.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cts.jinqigufen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tup.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kjq.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dox.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aaj.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://ftl.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yrs.yanxiufei.cn

[F04] 追加写入文件
来源：http://rqv.hongshengwenyu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yvq.bjfxy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fmg.jinghuilouyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rep.shanyushiyangtech.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jwb.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zty.meibo888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lpa.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jcu.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vst.9152youxi.cn

[F05] 判断文件或目录是否存在
来源：http://wnj.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ivu.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://lfg.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://aeg.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://ouc.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xaj.nanxuanxn.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bst.tian-w.cn

Ruby: File.exist?("a.txt")
来源：http://cyw.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://jvd.316326.xyz

[F06] 删除文件
来源：http://xfi.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://eki.yfazqb.com

PHP:  unlink("a.txt");
来源：http://wtv.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://naf.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://hul.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ovd.wangdashe.top

Go:   os.Remove("a.txt")
来源：http://uny.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://ioz.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://zot.gzhubu.top

[F07] 创建目录（含多级）
来源：http://bus.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zvy.zhiwuduotai.top


<!-- 参考信息 -->