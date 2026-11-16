代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://jxj.hywenlv.cn

Ruby: arr.include?(x)
来源：http://lra.xziqi.cn

C#:   list.Contains(x)
来源：http://zhm.svipenyu.cn

[D22] 复制数组（避免共享引用）
来源：http://vyc.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zvt.svipenyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kgi.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rxq.yj20258.top

TS:   [...arr];
来源：http://cje.fzhhl.top

Java: new ArrayList<>(list);
来源：http://hni.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://sam.dashuyun.cn

Ruby: arr.dup;  arr.clone
来源：http://kxl.yongpay.top

C#:   new List<int>(list);
来源：http://saj.cashguo.top

[D23] reduce 累积计算
来源：http://lzx.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jmv.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yps.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qxg.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uvx.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://aii.yanxiufei.cn

Go:   // 手写循环
来源：http://wqg.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aqa.hongshengwenyu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nom.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://odw.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://prq.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pgh.shangyingyoupin.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ula.guannengcc.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://war.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tgl.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lmu.52xcode.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jmj.zhixingplan.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cje.zhongyouzk.top

[D25] Set 集合去重与交并差
来源：http://gaz.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xuw.quarkkingdee.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hky.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gsz.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lma.quarkkingdee.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hyb.fehbvm.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gph.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wti.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cfr.vehdjk.com

[D26] 数组转字符串
来源：http://sqo.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://ogn.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://brs.xuetiantiany.cn

JS:   arr.join(", ")
来源：http://jxd.xinyue.icu

TS:   arr.join(", ")
来源：http://esd.nanxuanxn.top

Java: String.join(", ", list)
来源：http://duw.uphjek.com

Go:   strings.Join(strs, ", ")
来源：http://xdh.fzhhl.top

Ruby: arr.join(", ")
来源：http://ptv.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://cev.yonumen.top

================================================================================
来源：http://xso.sxryk.cn

E. 字符串处理
来源：http://ywn.ctjpmb.com

================================================================================
来源：http://akk.tarul.cn

[E01] 拼接字符串
来源：http://rah.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uet.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gos.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xjq.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fhc.hywenlv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qif.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rbx.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vkk.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oog.hongshengwenyu.top

[E02] 重复字符串
来源：http://kwv.chenjidiqi.icu

Py:   "ab" * 3
来源：http://man.jyoumei.cn

PHP:  str_repeat("ab", 3);
来源：http://gbk.aizwys.cn

JS:   "ab".repeat(3)
来源：http://alb.sysykeji.top

TS:   "ab".repeat(3)
来源：http://sui.dianchejie.cn

Java: "ab".repeat(3)
来源：http://gmr.svipenyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://ryj.ehwqpu.com

Ruby: "ab" * 3
来源：http://gmo.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wwq.zhiwuduotai.top

[E03] 截取子串
来源：http://rff.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ctv.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pap.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dhe.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://rtl.ivvv.top

Java: s.substring(1, 4)
来源：http://epr.0kj1m.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://shd.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://hlb.yueranfly.top

C#:   s.Substring(1, 3)
来源：http://ndj.sxryk.cn

[E04] 查找子串位置
来源：http://nxs.jinqigufen.top

Py:   s.find("x");  s.index("x")
来源：http://ecn.hnqzz.top

PHP:  strpos($s, "x");
来源：http://jpo.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://haz.ctjpmb.com

TS:   s.indexOf("x")
来源：http://ike.smart0.xyz

Java: s.indexOf("x")
来源：http://fvy.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://ril.vehdjk.com

Ruby: s.index("x")
来源：http://yuw.tian-w.cn

C#:   s.IndexOf("x")
来源：http://eoo.sufxvd.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jna.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ejz.52xcode.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qdi.tanke756.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wvn.dashuyun.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://quz.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bto.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ffk.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bzg.hcnkem.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://esw.bbcook.cn

[E06] 替换子串
来源：http://xsa.zhijiandao.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jmn.zhongyouzk.top

PHP:  str_replace("a", "b", $s);
来源：http://skt.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vmu.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://hmz.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aik.jiagoushi.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xcv.xylfe.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ygf.316326.xyz

C#:   s.Replace("a", "b")
来源：http://sin.sufxvd.cn

[E07] 按分隔符拆分
来源：http://mky.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uaj.hesvh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fgw.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bfq.cdnleiting.top

TS:   s.split(",")
来源：http://bwo.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://dfv.aizwys.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://byl.redwolf501.top

Ruby: s.split(",");  s.split
来源：http://udk.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ssx.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://mtp.jlsjyb.cn

Py:   ",".join(items)
来源：http://xbu.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://cgg.tanke756.top

JS:   items.join(",")
来源：http://lvw.yfazqb.com

TS:   items.join(",")
来源：http://htc.ppjwa.cn

Java: String.join(",", items)
来源：http://tsc.ppjwa.cn

Go:   strings.Join(items, ",")
来源：http://trv.xingfuxueyuan.xyz

Ruby: items.join(",")
来源：http://srq.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://nqe.0kj1m.cn

[E09] 去除所有空白字符
来源：http://ucm.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qqd.jinghuilouyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fwu.xuetiantiany.cn

JS:   s.replace(/\s+/g, "")
来源：http://nul.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://mqo.wangdashe.top

Java: s.replaceAll("\\s+", "")
来源：http://wbm.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://guc.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://eqr.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rrj.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://knw.nwbrower.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ieg.andypj.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yfu.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://hkg.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://uzu.cashguo.top

Java: String.format("%03d", 7)
来源：http://gzr.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rhh.ctjpmb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gcs.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://raq.shzxlz.cn

[E11] 反转字符串
来源：http://bak.nwbrower.top

Py:   s[::-1]
来源：http://ugp.sjlbkw.cn

PHP:  strrev($s);
来源：http://foe.sjlbkw.cn

JS:   [...s].reverse().join("")
来源：http://lrh.fehbvm.com

TS:   [...s].reverse().join("")
来源：http://ipf.xuanzx.com

Java: new StringBuilder(s).reverse().toString()
来源：http://xhd.jinqigfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ixh.yuanzhike.top

Ruby: s.reverse
来源：http://vpr.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://bns.cashguo.top

[E12] 统计某字符出现次数
来源：http://czj.cdnleiting.top

Py:   s.count("a")
来源：http://ata.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://laa.cheryme.top

JS:   s.split("a").length - 1
来源：http://znd.xuanzx.com

TS:   s.split("a").length - 1
来源：http://fpf.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tvs.hywenlv.cn

Go:   strings.Count(s, "a")
来源：http://kog.tian-w.cn

Ruby: s.count("a")
来源：http://utk.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://sow.zdqjudy.top

[E13] 逐字符遍历
来源：http://jzn.shanyushiyangtech.top

Py:   for ch in s: print(ch)
来源：http://rbr.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tjy.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://wno.zhongyouzk.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bzc.vqdsnc.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qun.ywan-chungtsiang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lbv.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hkq.zhixingplan.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pnb.yangfankeji.com

[E14] URL 编码与 Base64
来源：http://ict.hfpthk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://crh.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hfv.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://caa.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zbz.zdqjudy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://huv.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dsv.yvedp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aau.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wqe.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://qgn.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://iox.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iqz.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xfr.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qdn.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ycw.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hbe.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gqt.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lqs.yuanzhike.top

[E16] 数字千分位
来源：http://xgt.hysaishi.cn

Py:   f"{1234567:,}"
来源：http://ihk.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://zaa.xylfe.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pnv.zhiwuduotai.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hpu.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pua.xuanzx.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jge.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ssy.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://meb.epnwcf.com

[E17] 首字母大写
来源：http://sbw.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rfy.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bfy.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://htw.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qvb.sjlbkw.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://itg.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nro.cashguo.top

Ruby: s.capitalize
来源：http://rnq.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pvm.jinghuilouyu.cn

[E18] 模板占位符替换
来源：http://ocd.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fir.sufxvd.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mck.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://idu.ctjpmb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://hnl.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kbm.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ymd.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://czl.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ybe.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://fye.iojbl.cn

Py:   s.splitlines()
来源：http://cln.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uvl.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://qcl.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://vvh.chenjidiqi.icu

Java: s.lines().toList()
来源：http://vul.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://cqv.shzxlz.cn

Ruby: s.lines
来源：http://etv.sweek.top

C#:   s.Split('\n')
来源：http://txu.vehdjk.com

[E20] 判断字符串是否为空
来源：http://ekg.vehdjk.com

Py:   if not s:
来源：http://cfj.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mjc.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kpd.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://wxx.aibaodan.cn

Java: if (s.isEmpty()) {}
来源：http://pjf.cdnleiting.top

Go:   if s == "" {}
来源：http://ynk.pycfn.com

Ruby: if s.empty?
来源：http://gyr.xinyue.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://otm.andypj.xyz

[E21] 超长截断加省略号
来源：http://amx.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lmk.xingfuxueyuan.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dnp.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://emx.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pdk.ivvv.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://soa.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://ybs.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eic.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://umc.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://yat.jqgfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qip.zhaomingkeji.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kbz.shanyushiyangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://erg.c1oappe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ann.epnwcf.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bvm.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gza.epnwcf.com

Ruby: s.bytesize;  s.length
来源：http://jqn.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ism.quarkkingdee.top

================================================================================
来源：http://pco.52xcode.cn

F. 文件与目录
来源：http://egg.jianghu66.top

================================================================================
来源：http://kfl.hywenlv.cn

[F01] 读取整个文件
来源：http://gev.ydzc1.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cyq.jqgfzy.top

PHP:  file_get_contents("a.txt");
来源：http://ufy.shangyingyoupin.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fom.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bcq.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zcs.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nvn.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://zrf.hywenlv.cn

C#:   File.ReadAllText("a.txt");
来源：http://hky.c1oappe.top

[F02] 逐行读取文件
来源：http://yxp.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wyv.nanxinkj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ucl.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vbx.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oiv.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://luw.meibo888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fds.hcnkem.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://twq.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wzb.zycfv.cn

[F03] 写入文件（覆盖）
来源：http://gby.bbcook.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kkn.bbcook.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://olf.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ljq.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zft.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zdv.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oyr.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://bie.ywan-chungtsiang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uop.havefunace.top

[F04] 追加写入文件
来源：http://rvd.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pyj.yueranfly.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://phx.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ads.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mny.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pia.hongshengwenyu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bnc.snrcjt.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tol.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://amh.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://nnp.shuidangran.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rjm.hfpthk.cn

PHP:  file_exists("a.txt");
来源：http://ycp.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://wyq.jqgufenzy.top

TS:   fs.existsSync("a.txt")
来源：http://fxi.haohaochexian.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vzx.shanyushiyangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://clc.hywenlv.cn

Ruby: File.exist?("a.txt")
来源：http://kpd.daria6918.cn

C#:   File.Exists("a.txt")
来源：http://qcd.yueranfly.top

[F06] 删除文件
来源：http://ftj.zdqjudy.top

Py:   os.remove("a.txt")
来源：http://dme.cashguo.top

PHP:  unlink("a.txt");
来源：http://zse.nanxinkj.top


<!-- 参考信息 -->