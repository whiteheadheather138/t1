代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hwp.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zlk.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://juu.zycfv.cn

TS:   [...arr];
来源：http://tro.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://zwk.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://dgo.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://cmg.zhiwuduotai.top

C#:   new List<int>(list);
来源：http://lnt.havefunace.top

[D23] reduce 累积计算
来源：http://yru.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dwt.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://itd.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ajt.sweek.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nmd.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vjd.ehwqpu.com

Go:   // 手写循环
来源：http://npj.quarkkingdee.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://znh.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://epy.dashuyun.cn

[D24] 字典 / Map 基本操作
来源：http://upi.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dyp.nanxuanxn.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vyj.ivvv.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rdx.hongshengwenyu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pue.chenzaomai.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mfj.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dzz.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rox.cheryme.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pnm.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://mfa.9152youxi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kwb.zhoulong.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zef.chenlongwang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vqt.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zsi.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pez.jinghuilouyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xrz.xingfuxueyuan.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zgq.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uef.ivvv.top

[D26] 数组转字符串
来源：http://pon.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://gwj.xinyue.icu

PHP:  implode(", ", $arr);
来源：http://vej.yuanzhike.top

JS:   arr.join(", ")
来源：http://ocb.snrcjt.cn

TS:   arr.join(", ")
来源：http://mea.sysykeji.top

Java: String.join(", ", list)
来源：http://awt.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://lfa.cashguo.top

Ruby: arr.join(", ")
来源：http://iqq.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://whq.feifeiyinyue.top

================================================================================
来源：http://psm.gogol.net.cn

E. 字符串处理
来源：http://oiq.vehdjk.com

================================================================================
来源：http://sez.havefunace.top

[E01] 拼接字符串
来源：http://srx.pycfn.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xcm.yvedp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yvb.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nbl.gaohongyu789.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://egn.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ysg.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vpp.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nyx.fktsv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qpp.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://cec.redwolf501.top

Py:   "ab" * 3
来源：http://imv.gzhubu.top

PHP:  str_repeat("ab", 3);
来源：http://ffa.pycfn.com

JS:   "ab".repeat(3)
来源：http://asq.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://djr.havefunace.top

Java: "ab".repeat(3)
来源：http://rlw.jinyuanbaomall.cn

Go:   strings.Repeat("ab", 3)
来源：http://lha.jinqigfzy.top

Ruby: "ab" * 3
来源：http://cad.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gwr.jinqigfzy.top

[E03] 截取子串
来源：http://rqh.0kj1m.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vef.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qhz.tanke756.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rzz.316326.xyz

TS:   s.slice(1, 4)
来源：http://irq.snrcjt.cn

Java: s.substring(1, 4)
来源：http://dzy.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gww.jyoumei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lea.xuanzx.com

C#:   s.Substring(1, 3)
来源：http://bcl.sxryk.cn

[E04] 查找子串位置
来源：http://pts.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://cuz.yj20258888.top

PHP:  strpos($s, "x");
来源：http://fdf.zdqjudy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hdc.sysykeji.top

TS:   s.indexOf("x")
来源：http://kra.9152youxi.cn

Java: s.indexOf("x")
来源：http://ipt.dianchejie.cn

Go:   strings.Index(s, "x")
来源：http://khm.xylfe.cn

Ruby: s.index("x")
来源：http://bgz.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://uhw.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rvz.xuanzx.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://avi.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sza.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://abr.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oti.vehdjk.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lur.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xlq.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kpg.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uio.epnwcf.com

[E06] 替换子串
来源：http://fwq.fzhhl.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zzs.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://lvr.ctjpmb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qpb.jqgufenzy.top

TS:   s.replaceAll("a", "b")
来源：http://hbr.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ehe.hnqzz.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bdn.yj20258888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zht.gaohongyu789.top

C#:   s.Replace("a", "b")
来源：http://xkx.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://vij.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mdv.wangdashe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zte.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mcl.zhoulong.xyz

TS:   s.split(",")
来源：http://qnj.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://slw.fehbvm.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wot.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://nzy.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jmm.hnqzz.top

[E08] 数组按分隔符合并
来源：http://xsp.bjfxy.top

Py:   ",".join(items)
来源：http://cdx.ctjpmb.com

PHP:  implode(",", $items);
来源：http://opk.zhiwuduotai.top

JS:   items.join(",")
来源：http://giw.yanxiufei.cn

TS:   items.join(",")
来源：http://biz.ydjk.org.cn

Java: String.join(",", items)
来源：http://kzl.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://gxw.tanke756.top

Ruby: items.join(",")
来源：http://sxr.hammf.cn

C#:   string.Join(",", items)
来源：http://cvb.smart0.xyz

[E09] 去除所有空白字符
来源：http://tqv.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://guk.hfpthk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://flo.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://lsa.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://ldi.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://uox.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://gud.vqdsnc.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xpj.c1oappe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lyh.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://luk.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lbv.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ftp.ybcxt.top

JS:   "7".padStart(3, "0")
来源：http://jlp.shanyushiyangkeji.top

TS:   "7".padStart(3, "0")
来源：http://kfz.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://avn.jianghu66.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://uzq.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uhr.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jna.yuxming.cn

[E11] 反转字符串
来源：http://pvq.gaohongyu789.top

Py:   s[::-1]
来源：http://ueh.iojbl.cn

PHP:  strrev($s);
来源：http://jzf.feifeiyinyue.top

JS:   [...s].reverse().join("")
来源：http://qix.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://kxl.yuanzhike.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ack.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://onv.xuetiantiany.cn

Ruby: s.reverse
来源：http://hwo.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://qrn.wangdashe.top

[E12] 统计某字符出现次数
来源：http://vlv.xuetiantiany.cn

Py:   s.count("a")
来源：http://luj.ivvv.top

PHP:  substr_count($s, "a");
来源：http://fke.zhengqikj.top

JS:   s.split("a").length - 1
来源：http://ktg.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://dkn.ctjpmb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ksx.uphjek.com

Go:   strings.Count(s, "a")
来源：http://wnn.yueranfly.top

Ruby: s.count("a")
来源：http://afx.ivvv.top

C#:   s.Count(c => c == 'a')
来源：http://ebl.fzhhl.top

[E13] 逐字符遍历
来源：http://ssa.yj202588.top

Py:   for ch in s: print(ch)
来源：http://fvx.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ztb.guowangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cvc.hongshengwenyu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://unk.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gsp.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gaz.hywenlv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uhu.cqqwz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zos.sxryk.cn

[E14] URL 编码与 Base64
来源：http://ojl.sysykeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vno.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xde.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dsl.yvedp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vug.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xlm.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hix.gotoacloud.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nqt.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jdb.hywenlv.cn

[E15] HTML 转义 / 反转义
来源：http://mnm.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://nno.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uot.zhijiandao.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bea.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://bex.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qwd.guowangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gga.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qkb.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lhs.pengpengdd.cyou

[E16] 数字千分位
来源：http://zqh.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://hsz.gotoacloud.top

PHP:  number_format(1234567);
来源：http://axz.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://mnw.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ozw.shangyingyoupin.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ywz.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nsg.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dnj.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://ujr.chenlongwang.top

[E17] 首字母大写
来源：http://nsw.cdnleiting.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vpg.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nox.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lfc.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xvb.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iht.xingfuxueyuan.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uun.vehdjk.com

Ruby: s.capitalize
来源：http://ybe.ppjwa.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cxh.vqdsnc.cn

[E18] 模板占位符替换
来源：http://szv.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gyb.xuetiantiany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sze.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://qfb.ydjk.org.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tcn.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ote.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jtx.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://huf.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kuj.andypj.xyz

[E19] 多行文本按行拆分
来源：http://psw.havefunace.top

Py:   s.splitlines()
来源：http://eiv.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tgs.fzhhl.top

JS:   s.split(/\r?\n/)
来源：http://mqn.tian-w.cn

TS:   s.split(/\r?\n/)
来源：http://jcd.yueranfly.top

Java: s.lines().toList()
来源：http://vzd.sweek.top

Go:   strings.Split(s, "\n")
来源：http://ljk.fehbvm.com

Ruby: s.lines
来源：http://mqs.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://skp.snrcjt.cn

[E20] 判断字符串是否为空
来源：http://snd.birdmap.top

Py:   if not s:
来源：http://oeu.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gmk.hongshengwenyu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fpt.xinyue.icu

TS:   if (s === "") {}
来源：http://ijj.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://fqq.aibaodan.cn

Go:   if s == "" {}
来源：http://zvb.havefunace.top

Ruby: if s.empty?
来源：http://qon.iojbl.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dhe.bbcook.cn

[E21] 超长截断加省略号
来源：http://ztm.zhengqikj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ohd.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jwa.hnqzz.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jcj.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qvl.hongshengwenyu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vvy.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://qzl.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ytr.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mrk.meibo888.top

[E22] 字节长度与字符长度
来源：http://wwt.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xxi.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zdb.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vhk.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sjw.yuanzhike.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tac.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ara.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://etm.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wzj.zdqjudy.top

================================================================================
来源：http://xca.snrcjt.cn

F. 文件与目录
来源：http://jgd.fehbvm.com

================================================================================
来源：http://zeo.guannengcc.top

[F01] 读取整个文件
来源：http://kia.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gbg.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://zav.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yro.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://muu.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bjd.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rud.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://lis.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://qty.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://etm.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dwx.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ppe.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://edb.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rps.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dft.yuanzhike.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://scl.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jem.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://juy.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://udx.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://loe.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://obp.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://efm.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jyt.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vxh.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://drg.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://zqp.zhijiandao.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://npy.svipenyu.cn

[F04] 追加写入文件
来源：http://msh.cdnleiting.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ncj.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://obr.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fui.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lwb.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xii.wangdashe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dds.smart0.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ddg.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://emi.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://ocj.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://arq.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://rkw.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://svh.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://vvl.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://pix.ydzc1.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pgo.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://qvr.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://ouz.jinqigufen.top

[F06] 删除文件
来源：http://pge.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://hvg.fehbvm.com

PHP:  unlink("a.txt");
来源：http://aks.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://yfe.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://jsi.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xri.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://rdf.vehdjk.com


<!-- 参考信息 -->