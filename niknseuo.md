代发 wailian999

Java: new ArrayList<>(list);
来源：http://tmu.xinyue.icu

Go:   copied := append([]int(nil), arr...)
来源：http://ijj.zhixingplan.top

Ruby: arr.dup;  arr.clone
来源：http://uxf.cashguo.top

C#:   new List<int>(list);
来源：http://mif.uphjek.com

[D23] reduce 累积计算
来源：http://iqh.fktsv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gyr.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://opf.316326.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eol.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pho.xingfuxueyuan.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://tar.cheryme.top

Go:   // 手写循环
来源：http://nbj.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uqj.fanxiaobao.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oac.vqdsnc.cn

[D24] 字典 / Map 基本操作
来源：http://mpq.zhengqikj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jsy.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://abg.ivvv.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bjp.hnqzz.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sbq.fengsongda.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aib.kuanghao11.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oph.tarul.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cgo.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xki.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://ies.kuanghao11.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://idn.jyoumei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sta.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mcq.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hcn.fzhhl.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://axh.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xng.bbcook.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qqx.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rce.hammf.cn

[D26] 数组转字符串
来源：http://uck.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://opu.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://bed.kuanghao11.cn

JS:   arr.join(", ")
来源：http://nif.birdmap.top

TS:   arr.join(", ")
来源：http://cpd.fktsv.cn

Java: String.join(", ", list)
来源：http://zej.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://usd.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://glb.fzhhl.top

C#:   string.Join(", ", list)
来源：http://yma.zhijiandao.cn

================================================================================
来源：http://qgj.daria6918.cn

E. 字符串处理
来源：http://xdb.shzxlz.cn

================================================================================
来源：http://lxv.sjlbkw.cn

[E01] 拼接字符串
来源：http://lvz.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pzn.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wbb.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://acr.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jgu.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gkz.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ukt.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mhz.ybcxt.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vrs.52xcode.cn

[E02] 重复字符串
来源：http://akg.ybcxt.top

Py:   "ab" * 3
来源：http://fhz.bbcook.cn

PHP:  str_repeat("ab", 3);
来源：http://ndi.mhx1999.top

JS:   "ab".repeat(3)
来源：http://isp.smart0.xyz

TS:   "ab".repeat(3)
来源：http://ywo.wangdashe.top

Java: "ab".repeat(3)
来源：http://pwl.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://kin.jinqigufen.top

Ruby: "ab" * 3
来源：http://vlm.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wvn.hysaishi.cn

[E03] 截取子串
来源：http://frz.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dva.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sqk.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cld.xziqi.cn

TS:   s.slice(1, 4)
来源：http://dzz.cucudq.cn

Java: s.substring(1, 4)
来源：http://spw.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kwk.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://jpw.shanyushiyangtech.top

C#:   s.Substring(1, 3)
来源：http://its.fengsongda.top

[E04] 查找子串位置
来源：http://hcs.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://ckb.guannengcc.top

PHP:  strpos($s, "x");
来源：http://dsz.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ncs.sweek.top

TS:   s.indexOf("x")
来源：http://ffr.sysykeji.top

Java: s.indexOf("x")
来源：http://jyb.0kj1m.cn

Go:   strings.Index(s, "x")
来源：http://yim.9152youxi.cn

Ruby: s.index("x")
来源：http://ydi.uphjek.com

C#:   s.IndexOf("x")
来源：http://xul.9152youxi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://grz.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tya.cheryme.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jya.jiagoushi.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jdq.nanxuanxn.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qfa.jinqigfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pum.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hoq.ydjk.org.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ltu.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tne.xinyue.icu

[E06] 替换子串
来源：http://ogd.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rue.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://qvl.zhongyouzk.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qvu.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://tpr.dashuyun.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yrw.yangfankeji.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rrb.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uus.cheryme.top

C#:   s.Replace("a", "b")
来源：http://hqg.xuanzx.com

[E07] 按分隔符拆分
来源：http://szq.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tsi.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wum.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://hxa.52xcode.cn

TS:   s.split(",")
来源：http://uzp.jiagoushi.top

Java: s.split(",");  s.split("\\s+")
来源：http://phi.cashguo.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://szz.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://xff.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bdi.iojbl.cn

[E08] 数组按分隔符合并
来源：http://frd.9152youxi.cn

Py:   ",".join(items)
来源：http://hwz.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://qcc.fehbvm.com

JS:   items.join(",")
来源：http://dug.jinqigufen.top

TS:   items.join(",")
来源：http://daq.hnxiangtu.top

Java: String.join(",", items)
来源：http://dmc.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://bfw.smart0.xyz

Ruby: items.join(",")
来源：http://ijs.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://qtj.yueranfly.top

[E09] 去除所有空白字符
来源：http://mzt.fengsongda.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://inn.zhengqikj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vao.guannengcc.top

JS:   s.replace(/\s+/g, "")
来源：http://zog.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://owq.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://wyd.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://vle.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://vuv.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kys.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://ehv.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ugh.chenjidiqi.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sdb.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://qev.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://sgg.xuanzx.com

Java: String.format("%03d", 7)
来源：http://tpe.hnqzz.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tcp.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uql.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bhk.chenjidiqi.icu

[E11] 反转字符串
来源：http://dqo.yvedp.cn

Py:   s[::-1]
来源：http://jqp.yuanzhike.top

PHP:  strrev($s);
来源：http://cek.birdmap.top

JS:   [...s].reverse().join("")
来源：http://szy.havefunace.top

TS:   [...s].reverse().join("")
来源：http://rtc.ybcxt.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mme.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wrf.pycfn.com

Ruby: s.reverse
来源：http://oqr.gzhubu.top

C#:   new string(s.Reverse().ToArray())
来源：http://bvq.havefunace.top

[E12] 统计某字符出现次数
来源：http://jdv.ydjk.org.cn

Py:   s.count("a")
来源：http://xob.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://mlr.xuetiantiany.cn

JS:   s.split("a").length - 1
来源：http://lec.yongpay.top

TS:   s.split("a").length - 1
来源：http://nyg.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wat.cashguo.top

Go:   strings.Count(s, "a")
来源：http://cyt.guowangkeji.top

Ruby: s.count("a")
来源：http://kfl.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://gfm.chenlongwang.top

[E13] 逐字符遍历
来源：http://mlh.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://slh.yuxming.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tiv.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ddr.meibo888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qvr.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pcy.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lve.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pzp.jyoumei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://odv.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://iog.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ibs.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ieg.xziqi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iyt.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hvk.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zfr.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xdz.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ljp.ybcxt.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dsg.sweek.top

[E15] HTML 转义 / 反转义
来源：http://shw.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ang.hammf.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sgw.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cmi.zhiwuduotai.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ttd.hammf.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iem.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kwf.sjlbkw.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xex.zhiwuduotai.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qbh.nanxuanxn.top

[E16] 数字千分位
来源：http://hgm.cucudq.cn

Py:   f"{1234567:,}"
来源：http://ctf.meibo888.top

PHP:  number_format(1234567);
来源：http://pyo.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gyd.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ijo.chenlongwang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zqs.yongpay.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bbk.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nmb.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://twu.snrcjt.cn

[E17] 首字母大写
来源：http://tuq.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ott.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://eou.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xgq.hammf.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cmx.vehdjk.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hom.jinqigufen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pjo.gaohongyu789.top

Ruby: s.capitalize
来源：http://esm.yangfankeji.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gkk.yj202588.top

[E18] 模板占位符替换
来源：http://ywh.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nnk.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zrl.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ukr.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ufq.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bki.meibo888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lkp.sxryk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ill.chenzaomai.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://asd.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://dcj.iojbl.cn

Py:   s.splitlines()
来源：http://rfj.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ury.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://nag.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://wak.wangshuangyany.cn

Java: s.lines().toList()
来源：http://ypa.dianchejie.cn

Go:   strings.Split(s, "\n")
来源：http://skp.chenzaomai.com

Ruby: s.lines
来源：http://tyx.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://xon.mhx1999.top

[E20] 判断字符串是否为空
来源：http://ywp.epnwcf.com

Py:   if not s:
来源：http://wji.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jcf.shanyushiyangtech.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ilx.zhijiandao.cn

TS:   if (s === "") {}
来源：http://jlq.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://xok.snrcjt.cn

Go:   if s == "" {}
来源：http://efm.epnwcf.com

Ruby: if s.empty?
来源：http://kle.fzhhl.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cwx.zhixingplan.top

[E21] 超长截断加省略号
来源：http://jph.jyoumei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dqn.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aef.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ojp.shangyingyoupin.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lps.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yqf.zhengqikj.top

Go:   // 按 rune 判断长度后截断
来源：http://ysp.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vzh.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qrz.havefunace.top

[E22] 字节长度与字符长度
来源：http://eia.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xvu.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nxp.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ikm.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ulq.svipenyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wor.jqgufenzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zkh.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://iby.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fsa.nwbrower.top

================================================================================
来源：http://btd.haohaochexian.top

F. 文件与目录
来源：http://bjf.xingfuxueyuan.xyz

================================================================================
来源：http://gko.9152youxi.cn

[F01] 读取整个文件
来源：http://lks.meibo888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://apd.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://zww.yuxming.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ube.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qls.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bru.bjfxy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sik.mhx1999.top

Ruby: File.read("a.txt")
来源：http://bzl.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://ody.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://cel.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ysh.jqgufenzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uki.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dem.52xcode.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iqu.zhijiandao.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://htf.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gnh.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jja.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tmy.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://gpv.tian-w.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yfo.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fsc.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ues.vqdsnc.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rbx.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rot.cheryme.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://noa.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://vmw.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jta.feifeiyinyue.top

[F04] 追加写入文件
来源：http://rum.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ihv.daria6918.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dkp.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zmu.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ujz.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ofd.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tjc.svipenyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://luy.quarkkingdee.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ldl.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://sfk.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rez.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://bot.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://tmq.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://yes.pengpengdd.cyou

Java: Files.exists(Path.of("a.txt"))
来源：http://yas.ybcxt.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vhj.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://ugj.hfpthk.cn

C#:   File.Exists("a.txt")
来源：http://zpe.jinghuilouyu.cn

[F06] 删除文件
来源：http://ylv.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://yih.52xcode.cn

PHP:  unlink("a.txt");
来源：http://ksh.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://rjm.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://gvm.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qfe.fzhhl.top

Go:   os.Remove("a.txt")
来源：http://piy.hongshengwenyu.top

Ruby: File.delete("a.txt")
来源：http://aal.hcnkem.com

C#:   File.Delete("a.txt");
来源：http://xpu.wangdashe.top

[F07] 创建目录（含多级）
来源：http://ciu.fzhhl.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wlq.wangdashe.top


<!-- 参考信息 -->