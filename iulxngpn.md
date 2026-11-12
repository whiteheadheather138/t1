代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://cyw.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://gto.zhoulong.xyz

C#:   list.Contains(x)
来源：http://vmp.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://lrv.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pnn.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ijj.hfpthk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cxl.iojbl.cn

TS:   [...arr];
来源：http://kfg.tian-w.cn

Java: new ArrayList<>(list);
来源：http://dcx.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://djb.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://usm.gogol.net.cn

C#:   new List<int>(list);
来源：http://tzm.zdbjq.cn

[D23] reduce 累积计算
来源：http://wyo.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xto.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hpt.wangdashe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pgk.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rqc.chenlongwang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://snk.hongshengwenyu.top

Go:   // 手写循环
来源：http://ojx.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pgd.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://epa.pengpengdd.cyou

[D24] 字典 / Map 基本操作
来源：http://vrb.ydzc1.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://phj.shangyingyoupin.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fyh.zhiwuduotai.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aka.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://esi.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tmr.jinghuilouyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zra.jinghuilouyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zvh.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pca.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://uns.cheryme.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xtq.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rij.yueranfly.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rls.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qhb.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xta.svipenyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sjf.xziqi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uwk.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vdg.sxryk.cn

[D26] 数组转字符串
来源：http://cln.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://jmo.ivvv.top

PHP:  implode(", ", $arr);
来源：http://rgd.zhengqikj.top

JS:   arr.join(", ")
来源：http://isp.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://iqv.bbcook.cn

Java: String.join(", ", list)
来源：http://lhk.tianlin.xyz

Go:   strings.Join(strs, ", ")
来源：http://ngs.fzhhl.top

Ruby: arr.join(", ")
来源：http://wfu.ctjpmb.com

C#:   string.Join(", ", list)
来源：http://qrj.xingfuxueyuan.xyz

================================================================================
来源：http://iby.ybcxt.top

E. 字符串处理
来源：http://imm.snrcjt.cn

================================================================================
来源：http://kan.kuanghao11.cn

[E01] 拼接字符串
来源：http://njb.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nyx.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xuh.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bym.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fdl.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dvi.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://txq.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jvj.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yhq.havefunace.top

[E02] 重复字符串
来源：http://bsl.shuidangran.top

Py:   "ab" * 3
来源：http://pni.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://gjb.cdnleiting.top

JS:   "ab".repeat(3)
来源：http://qdl.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://uyh.chenzaomai.com

Java: "ab".repeat(3)
来源：http://mhb.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://kcw.zhoulong.xyz

Ruby: "ab" * 3
来源：http://quu.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cen.uphjek.com

[E03] 截取子串
来源：http://svr.nwbrower.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nqx.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rja.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mmn.cdnleiting.top

TS:   s.slice(1, 4)
来源：http://gki.yongpay.top

Java: s.substring(1, 4)
来源：http://zuh.smart0.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mls.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hys.shanyushiyangtech.top

C#:   s.Substring(1, 3)
来源：http://fzv.fehbvm.com

[E04] 查找子串位置
来源：http://lwx.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://izy.fktsv.cn

PHP:  strpos($s, "x");
来源：http://vpn.vqdsnc.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kvt.shuidangran.top

TS:   s.indexOf("x")
来源：http://hwx.wangdashe.top

Java: s.indexOf("x")
来源：http://gnu.pycfn.com

Go:   strings.Index(s, "x")
来源：http://pal.kuanghao11.cn

Ruby: s.index("x")
来源：http://jzm.sysykeji.top

C#:   s.IndexOf("x")
来源：http://yir.vehdjk.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://hsc.cdnleiting.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nha.ydzc1.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ulc.wangshuangyany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zee.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mfn.gzhubu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xmq.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sqr.fengsongda.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jcl.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yse.jyoumei.cn

[E06] 替换子串
来源：http://zwz.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oqf.hesvh.cn

PHP:  str_replace("a", "b", $s);
来源：http://erg.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kru.sysykeji.top

TS:   s.replaceAll("a", "b")
来源：http://meh.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qdv.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hsy.yuxming.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nuc.yuxming.cn

C#:   s.Replace("a", "b")
来源：http://snm.316326.xyz

[E07] 按分隔符拆分
来源：http://oay.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://maq.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tcn.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rih.hongshengwenyu.top

TS:   s.split(",")
来源：http://fey.feifeiyinyue.top

Java: s.split(",");  s.split("\\s+")
来源：http://bju.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ayi.shanyushiyangtech.top

Ruby: s.split(",");  s.split
来源：http://ifl.nanxuanxn.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tdm.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://woz.hfpthk.cn

Py:   ",".join(items)
来源：http://nms.hysaishi.cn

PHP:  implode(",", $items);
来源：http://nsb.jinqigfzy.top

JS:   items.join(",")
来源：http://kly.meibo888.top

TS:   items.join(",")
来源：http://mgg.gaohongyu789.top

Java: String.join(",", items)
来源：http://uap.ppjwa.cn

Go:   strings.Join(items, ",")
来源：http://icb.c1oappe.top

Ruby: items.join(",")
来源：http://twg.fehbvm.com

C#:   string.Join(",", items)
来源：http://pej.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://ybl.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fut.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://loz.jyoumei.cn

JS:   s.replace(/\s+/g, "")
来源：http://bde.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://lsv.zhiwuduotai.top

Java: s.replaceAll("\\s+", "")
来源：http://kir.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ocl.zhiwuduotai.top

Ruby: s.gsub(/\s+/, "")
来源：http://cqp.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rph.yongpay.top

[E10] 左侧补零 / 定长填充
来源：http://uxt.tarul.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://svr.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hgn.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://mta.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://kuh.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://msv.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yhh.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kph.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hro.pycfn.com

[E11] 反转字符串
来源：http://fdb.sweek.top

Py:   s[::-1]
来源：http://pzr.yueranfly.top

PHP:  strrev($s);
来源：http://wvv.yanxiufei.cn

JS:   [...s].reverse().join("")
来源：http://lun.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://qqs.fanxiaobao.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://hop.shanyushiyangtech.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fwn.sufxvd.cn

Ruby: s.reverse
来源：http://ljf.zycfv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fpo.yj202588.top

[E12] 统计某字符出现次数
来源：http://iea.yangfankeji.com

Py:   s.count("a")
来源：http://ums.tanke756.top

PHP:  substr_count($s, "a");
来源：http://crs.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://fzp.hongshengwenyu.top

TS:   s.split("a").length - 1
来源：http://gtj.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aur.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://qff.zdqjudy.top

Ruby: s.count("a")
来源：http://vwm.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://mbl.0kj1m.cn

[E13] 逐字符遍历
来源：http://ovl.dashuyun.cn

Py:   for ch in s: print(ch)
来源：http://kwz.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dns.dianchejie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lcs.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ecc.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bsg.ctjpmb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xsv.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jfk.tianlin.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rfc.wangdashe.top

[E14] URL 编码与 Base64
来源：http://nme.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bup.yuxming.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://aqv.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jfz.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fhc.yonumen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://phx.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uzj.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://skx.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jug.zhengqikj.top

[E15] HTML 转义 / 反转义
来源：http://yli.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ubl.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://inj.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xec.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pdp.zhongyouzk.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://icb.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qsq.ivvv.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://onf.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ujc.tanke756.top

[E16] 数字千分位
来源：http://hio.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://eex.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://pqa.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cri.xingfuxueyuan.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://lwv.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lqw.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ijj.tianlin.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xnw.ydjk.org.cn

C#:   1234567.ToString("N0")
来源：http://ycq.c1oappe.top

[E17] 首字母大写
来源：http://ypt.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bkj.vehdjk.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://kij.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mqj.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://car.daxiang520.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://thp.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hjy.cqqwz.cn

Ruby: s.capitalize
来源：http://pza.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jaf.svipenyu.cn

[E18] 模板占位符替换
来源：http://tnk.chenzaomai.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://snw.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lvf.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yfi.chenlongwang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jre.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dxh.jqgfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jxj.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ydk.jqgfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wlq.daxiang520.top

[E19] 多行文本按行拆分
来源：http://ert.svipenyu.cn

Py:   s.splitlines()
来源：http://rpk.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fzl.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://smf.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://tdj.zhiwuduotai.top

Java: s.lines().toList()
来源：http://zsw.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://xna.ydzc1.top

Ruby: s.lines
来源：http://hzh.zhoulong.xyz

C#:   s.Split('\n')
来源：http://vxe.shanyushiyangtech.top

[E20] 判断字符串是否为空
来源：http://qjm.zhaomingkeji.xyz

Py:   if not s:
来源：http://hyg.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ffh.jqgfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wrk.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://ipq.fktsv.cn

Java: if (s.isEmpty()) {}
来源：http://gsy.vqdsnc.cn

Go:   if s == "" {}
来源：http://cpz.sufxvd.cn

Ruby: if s.empty?
来源：http://rxb.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tji.yj20258.top

[E21] 超长截断加省略号
来源：http://ohg.sxryk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vtc.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cki.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jvq.sjlbkw.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qbd.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kbi.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://uwr.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kne.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://utq.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://ffa.kuanghao11.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oaw.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://anj.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hga.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://abb.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kmh.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qif.xuetiantiany.cn

Ruby: s.bytesize;  s.length
来源：http://cpy.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://got.zhaomingkeji.xyz

================================================================================
来源：http://cmw.xylfe.cn

F. 文件与目录
来源：http://pmd.jlsjyb.cn

================================================================================
来源：http://url.sxryk.cn

[F01] 读取整个文件
来源：http://fsk.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jmh.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://tki.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gez.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hls.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lyf.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://een.yj202588.top

Ruby: File.read("a.txt")
来源：http://yoe.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://dqa.ivvv.top

[F02] 逐行读取文件
来源：http://hzb.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aqo.shanyushiyangtech.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jgt.nanxinkj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vxe.chenjidiqi.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uef.ydjk.org.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mhg.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://drw.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ihh.c1oappe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ehu.yfazqb.com

[F03] 写入文件（覆盖）
来源：http://lwd.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tdq.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ogr.jinyuanbaomall.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ick.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vms.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gqt.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kmh.hcnkem.com

Ruby: File.write("a.txt", "hi")
来源：http://vwv.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hib.yuxming.cn

[F04] 追加写入文件
来源：http://ksv.xziqi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hzm.birdmap.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dut.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pot.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mkm.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dum.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cdt.shanyushiyangtech.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baq.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kmi.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://fgj.vehdjk.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iya.shanyushiyangkeji.top

PHP:  file_exists("a.txt");
来源：http://agy.yfazqb.com

JS:   fs.existsSync("a.txt")
来源：http://jlh.hysaishi.cn

TS:   fs.existsSync("a.txt")
来源：http://dxr.iojbl.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zrp.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vag.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://oly.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://zgv.ywan-chungtsiang.top

[F06] 删除文件
来源：http://nyq.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://xfi.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://huy.daxiang520.top


<!-- 参考信息 -->