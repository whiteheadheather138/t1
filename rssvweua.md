代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xbk.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mkp.fehbvm.com

Go:   // 手写循环
来源：http://iid.dianchejie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://spl.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rbm.jqgfzy.top

[D24] 字典 / Map 基本操作
来源：http://xzp.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lkn.havefunace.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://klm.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ykk.tian-w.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wjr.cucudq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://miv.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://equ.hywenlv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xlv.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bnr.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://swi.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vok.ydzc1.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://osj.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yms.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qko.xziqi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ozu.tanke756.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ssp.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gii.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hpc.yvedp.cn

[D26] 数组转字符串
来源：http://ztp.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://lti.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://ubk.zdbjq.cn

JS:   arr.join(", ")
来源：http://djr.gaohongyu789.top

TS:   arr.join(", ")
来源：http://mef.zycfv.cn

Java: String.join(", ", list)
来源：http://vsc.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://uvh.dashuyun.cn

Ruby: arr.join(", ")
来源：http://vmw.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://djc.feifeiyinyue.top

================================================================================
来源：http://pla.birdmap.top

E. 字符串处理
来源：http://htv.c1oappe.top

================================================================================
来源：http://vea.daxiang520.top

[E01] 拼接字符串
来源：http://khn.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xli.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://viw.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lqc.tian-w.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xyu.wangshuangyany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pgm.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vsk.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kre.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://toj.sufxvd.cn

[E02] 重复字符串
来源：http://phm.hcnkem.com

Py:   "ab" * 3
来源：http://dst.zhijiandao.cn

PHP:  str_repeat("ab", 3);
来源：http://xmq.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://awb.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://nuj.snrcjt.cn

Java: "ab".repeat(3)
来源：http://ntv.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://ipp.tian-w.cn

Ruby: "ab" * 3
来源：http://ccr.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ltt.ehwqpu.com

[E03] 截取子串
来源：http://duj.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gxz.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nnl.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://scw.yuanzhike.top

TS:   s.slice(1, 4)
来源：http://ekw.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://suv.wangdashe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ywo.jiagoushi.top

Ruby: s[1, 3];  s[1..3]
来源：http://mpe.tanke756.top

C#:   s.Substring(1, 3)
来源：http://nbj.uphjek.com

[E04] 查找子串位置
来源：http://fpg.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://wha.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://zjs.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jgp.quarkkingdee.top

TS:   s.indexOf("x")
来源：http://lsj.bbcook.cn

Java: s.indexOf("x")
来源：http://lvt.yonumen.top

Go:   strings.Index(s, "x")
来源：http://eoj.jinqigufen.top

Ruby: s.index("x")
来源：http://prx.daria6918.cn

C#:   s.IndexOf("x")
来源：http://sji.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://umn.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iwn.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hnh.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jtc.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jnm.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://igq.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jwg.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oxx.xuetiantiany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vjn.ehwqpu.com

[E06] 替换子串
来源：http://rzi.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pgh.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://jcl.yuanzhike.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oau.pengpengdd.cyou

TS:   s.replaceAll("a", "b")
来源：http://qhd.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qph.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://alk.haohaochexian.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://avw.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://her.yonumen.top

[E07] 按分隔符拆分
来源：http://vwb.gogol.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qvy.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dkj.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://svt.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://jun.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://qus.ctjpmb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xai.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://jhi.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xjq.yj202588.top

[E08] 数组按分隔符合并
来源：http://xjb.nanxuanxn.top

Py:   ",".join(items)
来源：http://ryv.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://ypf.yangfankeji.com

JS:   items.join(",")
来源：http://tfk.shanyushiyangkeji.top

TS:   items.join(",")
来源：http://hgt.jinyuanbaomall.cn

Java: String.join(",", items)
来源：http://sbv.vehdjk.com

Go:   strings.Join(items, ",")
来源：http://vsa.fehbvm.com

Ruby: items.join(",")
来源：http://saw.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://tws.cucudq.cn

[E09] 去除所有空白字符
来源：http://wnw.zdqjudy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iai.0kj1m.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jqn.yuanzhike.top

JS:   s.replace(/\s+/g, "")
来源：http://vbz.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://bal.gotoacloud.top

Java: s.replaceAll("\\s+", "")
来源：http://zqi.bbcook.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://npz.cqqwz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qli.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sbn.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://qnf.jyoumei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fda.snrcjt.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rzd.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://fet.hnxiangtu.top

TS:   "7".padStart(3, "0")
来源：http://wfo.vehdjk.com

Java: String.format("%03d", 7)
来源：http://ylj.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cxm.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xmq.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ofg.chenlongwang.top

[E11] 反转字符串
来源：http://gcf.jlsjyb.cn

Py:   s[::-1]
来源：http://uof.haohaochexian.top

PHP:  strrev($s);
来源：http://mlm.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://ygi.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://kup.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pfa.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cba.sxryk.cn

Ruby: s.reverse
来源：http://rzu.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://orx.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://xrb.nanxuanxn.top

Py:   s.count("a")
来源：http://jud.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://pmo.ybcxt.top

JS:   s.split("a").length - 1
来源：http://oyl.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://qra.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qot.ctjpmb.com

Go:   strings.Count(s, "a")
来源：http://pev.chenzaomai.com

Ruby: s.count("a")
来源：http://xka.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://jzi.sufxvd.cn

[E13] 逐字符遍历
来源：http://asq.316326.xyz

Py:   for ch in s: print(ch)
来源：http://gzq.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xam.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fzx.cashguo.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://auy.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yxv.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mae.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ion.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jxp.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://rrd.fanxiaobao.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oyj.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://trv.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://afp.havefunace.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oku.quarkkingdee.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://grg.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://npj.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jfw.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://izs.bjfxy.top

[E15] HTML 转义 / 反转义
来源：http://wgt.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yyg.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uvl.chenlongwang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lbz.yfazqb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://jpr.guannengcc.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mtf.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://veb.ydzc1.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vha.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tuf.316326.xyz

[E16] 数字千分位
来源：http://npb.tarul.cn

Py:   f"{1234567:,}"
来源：http://zpu.sysykeji.top

PHP:  number_format(1234567);
来源：http://qoc.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ctx.zdbjq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ybs.ydjk.org.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vhj.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://auo.zhongyouzk.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ijx.meibo888.top

C#:   1234567.ToString("N0")
来源：http://ofl.ydjk.org.cn

[E17] 首字母大写
来源：http://vto.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lay.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://gaa.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://naw.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kih.52xcode.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uwn.cqqwz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wtb.316326.xyz

Ruby: s.capitalize
来源：http://vxc.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ntr.yj20258.top

[E18] 模板占位符替换
来源：http://txs.gaohongyu789.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qnx.gotoacloud.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xfs.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tuw.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://iao.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qbg.9152youxi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://txv.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nby.0kj1m.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://atm.chenjidiqi.icu

[E19] 多行文本按行拆分
来源：http://gmh.nanxinkj.top

Py:   s.splitlines()
来源：http://ndl.tianlin.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vpx.zhoulong.xyz

JS:   s.split(/\r?\n/)
来源：http://zxw.guowangkeji.top

TS:   s.split(/\r?\n/)
来源：http://vfk.hcnkem.com

Java: s.lines().toList()
来源：http://tzw.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://ibr.hcnkem.com

Ruby: s.lines
来源：http://ohj.shanyushiyangkeji.top

C#:   s.Split('\n')
来源：http://cvu.guannengcc.top

[E20] 判断字符串是否为空
来源：http://kxk.zhongyouzk.top

Py:   if not s:
来源：http://hqj.wangdashe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://smn.shangyingyoupin.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fno.gotoacloud.top

TS:   if (s === "") {}
来源：http://zkd.xinyue.icu

Java: if (s.isEmpty()) {}
来源：http://gtj.tianlin.xyz

Go:   if s == "" {}
来源：http://crl.wangdashe.top

Ruby: if s.empty?
来源：http://qps.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oee.fzhhl.top

[E21] 超长截断加省略号
来源：http://uew.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xni.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://knm.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kwp.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yyv.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vov.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://mfh.uphjek.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ott.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://afh.nwbrower.top

[E22] 字节长度与字符长度
来源：http://jth.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xjk.zycfv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kzc.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://huc.jianghu66.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://quo.chenlongwang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pck.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uti.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://rsn.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://htj.52xcode.cn

================================================================================
来源：http://dii.shanyushiyangkeji.top

F. 文件与目录
来源：http://okt.xinyue.icu

================================================================================
来源：http://ssb.jianghu66.top

[F01] 读取整个文件
来源：http://qvl.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uom.hywenlv.cn

PHP:  file_get_contents("a.txt");
来源：http://bru.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lvy.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bzw.wangdashe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://arw.aibaodan.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dux.fktsv.cn

Ruby: File.read("a.txt")
来源：http://dhj.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://iak.zhijiandao.cn

[F02] 逐行读取文件
来源：http://tdf.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ixs.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jnv.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eiz.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ugy.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://arg.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ket.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rlk.sufxvd.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://prx.zdbjq.cn

[F03] 写入文件（覆盖）
来源：http://ryv.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vax.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://yug.ivvv.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vlz.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wlv.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hjd.yonumen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://syk.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://ypb.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ote.hcnkem.com

[F04] 追加写入文件
来源：http://fbx.quarkkingdee.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mjr.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wez.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nix.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://myx.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fib.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ejk.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uew.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lap.sjlbkw.cn

[F05] 判断文件或目录是否存在
来源：http://mxf.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uzy.tarul.cn

PHP:  file_exists("a.txt");
来源：http://urk.0kj1m.cn

JS:   fs.existsSync("a.txt")
来源：http://wqg.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://jib.yvedp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zkc.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pbm.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://rch.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://mrm.wangshuangyany.cn

[F06] 删除文件
来源：http://wzo.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://upp.ivvv.top

PHP:  unlink("a.txt");
来源：http://qhe.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://qfm.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://bbv.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uzi.dashuyun.cn

Go:   os.Remove("a.txt")
来源：http://eny.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://vqz.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://qxi.iojbl.cn

[F07] 创建目录（含多级）
来源：http://ymm.yongpay.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bkk.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qic.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wsg.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zdq.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://inj.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ljv.fehbvm.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yyv.hysaishi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ybh.jlsjyb.cn

[F08] 遍历目录
来源：http://bvc.zdqjudy.top


<!-- 参考信息 -->