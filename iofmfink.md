代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://njc.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://uaf.jinqigfzy.top

C#:   list.Contains(x)
来源：http://hqg.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://sjf.chenlongwang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dkh.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dkz.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zih.yj20258.top

TS:   [...arr];
来源：http://lix.havefunace.top

Java: new ArrayList<>(list);
来源：http://ujk.epnwcf.com

Go:   copied := append([]int(nil), arr...)
来源：http://gjm.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://nbk.vehdjk.com

C#:   new List<int>(list);
来源：http://srj.xingfuxueyuan.xyz

[D23] reduce 累积计算
来源：http://bhd.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kro.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://isv.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tii.hesvh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rts.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lrd.ivvv.top

Go:   // 手写循环
来源：http://xgb.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jae.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aej.smart0.xyz

[D24] 字典 / Map 基本操作
来源：http://zny.jqgufenzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kkw.hysaishi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xab.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fad.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nqk.cqqwz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://apx.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tsx.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rav.cheryme.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xvo.zhengqikj.top

[D25] Set 集合去重与交并差
来源：http://qqu.havefunace.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://puc.fanxiaobao.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uxw.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://etj.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lmw.hfpthk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://diz.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xnq.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sxq.zhengqikj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hla.jinqigufen.top

[D26] 数组转字符串
来源：http://yxp.sufxvd.cn

Py:   ", ".join(map(str, arr))
来源：http://aqu.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://fay.havefunace.top

JS:   arr.join(", ")
来源：http://tfo.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://ews.hfpthk.cn

Java: String.join(", ", list)
来源：http://yhk.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://fgx.havefunace.top

Ruby: arr.join(", ")
来源：http://dqa.yj20258.top

C#:   string.Join(", ", list)
来源：http://dek.hfpthk.cn

================================================================================
来源：http://dpb.aibaodan.cn

E. 字符串处理
来源：http://lmi.gaohongyu789.top

================================================================================
来源：http://cah.vqdsnc.cn

[E01] 拼接字符串
来源：http://sbt.guowangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://odp.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dsb.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ikl.gaohongyu789.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zbj.jinghuilouyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uik.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gly.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ovm.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jge.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://txt.nwbrower.top

Py:   "ab" * 3
来源：http://jib.hongshengwenyu.top

PHP:  str_repeat("ab", 3);
来源：http://ati.iojbl.cn

JS:   "ab".repeat(3)
来源：http://ilp.uphjek.com

TS:   "ab".repeat(3)
来源：http://hrb.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://aea.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://cuy.zycfv.cn

Ruby: "ab" * 3
来源：http://xmu.vehdjk.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gee.zycfv.cn

[E03] 截取子串
来源：http://sjd.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iim.dianchejie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jxk.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ssi.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://azr.zhengqikj.top

Java: s.substring(1, 4)
来源：http://yhg.yuanzhike.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zer.yuanzhike.top

Ruby: s[1, 3];  s[1..3]
来源：http://ieu.yj202588.top

C#:   s.Substring(1, 3)
来源：http://mcx.tanke756.top

[E04] 查找子串位置
来源：http://ojx.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://thq.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://jqy.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gsr.xuetiantiany.cn

TS:   s.indexOf("x")
来源：http://oxb.cqqwz.cn

Java: s.indexOf("x")
来源：http://mhi.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://ebb.haohaochexian.top

Ruby: s.index("x")
来源：http://xiq.jyoumei.cn

C#:   s.IndexOf("x")
来源：http://mdn.jinghuilouyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dzq.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zcf.nwbrower.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dvs.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xzj.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://loa.jianghu66.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sio.wangdashe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oxf.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yyl.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rmg.tianlin.xyz

[E06] 替换子串
来源：http://igh.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://okc.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://qam.chenzaomai.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yng.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://ecu.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ges.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tzt.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zvt.xuanzx.com

C#:   s.Replace("a", "b")
来源：http://cql.hnqzz.top

[E07] 按分隔符拆分
来源：http://msj.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gmx.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ilg.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wwk.yonumen.top

TS:   s.split(",")
来源：http://xqw.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uzj.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zku.yj202588.top

Ruby: s.split(",");  s.split
来源：http://yck.cdnleiting.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kws.hysaishi.cn

[E08] 数组按分隔符合并
来源：http://hwr.havefunace.top

Py:   ",".join(items)
来源：http://vra.hysaishi.cn

PHP:  implode(",", $items);
来源：http://hpl.wangshuangyany.cn

JS:   items.join(",")
来源：http://iwm.zhaomingkeji.xyz

TS:   items.join(",")
来源：http://awk.haohaochexian.top

Java: String.join(",", items)
来源：http://dfc.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://lwi.feifeiyinyue.top

Ruby: items.join(",")
来源：http://vus.0kj1m.cn

C#:   string.Join(",", items)
来源：http://yse.zhixingplan.top

[E09] 去除所有空白字符
来源：http://kvc.yvedp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xtc.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uvq.cheryme.top

JS:   s.replace(/\s+/g, "")
来源：http://uxj.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://ece.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://axw.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dio.daria6918.cn

Ruby: s.gsub(/\s+/, "")
来源：http://epz.shzxlz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pgv.shangyingyoupin.top

[E10] 左侧补零 / 定长填充
来源：http://uyt.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ibz.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lbf.smart0.xyz

JS:   "7".padStart(3, "0")
来源：http://rxc.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://vap.daxiang520.top

Java: String.format("%03d", 7)
来源：http://ejn.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://ebt.fanxiaobao.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://foi.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sic.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://nms.yj20258.top

Py:   s[::-1]
来源：http://oar.yj202588.top

PHP:  strrev($s);
来源：http://pua.ehwqpu.com

JS:   [...s].reverse().join("")
来源：http://lvp.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://rof.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cbr.snrcjt.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eaf.zycfv.cn

Ruby: s.reverse
来源：http://bvs.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yqg.jinqigfzy.top

[E12] 统计某字符出现次数
来源：http://cxq.nanxuanxn.top

Py:   s.count("a")
来源：http://fwx.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://peb.yj20258.top

JS:   s.split("a").length - 1
来源：http://wdr.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://onq.hnxiangtu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://put.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://ikr.xylfe.cn

Ruby: s.count("a")
来源：http://xjb.zhongyouzk.top

C#:   s.Count(c => c == 'a')
来源：http://xuz.xuetiantiany.cn

[E13] 逐字符遍历
来源：http://ebr.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://nfn.ybcxt.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://utf.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ttm.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jal.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ylg.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kcv.zdbjq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wjd.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yor.cheryme.top

[E14] URL 编码与 Base64
来源：http://wet.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qvo.yvedp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jav.tanke756.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uja.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qie.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ywy.hammf.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uum.gzhubu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nku.dianchejie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gjh.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://xys.zdqjudy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kki.hesvh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ith.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://leh.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://brq.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ser.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rja.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xop.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cvd.zycfv.cn

[E16] 数字千分位
来源：http://gho.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://jzp.xziqi.cn

PHP:  number_format(1234567);
来源：http://hcp.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qxb.redwolf501.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kbq.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ndf.aibaodan.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zwk.redwolf501.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zry.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://xbc.smart0.xyz

[E17] 首字母大写
来源：http://pxp.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hdy.zhoulong.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://mzs.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fyj.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://olp.9152youxi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://luz.pengpengdd.cyou

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gaj.daria6918.cn

Ruby: s.capitalize
来源：http://rey.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bbw.9152youxi.cn

[E18] 模板占位符替换
来源：http://xaw.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zst.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mep.sweek.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kcp.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://add.shangyingyoupin.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qbd.sxryk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uil.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rto.meibo888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ovc.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://isu.yj20258.top

Py:   s.splitlines()
来源：http://gmx.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wvf.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://jjk.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://kub.epnwcf.com

Java: s.lines().toList()
来源：http://cua.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://dyc.zhongyouzk.top

Ruby: s.lines
来源：http://tyh.cdnleiting.top

C#:   s.Split('\n')
来源：http://lne.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://bqh.wangshuangyany.cn

Py:   if not s:
来源：http://ohe.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ehu.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://crf.xylfe.cn

TS:   if (s === "") {}
来源：http://ihp.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://lcz.sxryk.cn

Go:   if s == "" {}
来源：http://jhs.daria6918.cn

Ruby: if s.empty?
来源：http://dtz.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xnr.zhengqikj.top

[E21] 超长截断加省略号
来源：http://hht.zhengqikj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zan.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xsw.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uej.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sys.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cit.ydzc1.top

Go:   // 按 rune 判断长度后截断
来源：http://mpj.52xcode.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yjy.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://byr.redwolf501.top

[E22] 字节长度与字符长度
来源：http://tqn.zycfv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://les.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yfq.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pas.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sko.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dfn.jqgufenzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zpv.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://zse.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qly.cucudq.cn

================================================================================
来源：http://fwn.yuxming.cn

F. 文件与目录
来源：http://ynw.9152youxi.cn

================================================================================
来源：http://trr.yj20258.top

[F01] 读取整个文件
来源：http://aio.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bgv.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://yqk.ehwqpu.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xjd.aizwys.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nsm.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wlq.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jpg.sysykeji.top

Ruby: File.read("a.txt")
来源：http://jsv.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://yfo.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://qct.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jpl.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oiu.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pav.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lwc.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tpr.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kgs.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lqt.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vee.tian-w.cn

[F03] 写入文件（覆盖）
来源：http://orj.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bmv.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ngf.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://beb.xingfuxueyuan.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://txk.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mhv.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ydy.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://pgl.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aou.yj20258.top

[F04] 追加写入文件
来源：http://soq.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pyc.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gco.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ilx.birdmap.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qcz.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tyb.hcnkem.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fxd.shuidangran.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ktp.zdbjq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nah.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://uuf.sysykeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ade.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://mkj.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://drl.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://cwm.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jjj.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ddd.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://cpy.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://mfe.yueranfly.top

[F06] 删除文件
来源：http://thm.cashguo.top

Py:   os.remove("a.txt")
来源：http://rjw.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://tsx.birdmap.top


<!-- 参考信息 -->