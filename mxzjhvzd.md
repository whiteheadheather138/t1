代发 wailian999

Java: new ArrayList<>(list);
来源：http://wvw.dianchejie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://avi.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://pcf.hesvh.cn

C#:   new List<int>(list);
来源：http://zkp.iojbl.cn

[D23] reduce 累积计算
来源：http://exe.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lxf.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ejj.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cwl.yuxming.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kxa.uphjek.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://bvt.yvedp.cn

Go:   // 手写循环
来源：http://npt.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nyk.sjlbkw.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xrc.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://osm.daxiang520.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dbb.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dfz.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dma.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kho.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qoc.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rem.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://irp.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sis.ctjpmb.com

[D25] Set 集合去重与交并差
来源：http://dwg.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://czd.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kvr.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nff.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pbh.fehbvm.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wdj.yueranfly.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oeu.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ahy.zhiwuduotai.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mds.aizwys.cn

[D26] 数组转字符串
来源：http://rse.dashuyun.cn

Py:   ", ".join(map(str, arr))
来源：http://ypi.sjlbkw.cn

PHP:  implode(", ", $arr);
来源：http://acs.hnxiangtu.top

JS:   arr.join(", ")
来源：http://moc.ppjwa.cn

TS:   arr.join(", ")
来源：http://ijn.yvedp.cn

Java: String.join(", ", list)
来源：http://nth.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://hwk.daxiang520.top

Ruby: arr.join(", ")
来源：http://tge.daxiang520.top

C#:   string.Join(", ", list)
来源：http://oyk.redwolf501.top

================================================================================
来源：http://wae.0kj1m.cn

E. 字符串处理
来源：http://jjb.mhx1999.top

================================================================================
来源：http://cpt.smart0.xyz

[E01] 拼接字符串
来源：http://yas.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aey.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://leo.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wsm.9152youxi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ngm.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ehu.shuidangran.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ncr.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fdu.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://noc.sysykeji.top

[E02] 重复字符串
来源：http://hcf.chenzaomai.com

Py:   "ab" * 3
来源：http://spe.wangdashe.top

PHP:  str_repeat("ab", 3);
来源：http://wmw.daria6918.cn

JS:   "ab".repeat(3)
来源：http://tvc.pycfn.com

TS:   "ab".repeat(3)
来源：http://wyj.jlsjyb.cn

Java: "ab".repeat(3)
来源：http://moq.snrcjt.cn

Go:   strings.Repeat("ab", 3)
来源：http://wix.xinyue.icu

Ruby: "ab" * 3
来源：http://dex.jinghuilouyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ppn.hfpthk.cn

[E03] 截取子串
来源：http://zba.shanyushiyangtech.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yqv.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uwe.yj20258888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://csm.fehbvm.com

TS:   s.slice(1, 4)
来源：http://ojb.hammf.cn

Java: s.substring(1, 4)
来源：http://fyg.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oxw.yj202588.top

Ruby: s[1, 3];  s[1..3]
来源：http://wsk.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://kbu.jqgfzy.top

[E04] 查找子串位置
来源：http://xma.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://ftq.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://dyx.mhx1999.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kiq.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://kab.cheryme.top

Java: s.indexOf("x")
来源：http://fis.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://srl.jlsjyb.cn

Ruby: s.index("x")
来源：http://dps.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://qlp.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wny.yuanzhike.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://riq.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vqi.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sfp.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ejx.tianlin.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fhi.jlsjyb.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pky.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vio.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fuz.aizwys.cn

[E06] 替换子串
来源：http://czk.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nlk.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://ief.cashguo.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jfm.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://uio.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nyg.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://znb.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rxr.snrcjt.cn

C#:   s.Replace("a", "b")
来源：http://fvh.yueranfly.top

[E07] 按分隔符拆分
来源：http://pzl.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wti.nwbrower.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jnr.ivvv.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://isw.havefunace.top

TS:   s.split(",")
来源：http://vrk.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://ixz.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cma.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://gfj.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uxv.chenjidiqi.icu

[E08] 数组按分隔符合并
来源：http://ytp.52xcode.cn

Py:   ",".join(items)
来源：http://nxv.yangfankeji.com

PHP:  implode(",", $items);
来源：http://njy.shanyushiyangkeji.top

JS:   items.join(",")
来源：http://shp.c1oappe.top

TS:   items.join(",")
来源：http://lap.shanyushiyangtech.top

Java: String.join(",", items)
来源：http://tfm.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://nqy.gogol.net.cn

Ruby: items.join(",")
来源：http://hly.316326.xyz

C#:   string.Join(",", items)
来源：http://ltd.xinyue.icu

[E09] 去除所有空白字符
来源：http://ven.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tij.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://otn.vqdsnc.cn

JS:   s.replace(/\s+/g, "")
来源：http://ber.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://nta.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://lbp.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xum.aibaodan.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ngs.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hql.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://gqo.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jsl.xuanzx.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mim.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://rzs.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://xyb.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://ehd.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://era.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bmx.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ghy.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://bry.dianchejie.cn

Py:   s[::-1]
来源：http://xax.hysaishi.cn

PHP:  strrev($s);
来源：http://yfq.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://shg.zhixingplan.top

TS:   [...s].reverse().join("")
来源：http://cwq.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zaw.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://bju.chenlongwang.top

Ruby: s.reverse
来源：http://eif.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://ejz.cucudq.cn

[E12] 统计某字符出现次数
来源：http://jha.cdnleiting.top

Py:   s.count("a")
来源：http://sxo.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://oeq.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://zmc.shanyushiyangtech.top

TS:   s.split("a").length - 1
来源：http://fob.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hws.zhongyouzk.top

Go:   strings.Count(s, "a")
来源：http://mwi.dianchejie.cn

Ruby: s.count("a")
来源：http://sus.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://mbd.vehdjk.com

[E13] 逐字符遍历
来源：http://aye.yvedp.cn

Py:   for ch in s: print(ch)
来源：http://xha.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sai.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ytq.hammf.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lfj.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cki.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xup.sysykeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rkg.jiagoushi.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uzn.smart0.xyz

[E14] URL 编码与 Base64
来源：http://ilv.ppjwa.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://neh.sysykeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://raj.shanyushiyangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://taf.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zul.ybcxt.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nyp.ywan-chungtsiang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sim.epnwcf.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://npt.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pgh.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://ngi.uphjek.com

Py:   html.escape(s);  html.unescape(s)
来源：http://srf.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://asy.vqdsnc.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pbw.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zff.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ycn.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sqd.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://umm.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gut.ppjwa.cn

[E16] 数字千分位
来源：http://yet.quarkkingdee.top

Py:   f"{1234567:,}"
来源：http://fpj.nanxinkj.top

PHP:  number_format(1234567);
来源：http://qvz.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://swv.cashguo.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qqy.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ost.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://epg.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nnm.dianchejie.cn

C#:   1234567.ToString("N0")
来源：http://jmy.uphjek.com

[E17] 首字母大写
来源：http://jdl.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://evn.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pie.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tqo.jinyuanbaomall.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://puu.chenzaomai.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xjp.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qvt.feifeiyinyue.top

Ruby: s.capitalize
来源：http://jwz.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xff.jianghu66.top

[E18] 模板占位符替换
来源：http://hwv.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yxw.birdmap.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dew.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://prp.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://taw.zycfv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jxt.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jgv.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wmg.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qhl.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://azh.yueranfly.top

Py:   s.splitlines()
来源：http://qio.ydzc1.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sjx.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://arj.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://gzt.yongpay.top

Java: s.lines().toList()
来源：http://hsm.hongshengwenyu.top

Go:   strings.Split(s, "\n")
来源：http://ofp.yvedp.cn

Ruby: s.lines
来源：http://iwi.cashguo.top

C#:   s.Split('\n')
来源：http://rxg.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://ptf.zhixingplan.top

Py:   if not s:
来源：http://jgl.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ati.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hsg.guannengcc.top

TS:   if (s === "") {}
来源：http://cgp.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://mjx.cqqwz.cn

Go:   if s == "" {}
来源：http://pmd.uphjek.com

Ruby: if s.empty?
来源：http://tzz.ivvv.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://foi.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://ccj.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lbh.hnxiangtu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://icr.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wpo.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ram.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zdt.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://tlg.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mwe.fehbvm.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rvr.mhx1999.top

[E22] 字节长度与字符长度
来源：http://oxz.nanxinkj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jjl.gaohongyu789.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gxx.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nrb.fehbvm.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jgs.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zto.ehwqpu.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yrp.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://cvy.gzhubu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://het.hnqzz.top

================================================================================
来源：http://njk.jyoumei.cn

F. 文件与目录
来源：http://zmc.hnqzz.top

================================================================================
来源：http://aoc.pycfn.com

[F01] 读取整个文件
来源：http://zfe.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lpf.0kj1m.cn

PHP:  file_get_contents("a.txt");
来源：http://slz.kuanghao11.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bjt.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://umb.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gyc.epnwcf.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ibs.feifeiyinyue.top

Ruby: File.read("a.txt")
来源：http://tgv.guannengcc.top

C#:   File.ReadAllText("a.txt");
来源：http://svz.nanxinkj.top

[F02] 逐行读取文件
来源：http://pnv.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://stw.ehwqpu.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jnm.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tyl.havefunace.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vur.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fcy.jyoumei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://edz.sysykeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://idc.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eit.nanxinkj.top

[F03] 写入文件（覆盖）
来源：http://luu.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://urs.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://irv.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iyt.quarkkingdee.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dbg.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cwc.nanxuanxn.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hcj.jianghu66.top

Ruby: File.write("a.txt", "hi")
来源：http://sgh.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pgk.jlsjyb.cn

[F04] 追加写入文件
来源：http://abj.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://idf.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cxu.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jgg.gzhubu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pvr.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://knn.yanxiufei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uzd.pycfn.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://edd.havefunace.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nrb.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://nbc.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qfs.birdmap.top

PHP:  file_exists("a.txt");
来源：http://thh.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://ymb.tanke756.top

TS:   fs.existsSync("a.txt")
来源：http://nur.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wwt.tarul.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ypx.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://chh.wangshuangyany.cn

C#:   File.Exists("a.txt")
来源：http://aei.zhixingplan.top

[F06] 删除文件
来源：http://sxr.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://iqc.fzhhl.top

PHP:  unlink("a.txt");
来源：http://qch.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lqw.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://chc.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kwv.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://pau.shanyushiyangtech.top

Ruby: File.delete("a.txt")
来源：http://brd.guannengcc.top

C#:   File.Delete("a.txt");
来源：http://eeh.yonumen.top

[F07] 创建目录（含多级）
来源：http://pnr.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dka.chenzaomai.com


<!-- 参考信息 -->