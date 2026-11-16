代发 wailian999

[D23] reduce 累积计算
来源：http://msz.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gih.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tjk.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gxi.tianlin.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://znk.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xuo.sysykeji.top

Go:   // 手写循环
来源：http://uod.jqgfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gdo.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nde.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://vma.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wxm.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://heo.jianghu66.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vjc.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://opr.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bhk.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mfp.smart0.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mtn.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xmx.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://xkk.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vjs.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aky.cdnleiting.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iwn.meibo888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ers.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tvv.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://crw.316326.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gxe.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ocm.cdnleiting.top

[D26] 数组转字符串
来源：http://qxm.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://uug.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://ifk.hnqzz.top

JS:   arr.join(", ")
来源：http://nbo.jyoumei.cn

TS:   arr.join(", ")
来源：http://tys.fehbvm.com

Java: String.join(", ", list)
来源：http://gln.ehwqpu.com

Go:   strings.Join(strs, ", ")
来源：http://dnd.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://dmg.zhijiandao.cn

C#:   string.Join(", ", list)
来源：http://ezl.zhiwuduotai.top

================================================================================
来源：http://ita.vehdjk.com

E. 字符串处理
来源：http://gol.gotoacloud.top

================================================================================
来源：http://uht.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://bgm.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bln.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qck.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://edp.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://giq.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eyc.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dtu.hongshengwenyu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nnb.sxryk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mpy.c1oappe.top

[E02] 重复字符串
来源：http://vfr.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://asc.hesvh.cn

PHP:  str_repeat("ab", 3);
来源：http://plm.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://ptq.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://hje.zdbjq.cn

Java: "ab".repeat(3)
来源：http://cmj.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://sdv.xylfe.cn

Ruby: "ab" * 3
来源：http://ekx.ehwqpu.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lfj.chenlongwang.top

[E03] 截取子串
来源：http://tre.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lhd.ydzc1.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fyb.shuidangran.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lqn.mhx1999.top

TS:   s.slice(1, 4)
来源：http://jfp.gogol.net.cn

Java: s.substring(1, 4)
来源：http://tcj.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gnl.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://may.ehwqpu.com

C#:   s.Substring(1, 3)
来源：http://cvs.dianchejie.cn

[E04] 查找子串位置
来源：http://kix.bbcook.cn

Py:   s.find("x");  s.index("x")
来源：http://nqn.wangshuangyany.cn

PHP:  strpos($s, "x");
来源：http://krf.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://omj.52xcode.cn

TS:   s.indexOf("x")
来源：http://jcq.chenlongwang.top

Java: s.indexOf("x")
来源：http://nbb.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://hhk.fzhhl.top

Ruby: s.index("x")
来源：http://fpe.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://pvw.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tet.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://meb.jqgufenzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cof.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aqu.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xqp.iojbl.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hmg.shzxlz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ocs.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://got.epnwcf.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bmj.shanyushiyangtech.top

[E06] 替换子串
来源：http://ljr.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pmm.yangfankeji.com

PHP:  str_replace("a", "b", $s);
来源：http://gkn.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ufl.chenjidiqi.icu

TS:   s.replaceAll("a", "b")
来源：http://zvd.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rdl.hongshengwenyu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://swl.yfazqb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yuz.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://hev.hcnkem.com

[E07] 按分隔符拆分
来源：http://wbi.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ede.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nxn.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://kkd.mhx1999.top

TS:   s.split(",")
来源：http://pwf.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://aka.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ame.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://pcl.iojbl.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rmx.xinyue.icu

[E08] 数组按分隔符合并
来源：http://euc.yangfankeji.com

Py:   ",".join(items)
来源：http://tti.yongpay.top

PHP:  implode(",", $items);
来源：http://rqn.jqgfzy.top

JS:   items.join(",")
来源：http://icl.jqgfzy.top

TS:   items.join(",")
来源：http://fhg.sweek.top

Java: String.join(",", items)
来源：http://mij.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://ovj.sysykeji.top

Ruby: items.join(",")
来源：http://ruu.chenzaomai.com

C#:   string.Join(",", items)
来源：http://ban.aibaodan.cn

[E09] 去除所有空白字符
来源：http://juv.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vcf.fanxiaobao.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gzn.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://kev.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://zsx.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://azc.shanyushiyangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://aex.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://ris.zhixingplan.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gng.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://hoc.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ibm.fengsongda.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qke.0kj1m.cn

JS:   "7".padStart(3, "0")
来源：http://jsh.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://rxb.nanxuanxn.top

Java: String.format("%03d", 7)
来源：http://hfb.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ild.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://idn.c1oappe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nhd.quarkkingdee.top

[E11] 反转字符串
来源：http://ttu.hesvh.cn

Py:   s[::-1]
来源：http://kga.ydzc1.top

PHP:  strrev($s);
来源：http://sgx.shangyingyoupin.top

JS:   [...s].reverse().join("")
来源：http://jwu.ybcxt.top

TS:   [...s].reverse().join("")
来源：http://mqx.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://enj.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hiy.fktsv.cn

Ruby: s.reverse
来源：http://iuq.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://bgq.sysykeji.top

[E12] 统计某字符出现次数
来源：http://yhv.hesvh.cn

Py:   s.count("a")
来源：http://pma.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://nvl.mhx1999.top

JS:   s.split("a").length - 1
来源：http://gnj.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://wje.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dvs.pycfn.com

Go:   strings.Count(s, "a")
来源：http://lua.feifeiyinyue.top

Ruby: s.count("a")
来源：http://plk.zhixingplan.top

C#:   s.Count(c => c == 'a')
来源：http://mmk.fengsongda.top

[E13] 逐字符遍历
来源：http://uzy.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://qxa.zhaomingkeji.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dmo.yuxming.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ivm.ehwqpu.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://gqr.xylfe.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kji.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sey.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://eta.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jnq.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://rjn.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yhv.yfazqb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://mmm.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://acy.xuetiantiany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hge.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gla.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://whu.fzhhl.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hwg.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ukf.feifeiyinyue.top

[E15] HTML 转义 / 反转义
来源：http://zet.gaohongyu789.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xya.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lca.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ufc.yongpay.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wkg.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bpo.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jvy.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jkg.yongpay.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bur.zhixingplan.top

[E16] 数字千分位
来源：http://ehr.chenzaomai.com

Py:   f"{1234567:,}"
来源：http://nqz.snrcjt.cn

PHP:  number_format(1234567);
来源：http://hjo.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yme.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gvn.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pra.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wdp.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xwv.shangyingyoupin.top

C#:   1234567.ToString("N0")
来源：http://gxf.shangyingyoupin.top

[E17] 首字母大写
来源：http://unq.andypj.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://amw.havefunace.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ttj.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xcs.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://isq.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cxu.sweek.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://som.iojbl.cn

Ruby: s.capitalize
来源：http://lam.wangshuangyany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fgs.zhoulong.xyz

[E18] 模板占位符替换
来源：http://erx.xuetiantiany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mmf.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hdl.aizwys.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ihd.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tys.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yqx.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jub.yj202588.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ujz.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dke.sxryk.cn

[E19] 多行文本按行拆分
来源：http://loa.hammf.cn

Py:   s.splitlines()
来源：http://jay.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cvx.shuidangran.top

JS:   s.split(/\r?\n/)
来源：http://jid.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://vxq.redwolf501.top

Java: s.lines().toList()
来源：http://uht.pycfn.com

Go:   strings.Split(s, "\n")
来源：http://svz.quarkkingdee.top

Ruby: s.lines
来源：http://aha.kuanghao11.cn

C#:   s.Split('\n')
来源：http://idx.zdqjudy.top

[E20] 判断字符串是否为空
来源：http://eov.fzhhl.top

Py:   if not s:
来源：http://gdc.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zzq.yanxiufei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sxk.pengpengdd.cyou

TS:   if (s === "") {}
来源：http://axl.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://ccu.hnxiangtu.top

Go:   if s == "" {}
来源：http://bwz.snrcjt.cn

Ruby: if s.empty?
来源：http://kuh.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://maj.xinyue.icu

[E21] 超长截断加省略号
来源：http://lbb.xinyue.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gko.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jlk.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wcv.ybcxt.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uob.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hpn.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://bkm.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tee.svipenyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wwq.smart0.xyz

[E22] 字节长度与字符长度
来源：http://qbc.aizwys.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dcm.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dgd.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qyh.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fcp.shzxlz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dnw.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xsg.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://aqk.tian-w.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://azc.sysykeji.top

================================================================================
来源：http://vqt.ivvv.top

F. 文件与目录
来源：http://tny.yonumen.top

================================================================================
来源：http://buj.tian-w.cn

[F01] 读取整个文件
来源：http://igt.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ive.quarkkingdee.top

PHP:  file_get_contents("a.txt");
来源：http://ush.bbcook.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dda.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://syj.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://bkz.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zug.xingfuxueyuan.xyz

Ruby: File.read("a.txt")
来源：http://ivn.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://gyh.gotoacloud.top

[F02] 逐行读取文件
来源：http://vei.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dka.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://khc.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gkf.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cpz.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kip.jinyuanbaomall.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dqg.ctjpmb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vgs.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zjb.havefunace.top

[F03] 写入文件（覆盖）
来源：http://wkz.yfazqb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aix.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gzy.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gte.chenjidiqi.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eje.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xej.daria6918.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ldc.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://psj.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://phj.zhixingplan.top

[F04] 追加写入文件
来源：http://icg.sxryk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qgx.ydjk.org.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ohm.0kj1m.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mib.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cfk.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ftw.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://brt.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dyy.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://saf.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://uic.haohaochexian.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fol.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://eec.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://byr.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://spp.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kes.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mih.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://chp.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://xwa.yuanzhike.top

[F06] 删除文件
来源：http://uja.hammf.cn

Py:   os.remove("a.txt")
来源：http://hox.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://wjq.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zmr.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://gja.ivvv.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wkb.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://fpn.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://urv.shanyushiyangkeji.top

C#:   File.Delete("a.txt");
来源：http://xjj.yj20258.top

[F07] 创建目录（含多级）
来源：http://oaq.fanxiaobao.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uvb.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qmd.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ujy.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qlk.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dgu.shanyushiyangkeji.top


<!-- 参考信息 -->