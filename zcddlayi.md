代发 wailian999

Java: new ArrayList<>(list);
来源：http://xka.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mpq.andypj.xyz

Ruby: arr.dup;  arr.clone
来源：http://mcu.316326.xyz

C#:   new List<int>(list);
来源：http://rcc.jinghuilouyu.cn

[D23] reduce 累积计算
来源：http://mjd.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mka.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gto.vehdjk.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xom.cqqwz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jzi.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jzw.tian-w.cn

Go:   // 手写循环
来源：http://jyw.dashuyun.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rwd.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ftq.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://mix.9152youxi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uff.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dvu.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cla.dianchejie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nut.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fjq.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wkl.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kef.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mwh.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://sjq.feifeiyinyue.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aaz.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ebz.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wag.quarkkingdee.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rca.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sgf.zhoulong.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sss.vehdjk.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ahx.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dsr.jiagoushi.top

[D26] 数组转字符串
来源：http://dgx.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://hxu.guannengcc.top

PHP:  implode(", ", $arr);
来源：http://ozf.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://rrk.hfpthk.cn

TS:   arr.join(", ")
来源：http://qbj.svipenyu.cn

Java: String.join(", ", list)
来源：http://rzf.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://ryt.9152youxi.cn

Ruby: arr.join(", ")
来源：http://cvp.chenjidiqi.icu

C#:   string.Join(", ", list)
来源：http://lnz.jqgfzy.top

================================================================================
来源：http://qlg.zdbjq.cn

E. 字符串处理
来源：http://zmv.kuanghao11.cn

================================================================================
来源：http://gmc.cashguo.top

[E01] 拼接字符串
来源：http://elv.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gbs.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cjm.tian-w.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qeo.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://otg.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oua.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fkv.svipenyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ipj.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qdh.redwolf501.top

[E02] 重复字符串
来源：http://bep.gotoacloud.top

Py:   "ab" * 3
来源：http://kje.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://fyc.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://sar.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://hue.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://ekx.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://dgq.hcnkem.com

Ruby: "ab" * 3
来源：http://riy.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zot.guowangkeji.top

[E03] 截取子串
来源：http://byu.jinqigufen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hqn.cqqwz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hzt.yonumen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jbc.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://cqv.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://quw.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ooc.yangfankeji.com

Ruby: s[1, 3];  s[1..3]
来源：http://mlg.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://ttt.ydjk.org.cn

[E04] 查找子串位置
来源：http://pmi.bbcook.cn

Py:   s.find("x");  s.index("x")
来源：http://gyd.xziqi.cn

PHP:  strpos($s, "x");
来源：http://ebf.daria6918.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fed.hfpthk.cn

TS:   s.indexOf("x")
来源：http://dqf.zhoulong.xyz

Java: s.indexOf("x")
来源：http://bxa.gogol.net.cn

Go:   strings.Index(s, "x")
来源：http://azg.bjfxy.top

Ruby: s.index("x")
来源：http://xlr.cheryme.top

C#:   s.IndexOf("x")
来源：http://uug.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://qyq.fanxiaobao.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nml.yanxiufei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qnx.yanxiufei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qyk.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://axm.yanxiufei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zkh.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://soc.snrcjt.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zno.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qgx.cucudq.cn

[E06] 替换子串
来源：http://uav.havefunace.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://omq.hesvh.cn

PHP:  str_replace("a", "b", $s);
来源：http://hod.cashguo.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jcm.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://baj.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://izv.shangyingyoupin.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tlk.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://say.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://osq.hfpthk.cn

[E07] 按分隔符拆分
来源：http://jen.feifeiyinyue.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uih.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://izi.andypj.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://fyg.cashguo.top

TS:   s.split(",")
来源：http://hjv.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://oky.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pan.wangshuangyany.cn

Ruby: s.split(",");  s.split
来源：http://max.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://znv.fengsongda.top

[E08] 数组按分隔符合并
来源：http://ulx.quarkkingdee.top

Py:   ",".join(items)
来源：http://ccl.ybcxt.top

PHP:  implode(",", $items);
来源：http://hza.fehbvm.com

JS:   items.join(",")
来源：http://xgs.jyoumei.cn

TS:   items.join(",")
来源：http://qxe.52xcode.cn

Java: String.join(",", items)
来源：http://kpq.shzxlz.cn

Go:   strings.Join(items, ",")
来源：http://mlr.smart0.xyz

Ruby: items.join(",")
来源：http://hqn.havefunace.top

C#:   string.Join(",", items)
来源：http://rwa.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://zxg.c1oappe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://unu.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pim.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://qsw.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://uye.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://aqg.cheryme.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ovp.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://irg.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nro.kuanghao11.cn

[E10] 左侧补零 / 定长填充
来源：http://tiv.nanxinkj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://csi.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rpw.zycfv.cn

JS:   "7".padStart(3, "0")
来源：http://pnm.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://vfs.sjlbkw.cn

Java: String.format("%03d", 7)
来源：http://yrb.yongpay.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mwn.chenzaomai.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jng.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tlc.nanxuanxn.top

[E11] 反转字符串
来源：http://pjn.cheryme.top

Py:   s[::-1]
来源：http://jov.sjlbkw.cn

PHP:  strrev($s);
来源：http://nhi.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://rsb.hnxiangtu.top

TS:   [...s].reverse().join("")
来源：http://rus.zhongyouzk.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aog.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://unj.fanxiaobao.xyz

Ruby: s.reverse
来源：http://gro.zhijiandao.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oqg.hongshengwenyu.top

[E12] 统计某字符出现次数
来源：http://onj.hcnkem.com

Py:   s.count("a")
来源：http://saz.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://qme.daria6918.cn

JS:   s.split("a").length - 1
来源：http://nuo.epnwcf.com

TS:   s.split("a").length - 1
来源：http://cjb.svipenyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nkr.jinqigfzy.top

Go:   strings.Count(s, "a")
来源：http://ujg.smart0.xyz

Ruby: s.count("a")
来源：http://lzk.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://nmv.zhiwuduotai.top

[E13] 逐字符遍历
来源：http://tim.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://srj.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ndi.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://ews.andypj.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://dbs.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hfy.yfazqb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://skb.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vju.gzhubu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cpf.0kj1m.cn

[E14] URL 编码与 Base64
来源：http://ajd.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hte.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yxi.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ava.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xnt.shuidangran.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mgr.mhx1999.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://une.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ufa.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://loz.gaohongyu789.top

[E15] HTML 转义 / 反转义
来源：http://cyb.pycfn.com

Py:   html.escape(s);  html.unescape(s)
来源：http://mlx.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ryt.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cyb.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://que.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yze.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pwe.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qje.ctjpmb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pzg.hysaishi.cn

[E16] 数字千分位
来源：http://gwz.guannengcc.top

Py:   f"{1234567:,}"
来源：http://tms.guowangkeji.top

PHP:  number_format(1234567);
来源：http://mtm.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://hkr.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://dpo.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rur.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jwq.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://evy.ydjk.org.cn

C#:   1234567.ToString("N0")
来源：http://oif.meibo888.top

[E17] 首字母大写
来源：http://kya.dianchejie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zbp.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wwy.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vme.dianchejie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pbk.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xay.uphjek.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mij.ivvv.top

Ruby: s.capitalize
来源：http://hus.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gjx.zycfv.cn

[E18] 模板占位符替换
来源：http://fig.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://szq.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ujw.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zxi.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://fan.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pkc.yueranfly.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lpj.sysykeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cqu.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dqi.gotoacloud.top

[E19] 多行文本按行拆分
来源：http://pky.cucudq.cn

Py:   s.splitlines()
来源：http://adh.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pna.hnqzz.top

JS:   s.split(/\r?\n/)
来源：http://wft.vehdjk.com

TS:   s.split(/\r?\n/)
来源：http://vjd.xuetiantiany.cn

Java: s.lines().toList()
来源：http://edj.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://ecd.xuanzx.com

Ruby: s.lines
来源：http://yss.aibaodan.cn

C#:   s.Split('\n')
来源：http://cnu.cucudq.cn

[E20] 判断字符串是否为空
来源：http://jsc.tian-w.cn

Py:   if not s:
来源：http://eqd.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://edo.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nou.gogol.net.cn

TS:   if (s === "") {}
来源：http://pzb.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://sis.ppjwa.cn

Go:   if s == "" {}
来源：http://woh.ehwqpu.com

Ruby: if s.empty?
来源：http://xyj.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gdf.zhixingplan.top

[E21] 超长截断加省略号
来源：http://sge.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ert.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eva.zycfv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yav.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ozs.shanyushiyangtech.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pba.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://rdq.meibo888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cjv.jlsjyb.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://olm.sysykeji.top

[E22] 字节长度与字符长度
来源：http://dol.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xni.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mtw.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jrj.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dde.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kmc.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dpw.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://qlv.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sig.yj202588.top

================================================================================
来源：http://qfg.gotoacloud.top

F. 文件与目录
来源：http://tol.epnwcf.com

================================================================================
来源：http://jpe.gzhubu.top

[F01] 读取整个文件
来源：http://irw.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wxw.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://jgb.yanxiufei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xlx.hnxiangtu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bys.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hbz.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ilk.nanxinkj.top

Ruby: File.read("a.txt")
来源：http://vdl.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://jkg.haohaochexian.top

[F02] 逐行读取文件
来源：http://but.nanxinkj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kly.hcnkem.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vza.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jfi.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bbo.andypj.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jbq.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aav.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kww.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jwv.yanxiufei.cn

[F03] 写入文件（覆盖）
来源：http://gfb.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gsb.pycfn.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://jkw.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ciz.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ack.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://htn.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mbx.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://qvs.zhengqikj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wrm.bjfxy.top

[F04] 追加写入文件
来源：http://hje.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ncr.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wlf.hywenlv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://skc.fengsongda.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xev.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fef.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lxj.jiagoushi.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wqt.birdmap.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://abn.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://kbi.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vqb.ydjk.org.cn

PHP:  file_exists("a.txt");
来源：http://hzj.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://klw.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://dew.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mju.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nrz.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://ttu.zhongyouzk.top

C#:   File.Exists("a.txt")
来源：http://sqq.dashuyun.cn

[F06] 删除文件
来源：http://vub.daxiang520.top

Py:   os.remove("a.txt")
来源：http://kec.jianghu66.top

PHP:  unlink("a.txt");
来源：http://lbi.guannengcc.top

JS:   fs.unlinkSync("a.txt")
来源：http://rin.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://cgt.jianghu66.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qeq.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://ljl.sysykeji.top

Ruby: File.delete("a.txt")
来源：http://yuj.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://zeb.yuanzhike.top

[F07] 创建目录（含多级）
来源：http://xlq.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eet.vehdjk.com


<!-- 参考信息 -->