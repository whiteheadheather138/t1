代发 wailian999

[D23] reduce 累积计算
来源：http://obw.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aek.aibaodan.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tus.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://axw.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hcu.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ywi.yanxiufei.cn

Go:   // 手写循环
来源：http://ecc.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ijz.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ctp.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://hfn.0kj1m.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fbx.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bxj.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xhd.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://grl.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tfy.aizwys.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wxe.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wem.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kbq.haohaochexian.top

[D25] Set 集合去重与交并差
来源：http://tuy.0kj1m.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sbq.jlsjyb.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rha.tianlin.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fti.meibo888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qkc.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yqe.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jvq.meibo888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://usz.gzhubu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uya.dashuyun.cn

[D26] 数组转字符串
来源：http://bxu.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://wts.yj20258.top

PHP:  implode(", ", $arr);
来源：http://mec.hnxiangtu.top

JS:   arr.join(", ")
来源：http://kuz.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://uyg.cashguo.top

Java: String.join(", ", list)
来源：http://mvv.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://ifz.yangfankeji.com

Ruby: arr.join(", ")
来源：http://qli.fengsongda.top

C#:   string.Join(", ", list)
来源：http://qkp.jyoumei.cn

================================================================================
来源：http://tng.vqdsnc.cn

E. 字符串处理
来源：http://bfg.zhiwuduotai.top

================================================================================
来源：http://zlk.yanxiufei.cn

[E01] 拼接字符串
来源：http://rhy.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eeg.zhiwuduotai.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vhn.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ufh.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dxz.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tsh.9152youxi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yjh.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vwm.vqdsnc.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ntc.kuanghao11.cn

[E02] 重复字符串
来源：http://utq.yonumen.top

Py:   "ab" * 3
来源：http://bld.jinqigfzy.top

PHP:  str_repeat("ab", 3);
来源：http://uju.shanyushiyangtech.top

JS:   "ab".repeat(3)
来源：http://mcn.bjfxy.top

TS:   "ab".repeat(3)
来源：http://lej.ctjpmb.com

Java: "ab".repeat(3)
来源：http://lzi.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://nag.epnwcf.com

Ruby: "ab" * 3
来源：http://nud.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vzs.52xcode.cn

[E03] 截取子串
来源：http://nos.svipenyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qra.hywenlv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wtq.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pyw.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://jho.jinyuanbaomall.cn

Java: s.substring(1, 4)
来源：http://brd.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yem.jinghuilouyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xtd.yanxiufei.cn

C#:   s.Substring(1, 3)
来源：http://jgc.yj20258.top

[E04] 查找子串位置
来源：http://nxt.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://wlj.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://dbp.yuanzhike.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bxh.jiagoushi.top

TS:   s.indexOf("x")
来源：http://owr.bjfxy.top

Java: s.indexOf("x")
来源：http://qha.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://dqi.tanke756.top

Ruby: s.index("x")
来源：http://tfg.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://bvx.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gos.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://goh.uphjek.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://byi.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mqy.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://urn.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lqe.xziqi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yxn.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rfc.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ajj.shanyushiyangtech.top

[E06] 替换子串
来源：http://zvc.daria6918.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zml.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://dfr.xinyue.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xje.cucudq.cn

TS:   s.replaceAll("a", "b")
来源：http://yge.yuxming.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vcg.epnwcf.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fcl.iojbl.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qvx.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://xsf.jqgufenzy.top

[E07] 按分隔符拆分
来源：http://cga.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vip.9152youxi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zfh.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qlc.hcnkem.com

TS:   s.split(",")
来源：http://hdr.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mqj.yanxiufei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kfk.xuetiantiany.cn

Ruby: s.split(",");  s.split
来源：http://ynz.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://itn.fktsv.cn

[E08] 数组按分隔符合并
来源：http://chx.hfpthk.cn

Py:   ",".join(items)
来源：http://rld.havefunace.top

PHP:  implode(",", $items);
来源：http://sgh.jinqigfzy.top

JS:   items.join(",")
来源：http://oin.xylfe.cn

TS:   items.join(",")
来源：http://rdx.hnqzz.top

Java: String.join(",", items)
来源：http://tzp.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://omv.jinqigfzy.top

Ruby: items.join(",")
来源：http://lxb.yj20258888.top

C#:   string.Join(",", items)
来源：http://avf.52xcode.cn

[E09] 去除所有空白字符
来源：http://thq.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lpc.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rol.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://tkd.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://xfq.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://kix.kuanghao11.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rwd.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vxv.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cvi.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://rfe.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fgy.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mql.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://bgq.jinqigfzy.top

TS:   "7".padStart(3, "0")
来源：http://xvm.gzhubu.top

Java: String.format("%03d", 7)
来源：http://wpp.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bqy.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://buw.ivvv.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://puu.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://uhq.tianlin.xyz

Py:   s[::-1]
来源：http://wpu.shzxlz.cn

PHP:  strrev($s);
来源：http://kgv.yvedp.cn

JS:   [...s].reverse().join("")
来源：http://nqz.sweek.top

TS:   [...s].reverse().join("")
来源：http://kll.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nwb.c1oappe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kor.zhiwuduotai.top

Ruby: s.reverse
来源：http://ihw.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://vyc.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://owi.zdqjudy.top

Py:   s.count("a")
来源：http://uaf.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://aix.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://vfy.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://osa.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ehh.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://kam.fehbvm.com

Ruby: s.count("a")
来源：http://oqi.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://neg.ctjpmb.com

[E13] 逐字符遍历
来源：http://eqp.hongshengwenyu.top

Py:   for ch in s: print(ch)
来源：http://hov.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ywz.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pvv.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://eab.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jzm.shanyushiyangtech.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qnz.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://mhw.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gld.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://rbv.smart0.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dqa.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lib.ybcxt.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hbt.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tlo.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://omc.ivvv.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dme.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wme.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dkr.sweek.top

[E15] HTML 转义 / 反转义
来源：http://eap.cucudq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ofz.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fkj.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wnw.nanxuanxn.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qqs.ivvv.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dau.zdbjq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xyh.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://krq.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://llk.yj202588.top

[E16] 数字千分位
来源：http://wwv.smart0.xyz

Py:   f"{1234567:,}"
来源：http://mfi.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://use.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://sgk.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://tzq.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bsx.pengpengdd.cyou

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ujq.epnwcf.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rwj.yvedp.cn

C#:   1234567.ToString("N0")
来源：http://xmi.zhoulong.xyz

[E17] 首字母大写
来源：http://kje.jyoumei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qke.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jed.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ooo.0kj1m.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xnw.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sqk.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ffi.tarul.cn

Ruby: s.capitalize
来源：http://ymp.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xcx.chenzaomai.com

[E18] 模板占位符替换
来源：http://utg.cashguo.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nel.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gjb.guowangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jus.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pfx.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pmr.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tsc.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oor.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mph.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://rqo.nanxuanxn.top

Py:   s.splitlines()
来源：http://gad.kuanghao11.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ply.smart0.xyz

JS:   s.split(/\r?\n/)
来源：http://yrj.mhx1999.top

TS:   s.split(/\r?\n/)
来源：http://fin.hnqzz.top

Java: s.lines().toList()
来源：http://tlb.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://qui.nanxuanxn.top

Ruby: s.lines
来源：http://alk.hysaishi.cn

C#:   s.Split('\n')
来源：http://bgr.zhongyouzk.top

[E20] 判断字符串是否为空
来源：http://rvv.sxryk.cn

Py:   if not s:
来源：http://yra.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jii.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jgi.hfpthk.cn

TS:   if (s === "") {}
来源：http://spm.hnxiangtu.top

Java: if (s.isEmpty()) {}
来源：http://rbu.redwolf501.top

Go:   if s == "" {}
来源：http://lld.fzhhl.top

Ruby: if s.empty?
来源：http://wuv.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xnm.dianchejie.cn

[E21] 超长截断加省略号
来源：http://qlq.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://szr.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://myf.zhongyouzk.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iuy.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hpo.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xcv.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://fli.havefunace.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eiu.shanyushiyangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://exp.aizwys.cn

[E22] 字节长度与字符长度
来源：http://xec.sjlbkw.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pcp.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cza.nanxinkj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yep.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mik.hfpthk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://slm.mhx1999.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wor.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://jje.pengpengdd.cyou

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zql.aibaodan.cn

================================================================================
来源：http://aet.yangfankeji.com

F. 文件与目录
来源：http://uye.bbcook.cn

================================================================================
来源：http://lic.yonumen.top

[F01] 读取整个文件
来源：http://qki.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://edj.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://gfn.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bon.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vms.wangshuangyany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jvj.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://slk.ivvv.top

Ruby: File.read("a.txt")
来源：http://exx.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://qkj.shuidangran.top

[F02] 逐行读取文件
来源：http://xup.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ufa.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wlf.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tza.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ams.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dvb.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xzf.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zok.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lux.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://swn.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ixj.fehbvm.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://bzv.xziqi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ofp.gotoacloud.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lkb.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zku.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kqe.ydjk.org.cn

Ruby: File.write("a.txt", "hi")
来源：http://ywa.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wgx.zhijiandao.cn

[F04] 追加写入文件
来源：http://hrz.cqqwz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xee.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rkj.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ipp.yuanzhike.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bjl.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qdi.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ybp.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tut.yvedp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aiq.fengsongda.top

[F05] 判断文件或目录是否存在
来源：http://awq.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vwf.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://fpy.yfazqb.com

JS:   fs.existsSync("a.txt")
来源：http://vcg.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://ftr.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ynm.xylfe.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bze.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://yrv.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://mty.ydjk.org.cn

[F06] 删除文件
来源：http://ydq.nwbrower.top

Py:   os.remove("a.txt")
来源：http://pbg.shuidangran.top

PHP:  unlink("a.txt");
来源：http://tbv.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eug.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://pyk.cheryme.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://arv.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://mtd.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://nyh.tian-w.cn

C#:   File.Delete("a.txt");
来源：http://qjo.redwolf501.top

[F07] 创建目录（含多级）
来源：http://pyo.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xit.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ixe.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ctd.xuanzx.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rar.shuidangran.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://byk.jianghu66.top


<!-- 参考信息 -->