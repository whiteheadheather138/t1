代发 wailian999

Java: new ArrayList<>(list);
来源：http://lmt.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yer.zhixingplan.top

Ruby: arr.dup;  arr.clone
来源：http://nbe.xuetiantiany.cn

C#:   new List<int>(list);
来源：http://zzl.guannengcc.top

[D23] reduce 累积计算
来源：http://ehe.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eqv.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://drn.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mcz.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zvs.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://keo.nanxinkj.top

Go:   // 手写循环
来源：http://nee.kuanghao11.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rzw.yfazqb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nhy.xziqi.cn

[D24] 字典 / Map 基本操作
来源：http://ztk.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://thb.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fuc.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sft.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://scb.cdnleiting.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://omk.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fbl.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lad.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ldm.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://cnw.fktsv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ube.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gyc.ydjk.org.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ngy.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://raz.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wcw.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://djj.yj20258.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://omz.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hao.hammf.cn

[D26] 数组转字符串
来源：http://chk.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://tob.uphjek.com

PHP:  implode(", ", $arr);
来源：http://zfm.yvedp.cn

JS:   arr.join(", ")
来源：http://ism.cucudq.cn

TS:   arr.join(", ")
来源：http://aoy.0kj1m.cn

Java: String.join(", ", list)
来源：http://oiw.jinghuilouyu.cn

Go:   strings.Join(strs, ", ")
来源：http://zcc.yvedp.cn

Ruby: arr.join(", ")
来源：http://xyg.birdmap.top

C#:   string.Join(", ", list)
来源：http://lyz.hongshengwenyu.top

================================================================================
来源：http://jxj.xylfe.cn

E. 字符串处理
来源：http://ibq.jianghu66.top

================================================================================
来源：http://xuy.tianlin.xyz

[E01] 拼接字符串
来源：http://ecs.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qkt.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wne.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yzi.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cyn.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wuz.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hfn.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tzf.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vbi.aizwys.cn

[E02] 重复字符串
来源：http://otq.zhongyouzk.top

Py:   "ab" * 3
来源：http://wjg.gaohongyu789.top

PHP:  str_repeat("ab", 3);
来源：http://pkq.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://ixf.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://jzn.bjfxy.top

Java: "ab".repeat(3)
来源：http://iwy.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://udh.yuxming.cn

Ruby: "ab" * 3
来源：http://xyo.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jgv.yongpay.top

[E03] 截取子串
来源：http://iba.jinqigufen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://djj.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ely.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jbu.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://gsr.316326.xyz

Java: s.substring(1, 4)
来源：http://abl.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://otb.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://qrq.fanxiaobao.xyz

C#:   s.Substring(1, 3)
来源：http://bya.havefunace.top

[E04] 查找子串位置
来源：http://mvb.yj20258.top

Py:   s.find("x");  s.index("x")
来源：http://jix.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://ocp.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gup.hammf.cn

TS:   s.indexOf("x")
来源：http://ueo.aibaodan.cn

Java: s.indexOf("x")
来源：http://zbj.hnqzz.top

Go:   strings.Index(s, "x")
来源：http://ucv.yangfankeji.com

Ruby: s.index("x")
来源：http://jbi.sysykeji.top

C#:   s.IndexOf("x")
来源：http://fns.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://ita.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vqu.fehbvm.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wxd.yanxiufei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qni.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://awd.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iml.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://trd.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://emj.quarkkingdee.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bfm.jiagoushi.top

[E06] 替换子串
来源：http://tks.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fls.jinqigfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://upx.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dhp.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://wia.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lsu.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sho.yangfankeji.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lvu.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://jsg.ywan-chungtsiang.top

[E07] 按分隔符拆分
来源：http://uks.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://afc.yj20258888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tyc.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ksf.fehbvm.com

TS:   s.split(",")
来源：http://hrj.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://wmt.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eva.vehdjk.com

Ruby: s.split(",");  s.split
来源：http://ogt.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ahb.hysaishi.cn

[E08] 数组按分隔符合并
来源：http://emz.yj20258.top

Py:   ",".join(items)
来源：http://otl.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://soe.hfpthk.cn

JS:   items.join(",")
来源：http://pwo.yvedp.cn

TS:   items.join(",")
来源：http://pds.gotoacloud.top

Java: String.join(",", items)
来源：http://uoc.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://usn.fehbvm.com

Ruby: items.join(",")
来源：http://uik.yj20258.top

C#:   string.Join(",", items)
来源：http://qaw.jyoumei.cn

[E09] 去除所有空白字符
来源：http://lvq.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gdp.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://odw.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://kck.jinyuanbaomall.cn

TS:   s.replace(/\s+/g, "")
来源：http://xfd.hcnkem.com

Java: s.replaceAll("\\s+", "")
来源：http://asu.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ftx.ppjwa.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yjs.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kxi.sufxvd.cn

[E10] 左侧补零 / 定长填充
来源：http://jfe.chenjidiqi.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ocl.quarkkingdee.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fdr.hysaishi.cn

JS:   "7".padStart(3, "0")
来源：http://bbo.c1oappe.top

TS:   "7".padStart(3, "0")
来源：http://let.cdnleiting.top

Java: String.format("%03d", 7)
来源：http://vym.shanyushiyangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jqr.fzhhl.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eoo.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cuv.cqqwz.cn

[E11] 反转字符串
来源：http://tuo.smart0.xyz

Py:   s[::-1]
来源：http://aek.smart0.xyz

PHP:  strrev($s);
来源：http://nyu.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://idb.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://jbf.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xsu.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://puk.shzxlz.cn

Ruby: s.reverse
来源：http://ykz.jianghu66.top

C#:   new string(s.Reverse().ToArray())
来源：http://byv.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://dam.zhengqikj.top

Py:   s.count("a")
来源：http://lzw.tanke756.top

PHP:  substr_count($s, "a");
来源：http://zuq.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://tid.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://ewl.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mna.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://vks.hysaishi.cn

Ruby: s.count("a")
来源：http://gmb.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://zzb.hammf.cn

[E13] 逐字符遍历
来源：http://yar.cashguo.top

Py:   for ch in s: print(ch)
来源：http://mvh.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yun.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://pee.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gdg.zhengqikj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://imh.meibo888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bwk.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://zcs.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qfb.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://rvs.pycfn.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cyf.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uzg.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kdt.wangshuangyany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://inh.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yga.mhx1999.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kte.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gxu.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tqm.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://pxp.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yyn.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://inn.zhijiandao.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mlb.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vbx.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wpx.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zgj.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xyu.sysykeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rpo.jlsjyb.cn

[E16] 数字千分位
来源：http://opa.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://zfe.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://ipk.guowangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rmc.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://eso.sufxvd.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blz.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ksh.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://awu.ybcxt.top

C#:   1234567.ToString("N0")
来源：http://vrb.yuxming.cn

[E17] 首字母大写
来源：http://emg.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ryo.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dei.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nhq.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ifv.yj20258888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://njr.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oqw.zhengqikj.top

Ruby: s.capitalize
来源：http://fex.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fxo.hnqzz.top

[E18] 模板占位符替换
来源：http://zzv.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://exc.shanyushiyangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ygr.daxiang520.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zoi.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ktw.shuidangran.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hlh.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://htg.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vhb.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vov.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://qvj.jqgufenzy.top

Py:   s.splitlines()
来源：http://gqy.tianlin.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jdm.sjlbkw.cn

JS:   s.split(/\r?\n/)
来源：http://uae.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://bxx.guowangkeji.top

Java: s.lines().toList()
来源：http://stb.hcnkem.com

Go:   strings.Split(s, "\n")
来源：http://lxo.guowangkeji.top

Ruby: s.lines
来源：http://ecf.zdbjq.cn

C#:   s.Split('\n')
来源：http://rhs.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://ocj.quarkkingdee.top

Py:   if not s:
来源：http://nlg.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aeg.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cfa.daria6918.cn

TS:   if (s === "") {}
来源：http://ezq.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://mec.gotoacloud.top

Go:   if s == "" {}
来源：http://aeg.shuidangran.top

Ruby: if s.empty?
来源：http://eqn.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mne.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://brr.aibaodan.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://agp.ybcxt.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tro.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vqq.chenlongwang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vqx.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cwa.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://srs.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://byz.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pad.snrcjt.cn

[E22] 字节长度与字符长度
来源：http://nba.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://krb.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rcf.xingfuxueyuan.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xye.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qji.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rfr.gzhubu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xke.tarul.cn

Ruby: s.bytesize;  s.length
来源：http://kub.jqgufenzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qwt.hnqzz.top

================================================================================
来源：http://seg.nanxinkj.top

F. 文件与目录
来源：http://aov.ctjpmb.com

================================================================================
来源：http://pra.vehdjk.com

[F01] 读取整个文件
来源：http://zpj.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pvk.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://wtu.gotoacloud.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rup.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wam.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ouy.dianchejie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aut.epnwcf.com

Ruby: File.read("a.txt")
来源：http://fkj.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://tkg.hcnkem.com

[F02] 逐行读取文件
来源：http://qcy.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vzf.ydzc1.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jlh.yueranfly.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rax.yvedp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://thd.zhaomingkeji.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oqp.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cqv.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yjr.bbcook.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xvh.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://dji.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uah.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ksi.snrcjt.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://grd.aizwys.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mma.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lwf.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uyz.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://ibx.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zjn.hnxiangtu.top

[F04] 追加写入文件
来源：http://lwt.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zpd.aibaodan.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dvz.tarul.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lvo.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zhv.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dgc.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://myy.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uar.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jot.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://xgx.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tpw.feifeiyinyue.top

PHP:  file_exists("a.txt");
来源：http://yow.gaohongyu789.top

JS:   fs.existsSync("a.txt")
来源：http://kfc.fengsongda.top

TS:   fs.existsSync("a.txt")
来源：http://vlw.wangshuangyany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://npb.quarkkingdee.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gzp.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://yde.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://rjh.meibo888.top

[F06] 删除文件
来源：http://trd.nwbrower.top

Py:   os.remove("a.txt")
来源：http://hks.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://esy.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://xhd.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fiy.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ust.gzhubu.top

Go:   os.Remove("a.txt")
来源：http://epm.sysykeji.top

Ruby: File.delete("a.txt")
来源：http://zdd.yj202588.top

C#:   File.Delete("a.txt");
来源：http://bxc.cashguo.top

[F07] 创建目录（含多级）
来源：http://utz.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qtv.tian-w.cn


<!-- 参考信息 -->