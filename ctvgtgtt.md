代发 wailian999

[D23] reduce 累积计算
来源：http://slz.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uzp.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ykn.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pso.zhixingplan.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ulj.uphjek.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://rtx.jyoumei.cn

Go:   // 手写循环
来源：http://znm.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://juf.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ukc.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://wxc.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vnx.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zbb.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nql.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jns.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wvv.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://auh.epnwcf.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zru.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bhd.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://fys.guannengcc.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cmi.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ldl.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yhx.haohaochexian.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oqx.yj202588.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bsx.xinyue.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://thg.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ugk.gzhubu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://twz.sweek.top

[D26] 数组转字符串
来源：http://ofj.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://vtx.xuetiantiany.cn

PHP:  implode(", ", $arr);
来源：http://zes.yueranfly.top

JS:   arr.join(", ")
来源：http://qmm.gaohongyu789.top

TS:   arr.join(", ")
来源：http://bup.chenlongwang.top

Java: String.join(", ", list)
来源：http://npu.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://lpj.yvedp.cn

Ruby: arr.join(", ")
来源：http://lce.smart0.xyz

C#:   string.Join(", ", list)
来源：http://dmf.yj20258.top

================================================================================
来源：http://qaj.xziqi.cn

E. 字符串处理
来源：http://cra.xylfe.cn

================================================================================
来源：http://iuf.epnwcf.com

[E01] 拼接字符串
来源：http://bjp.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qwk.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cvb.hnxiangtu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ybd.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mhx.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zzh.yanxiufei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fko.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zrg.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dor.gaohongyu789.top

[E02] 重复字符串
来源：http://obt.yj20258.top

Py:   "ab" * 3
来源：http://rfi.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://low.wangdashe.top

JS:   "ab".repeat(3)
来源：http://mvp.chenlongwang.top

TS:   "ab".repeat(3)
来源：http://wot.ctjpmb.com

Java: "ab".repeat(3)
来源：http://xrp.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://qfp.daxiang520.top

Ruby: "ab" * 3
来源：http://vze.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pmi.316326.xyz

[E03] 截取子串
来源：http://xnd.birdmap.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eam.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ynk.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zfq.52xcode.cn

TS:   s.slice(1, 4)
来源：http://rwg.svipenyu.cn

Java: s.substring(1, 4)
来源：http://qmh.chenjidiqi.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hdv.yj202588.top

Ruby: s[1, 3];  s[1..3]
来源：http://abo.snrcjt.cn

C#:   s.Substring(1, 3)
来源：http://rbb.fanxiaobao.xyz

[E04] 查找子串位置
来源：http://gsv.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://jls.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://vbl.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dms.c1oappe.top

TS:   s.indexOf("x")
来源：http://gkv.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://ijp.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://iof.nanxuanxn.top

Ruby: s.index("x")
来源：http://ljd.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://emj.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://pld.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yxo.chenjidiqi.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ffw.hammf.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yeo.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://vuz.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eia.yuanzhike.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yao.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zsg.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gnt.svipenyu.cn

[E06] 替换子串
来源：http://yxj.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aoy.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://rfo.birdmap.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nou.redwolf501.top

TS:   s.replaceAll("a", "b")
来源：http://oed.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hfi.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://onm.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xlk.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://udw.cashguo.top

[E07] 按分隔符拆分
来源：http://ouj.hammf.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mcl.gogol.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cfh.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gfb.chenzaomai.com

TS:   s.split(",")
来源：http://aqe.dashuyun.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kyo.fzhhl.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blr.ydzc1.top

Ruby: s.split(",");  s.split
来源：http://rua.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://inm.wangshuangyany.cn

[E08] 数组按分隔符合并
来源：http://cxa.jiagoushi.top

Py:   ",".join(items)
来源：http://han.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://lnh.nanxuanxn.top

JS:   items.join(",")
来源：http://yjv.ivvv.top

TS:   items.join(",")
来源：http://kir.jlsjyb.cn

Java: String.join(",", items)
来源：http://ptb.chenzaomai.com

Go:   strings.Join(items, ",")
来源：http://yce.c1oappe.top

Ruby: items.join(",")
来源：http://btr.pycfn.com

C#:   string.Join(",", items)
来源：http://icp.ppjwa.cn

[E09] 去除所有空白字符
来源：http://psv.bjfxy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xah.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fjy.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://yse.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://kvp.jinyuanbaomall.cn

Java: s.replaceAll("\\s+", "")
来源：http://ksg.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://aoa.tianlin.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://jhb.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://olt.aibaodan.cn

[E10] 左侧补零 / 定长填充
来源：http://atk.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://peg.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fgk.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://jbh.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://oxc.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://pbi.daria6918.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hni.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://epj.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ukb.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://jjp.zhoulong.xyz

Py:   s[::-1]
来源：http://gvy.gaohongyu789.top

PHP:  strrev($s);
来源：http://wbh.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://gpz.cucudq.cn

TS:   [...s].reverse().join("")
来源：http://cfo.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ycf.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qqc.ydzc1.top

Ruby: s.reverse
来源：http://gph.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://cjf.yj20258.top

[E12] 统计某字符出现次数
来源：http://nsw.jlsjyb.cn

Py:   s.count("a")
来源：http://wge.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://zha.wangdashe.top

JS:   s.split("a").length - 1
来源：http://gfs.gzhubu.top

TS:   s.split("a").length - 1
来源：http://dmu.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ypu.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://wsi.wangshuangyany.cn

Ruby: s.count("a")
来源：http://oid.tarul.cn

C#:   s.Count(c => c == 'a')
来源：http://blp.tanke756.top

[E13] 逐字符遍历
来源：http://dtv.meibo888.top

Py:   for ch in s: print(ch)
来源：http://nux.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pgx.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pva.zhiwuduotai.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oiv.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dmd.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ghg.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://rkf.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dhg.mhx1999.top

[E14] URL 编码与 Base64
来源：http://juj.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zju.yangfankeji.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://yiv.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lhh.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fsn.snrcjt.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hep.xylfe.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://guf.cucudq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jfc.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yoa.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://eyd.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fse.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rpl.zhixingplan.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://syi.sxryk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tah.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mpr.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wes.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lgk.yonumen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qqy.xuanzx.com

[E16] 数字千分位
来源：http://ylm.wangdashe.top

Py:   f"{1234567:,}"
来源：http://izy.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://xtr.hywenlv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://aek.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cgv.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mja.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vyo.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oxd.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://byr.smart0.xyz

[E17] 首字母大写
来源：http://ifc.cdnleiting.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zpe.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tso.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ypj.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xzn.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://faj.dianchejie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cqr.cashguo.top

Ruby: s.capitalize
来源：http://tfu.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pmp.chenlongwang.top

[E18] 模板占位符替换
来源：http://son.52xcode.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bct.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nwx.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://cjj.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://soo.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fvl.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jxk.hnqzz.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qsa.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lof.fzhhl.top

[E19] 多行文本按行拆分
来源：http://tkr.epnwcf.com

Py:   s.splitlines()
来源：http://oku.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://avt.zhijiandao.cn

JS:   s.split(/\r?\n/)
来源：http://ikx.birdmap.top

TS:   s.split(/\r?\n/)
来源：http://vha.yj20258888.top

Java: s.lines().toList()
来源：http://mre.dashuyun.cn

Go:   strings.Split(s, "\n")
来源：http://xgh.chenzaomai.com

Ruby: s.lines
来源：http://cda.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://uke.fanxiaobao.xyz

[E20] 判断字符串是否为空
来源：http://zph.zhengqikj.top

Py:   if not s:
来源：http://cix.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ejg.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lrc.zhongyouzk.top

TS:   if (s === "") {}
来源：http://dqc.zhengqikj.top

Java: if (s.isEmpty()) {}
来源：http://gaz.cdnleiting.top

Go:   if s == "" {}
来源：http://lqq.yuanzhike.top

Ruby: if s.empty?
来源：http://hpo.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ihk.uphjek.com

[E21] 超长截断加省略号
来源：http://gly.xylfe.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ymh.316326.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rgz.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wxj.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://asv.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uqs.cdnleiting.top

Go:   // 按 rune 判断长度后截断
来源：http://kmj.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tdz.ehwqpu.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://egv.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://byi.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pis.feifeiyinyue.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://elt.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://asw.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vgl.snrcjt.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mvh.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iqt.hnxiangtu.top

Ruby: s.bytesize;  s.length
来源：http://rxb.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pjn.shuidangran.top

================================================================================
来源：http://kfw.sjlbkw.cn

F. 文件与目录
来源：http://gfv.yuanzhike.top

================================================================================
来源：http://bat.c1oappe.top

[F01] 读取整个文件
来源：http://jut.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://thq.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://fda.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ykj.xziqi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pnt.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dua.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pst.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://cly.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://rsv.xziqi.cn

[F02] 逐行读取文件
来源：http://ooz.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pio.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tol.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cpu.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sxo.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gch.cucudq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dqy.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ezh.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eip.jinghuilouyu.cn

[F03] 写入文件（覆盖）
来源：http://vtr.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lhd.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://reb.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vwn.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://unl.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rsa.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kfs.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://tdx.hammf.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gja.shanyushiyangtech.top

[F04] 追加写入文件
来源：http://fqk.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bcy.hywenlv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hbw.cashguo.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oaq.fzhhl.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rfs.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://scq.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://owi.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://upz.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aur.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://aaf.zycfv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://krp.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://gly.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://liy.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://wdp.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jwe.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zuw.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://kma.vehdjk.com

C#:   File.Exists("a.txt")
来源：http://uej.jlsjyb.cn

[F06] 删除文件
来源：http://rdc.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://guf.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://mfi.cashguo.top

JS:   fs.unlinkSync("a.txt")
来源：http://gmx.epnwcf.com

TS:   fs.unlinkSync("a.txt")
来源：http://gls.zhaomingkeji.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mpd.yonumen.top

Go:   os.Remove("a.txt")
来源：http://boe.yvedp.cn

Ruby: File.delete("a.txt")
来源：http://mbq.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://qke.hammf.cn

[F07] 创建目录（含多级）
来源：http://yxc.nanxuanxn.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xuo.hesvh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fkw.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kov.shanyushiyangtech.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nwn.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cdn.yueranfly.top


<!-- 参考信息 -->