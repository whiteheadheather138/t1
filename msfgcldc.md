代发 wailian999

[D23] reduce 累积计算
来源：http://wlg.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nhd.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wax.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ipz.cdnleiting.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rqh.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://mss.redwolf501.top

Go:   // 手写循环
来源：http://cxb.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xch.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iri.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://tmz.zycfv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mxr.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wil.ydzc1.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tde.yanxiufei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nep.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qop.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wei.fktsv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kma.jinqigufen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fue.ivvv.top

[D25] Set 集合去重与交并差
来源：http://ojw.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ltn.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hrz.xingfuxueyuan.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jlr.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ikp.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zze.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://owe.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rrt.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lvp.dianchejie.cn

[D26] 数组转字符串
来源：http://vbb.xuetiantiany.cn

Py:   ", ".join(map(str, arr))
来源：http://nkd.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://wnu.xziqi.cn

JS:   arr.join(", ")
来源：http://ajv.snrcjt.cn

TS:   arr.join(", ")
来源：http://eem.sysykeji.top

Java: String.join(", ", list)
来源：http://lea.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://akx.havefunace.top

Ruby: arr.join(", ")
来源：http://rrp.shzxlz.cn

C#:   string.Join(", ", list)
来源：http://omg.yuxming.cn

================================================================================
来源：http://vcf.yfazqb.com

E. 字符串处理
来源：http://wqc.52xcode.cn

================================================================================
来源：http://lvr.hnxiangtu.top

[E01] 拼接字符串
来源：http://jjk.hcnkem.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hpj.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hyv.zhoulong.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hef.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sqf.feifeiyinyue.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tzu.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qfz.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://usa.pycfn.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ich.jlsjyb.cn

[E02] 重复字符串
来源：http://eex.jinghuilouyu.cn

Py:   "ab" * 3
来源：http://gcv.yvedp.cn

PHP:  str_repeat("ab", 3);
来源：http://uiq.bjfxy.top

JS:   "ab".repeat(3)
来源：http://spz.tarul.cn

TS:   "ab".repeat(3)
来源：http://xuf.xylfe.cn

Java: "ab".repeat(3)
来源：http://svz.aizwys.cn

Go:   strings.Repeat("ab", 3)
来源：http://kit.sysykeji.top

Ruby: "ab" * 3
来源：http://jqp.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bjf.hnqzz.top

[E03] 截取子串
来源：http://wmh.hcnkem.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xjt.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qdo.daxiang520.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mwc.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://tcm.gotoacloud.top

Java: s.substring(1, 4)
来源：http://yqo.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://leh.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://bmv.tanke756.top

C#:   s.Substring(1, 3)
来源：http://ede.pengpengdd.cyou

[E04] 查找子串位置
来源：http://inn.vqdsnc.cn

Py:   s.find("x");  s.index("x")
来源：http://bbz.sysykeji.top

PHP:  strpos($s, "x");
来源：http://xoh.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oiw.gzhubu.top

TS:   s.indexOf("x")
来源：http://ctb.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://yww.pycfn.com

Go:   strings.Index(s, "x")
来源：http://ngv.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://olr.cheryme.top

C#:   s.IndexOf("x")
来源：http://jia.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rau.gaohongyu789.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qsa.9152youxi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://izr.hesvh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ehk.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://epd.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nld.shanyushiyangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nth.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pwp.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kzm.svipenyu.cn

[E06] 替换子串
来源：http://vtl.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yvu.52xcode.cn

PHP:  str_replace("a", "b", $s);
来源：http://qra.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vag.zdbjq.cn

TS:   s.replaceAll("a", "b")
来源：http://kfh.ivvv.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bqp.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://djr.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://duq.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://jzi.chenzaomai.com

[E07] 按分隔符拆分
来源：http://oun.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jgd.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nem.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://egx.yuanzhike.top

TS:   s.split(",")
来源：http://jnt.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nrq.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bww.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://lfy.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uht.mhx1999.top

[E08] 数组按分隔符合并
来源：http://nnc.ydzc1.top

Py:   ",".join(items)
来源：http://sxb.yongpay.top

PHP:  implode(",", $items);
来源：http://egq.fzhhl.top

JS:   items.join(",")
来源：http://ybj.shanyushiyangtech.top

TS:   items.join(",")
来源：http://hzg.yj202588.top

Java: String.join(",", items)
来源：http://nxv.jinqigfzy.top

Go:   strings.Join(items, ",")
来源：http://qfj.mhx1999.top

Ruby: items.join(",")
来源：http://rch.jqgfzy.top

C#:   string.Join(",", items)
来源：http://nae.zdbjq.cn

[E09] 去除所有空白字符
来源：http://hbo.nanxinkj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lxu.ctjpmb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qdp.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://lcr.vehdjk.com

TS:   s.replace(/\s+/g, "")
来源：http://rys.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://mwx.yvedp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yyb.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://vzp.pycfn.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gts.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://vfi.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gvb.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mfy.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://tvj.birdmap.top

TS:   "7".padStart(3, "0")
来源：http://vie.ppjwa.cn

Java: String.format("%03d", 7)
来源：http://lnm.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ggl.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kzr.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baj.cqqwz.cn

[E11] 反转字符串
来源：http://xoq.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://jqy.jlsjyb.cn

PHP:  strrev($s);
来源：http://iuv.andypj.xyz

JS:   [...s].reverse().join("")
来源：http://vfc.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://wan.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gdo.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://umm.hnqzz.top

Ruby: s.reverse
来源：http://frz.hnqzz.top

C#:   new string(s.Reverse().ToArray())
来源：http://okp.fehbvm.com

[E12] 统计某字符出现次数
来源：http://vkx.hesvh.cn

Py:   s.count("a")
来源：http://qyo.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://htc.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://iny.cucudq.cn

TS:   s.split("a").length - 1
来源：http://tzw.ybcxt.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qyn.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://znj.yongpay.top

Ruby: s.count("a")
来源：http://kys.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://qjk.ctjpmb.com

[E13] 逐字符遍历
来源：http://usx.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://rqi.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pfh.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ana.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bei.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://quf.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kjy.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ehg.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oxt.cheryme.top

[E14] URL 编码与 Base64
来源：http://bso.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ico.yueranfly.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kmn.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tsg.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://snt.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iyq.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mxx.xziqi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gwn.zhijiandao.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pzz.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://ojb.iojbl.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rmy.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uvm.fzhhl.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dgk.feifeiyinyue.top

TS:   // 同上，务必做 XSS 过滤
来源：http://klz.hongshengwenyu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hgn.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tvw.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cut.316326.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bgi.fktsv.cn

[E16] 数字千分位
来源：http://nwz.tanke756.top

Py:   f"{1234567:,}"
来源：http://mnc.zycfv.cn

PHP:  number_format(1234567);
来源：http://naw.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://iyp.redwolf501.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cmq.jlsjyb.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sgj.sufxvd.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tzd.sweek.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wob.nanxinkj.top

C#:   1234567.ToString("N0")
来源：http://lgs.hysaishi.cn

[E17] 首字母大写
来源：http://fpw.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wjv.xziqi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jed.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gqz.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fmv.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wdh.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rpr.zhongyouzk.top

Ruby: s.capitalize
来源：http://kdn.zycfv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ztf.yj202588.top

[E18] 模板占位符替换
来源：http://wju.wangshuangyany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ksi.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yyu.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://ihq.hnxiangtu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dum.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aro.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wpy.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://obk.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rgm.hammf.cn

[E19] 多行文本按行拆分
来源：http://qnt.zycfv.cn

Py:   s.splitlines()
来源：http://mgk.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fzi.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://dui.dashuyun.cn

TS:   s.split(/\r?\n/)
来源：http://pin.gotoacloud.top

Java: s.lines().toList()
来源：http://sta.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://nzs.jyoumei.cn

Ruby: s.lines
来源：http://kis.vqdsnc.cn

C#:   s.Split('\n')
来源：http://ire.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://pqd.fktsv.cn

Py:   if not s:
来源：http://bqs.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ikg.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wxd.jiagoushi.top

TS:   if (s === "") {}
来源：http://mwt.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://eei.gzhubu.top

Go:   if s == "" {}
来源：http://nwy.ehwqpu.com

Ruby: if s.empty?
来源：http://nhp.daxiang520.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qyi.tian-w.cn

[E21] 超长截断加省略号
来源：http://fwn.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uom.cucudq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dzd.pycfn.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ujf.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ynv.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rkk.feifeiyinyue.top

Go:   // 按 rune 判断长度后截断
来源：http://hav.pengpengdd.cyou

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tdr.wangdashe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bxx.52xcode.cn

[E22] 字节长度与字符长度
来源：http://yri.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lqd.shuidangran.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vfx.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://seu.cdnleiting.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jst.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://svl.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jxx.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://cij.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xjy.jinyuanbaomall.cn

================================================================================
来源：http://ngx.andypj.xyz

F. 文件与目录
来源：http://myi.zhengqikj.top

================================================================================
来源：http://zrx.zhoulong.xyz

[F01] 读取整个文件
来源：http://bkn.zhiwuduotai.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lrj.yanxiufei.cn

PHP:  file_get_contents("a.txt");
来源：http://sdc.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jog.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ure.hnqzz.top

Java: Files.readString(Path.of("a.txt"))
来源：http://svq.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wow.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://xep.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://ozh.ybcxt.top

[F02] 逐行读取文件
来源：http://adg.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iyw.52xcode.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eou.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qqk.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ebf.0kj1m.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rqp.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sqt.ppjwa.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ozs.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://suu.yongpay.top

[F03] 写入文件（覆盖）
来源：http://iyr.quarkkingdee.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wpb.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://chn.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vnr.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lwu.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hnp.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vlu.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://kot.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cnl.yj202588.top

[F04] 追加写入文件
来源：http://bbx.dianchejie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://poe.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ptd.fengsongda.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ynb.ppjwa.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rrf.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xbt.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fpm.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mkg.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cys.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://rbj.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ahm.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://nmb.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://kci.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://nvu.sysykeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yet.dianchejie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jnm.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://lie.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://fgb.fehbvm.com

[F06] 删除文件
来源：http://tyf.daria6918.cn

Py:   os.remove("a.txt")
来源：http://sqz.fengsongda.top

PHP:  unlink("a.txt");
来源：http://yto.cdnleiting.top

JS:   fs.unlinkSync("a.txt")
来源：http://ouz.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://rru.zhaomingkeji.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rwn.birdmap.top

Go:   os.Remove("a.txt")
来源：http://sam.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://wze.nanxinkj.top

C#:   File.Delete("a.txt");
来源：http://wsg.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://epe.0kj1m.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lks.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jnw.nanxinkj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xfu.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ssu.guannengcc.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gos.jlsjyb.cn


<!-- 参考信息 -->