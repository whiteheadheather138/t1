代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://htl.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gjt.fehbvm.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bnk.zhiwuduotai.top

TS:   [...arr];
来源：http://mua.fktsv.cn

Java: new ArrayList<>(list);
来源：http://ipb.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://ijz.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://sjp.dianchejie.cn

C#:   new List<int>(list);
来源：http://dng.dianchejie.cn

[D23] reduce 累积计算
来源：http://zee.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zsy.yvedp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lnw.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kre.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pwa.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cdy.chenzaomai.com

Go:   // 手写循环
来源：http://fdm.yanxiufei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dza.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dcy.smart0.xyz

[D24] 字典 / Map 基本操作
来源：http://hyp.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pyd.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lzv.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cgu.andypj.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nik.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xrv.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mwo.jinqigfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dpo.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xcr.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://lgr.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://czn.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ktl.zycfv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zll.sxryk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dxi.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nyz.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yps.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vjz.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hlo.vqdsnc.cn

[D26] 数组转字符串
来源：http://jhr.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://yns.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://zmc.tianlin.xyz

JS:   arr.join(", ")
来源：http://uar.zdbjq.cn

TS:   arr.join(", ")
来源：http://nnn.vehdjk.com

Java: String.join(", ", list)
来源：http://mpd.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://lnw.haohaochexian.top

Ruby: arr.join(", ")
来源：http://wbh.bbcook.cn

C#:   string.Join(", ", list)
来源：http://unx.bjfxy.top

================================================================================
来源：http://mhz.zhijiandao.cn

E. 字符串处理
来源：http://anc.cheryme.top

================================================================================
来源：http://sgq.cheryme.top

[E01] 拼接字符串
来源：http://lif.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://axj.aizwys.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cec.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://evw.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wdq.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ont.tanke756.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qgm.sysykeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lmt.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dmt.fehbvm.com

[E02] 重复字符串
来源：http://aqa.fengsongda.top

Py:   "ab" * 3
来源：http://vnp.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://tpd.hcnkem.com

JS:   "ab".repeat(3)
来源：http://pve.hcnkem.com

TS:   "ab".repeat(3)
来源：http://gkh.chenzaomai.com

Java: "ab".repeat(3)
来源：http://jgh.snrcjt.cn

Go:   strings.Repeat("ab", 3)
来源：http://rgo.fktsv.cn

Ruby: "ab" * 3
来源：http://dty.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://okv.dianchejie.cn

[E03] 截取子串
来源：http://tjq.ctjpmb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dlx.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xyx.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zxw.uphjek.com

TS:   s.slice(1, 4)
来源：http://rcz.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://kwm.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://asr.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://suv.sjlbkw.cn

C#:   s.Substring(1, 3)
来源：http://xgq.hesvh.cn

[E04] 查找子串位置
来源：http://wrj.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://htc.dashuyun.cn

PHP:  strpos($s, "x");
来源：http://lgx.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jxf.zhaomingkeji.xyz

TS:   s.indexOf("x")
来源：http://guz.zhongyouzk.top

Java: s.indexOf("x")
来源：http://xxi.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://wzs.fktsv.cn

Ruby: s.index("x")
来源：http://nec.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://pfz.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://spq.jqgufenzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hmd.gaohongyu789.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wmq.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://boz.redwolf501.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uaa.bbcook.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.andypj.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sdy.wangshuangyany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ydv.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jov.quarkkingdee.top

[E06] 替换子串
来源：http://num.hnqzz.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wsb.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://ikk.kuanghao11.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yep.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://gbg.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cmm.feifeiyinyue.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kpn.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dim.fehbvm.com

C#:   s.Replace("a", "b")
来源：http://ubn.fktsv.cn

[E07] 按分隔符拆分
来源：http://spa.quarkkingdee.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xuo.wangshuangyany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dyx.aizwys.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pdm.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://xkn.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hmw.yj202588.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rcj.sweek.top

Ruby: s.split(",");  s.split
来源：http://rak.xziqi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mot.chenlongwang.top

[E08] 数组按分隔符合并
来源：http://juo.c1oappe.top

Py:   ",".join(items)
来源：http://ckq.jinghuilouyu.cn

PHP:  implode(",", $items);
来源：http://paf.jyoumei.cn

JS:   items.join(",")
来源：http://zjk.tarul.cn

TS:   items.join(",")
来源：http://fsr.hywenlv.cn

Java: String.join(",", items)
来源：http://pou.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://sjz.zhiwuduotai.top

Ruby: items.join(",")
来源：http://bfb.pengpengdd.cyou

C#:   string.Join(",", items)
来源：http://rwb.dianchejie.cn

[E09] 去除所有空白字符
来源：http://xoh.zhengqikj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nwt.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ako.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://zyn.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://wxw.havefunace.top

Java: s.replaceAll("\\s+", "")
来源：http://kqo.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://rab.vqdsnc.cn

Ruby: s.gsub(/\s+/, "")
来源：http://iyy.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://knm.daria6918.cn

[E10] 左侧补零 / 定长填充
来源：http://syg.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qgo.quarkkingdee.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://abx.shanyushiyangtech.top

JS:   "7".padStart(3, "0")
来源：http://yzq.jinqigfzy.top

TS:   "7".padStart(3, "0")
来源：http://bwl.nanxuanxn.top

Java: String.format("%03d", 7)
来源：http://dvq.fanxiaobao.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://hzw.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uzi.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gva.c1oappe.top

[E11] 反转字符串
来源：http://dcr.daria6918.cn

Py:   s[::-1]
来源：http://ktp.sweek.top

PHP:  strrev($s);
来源：http://efh.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://fjq.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://cqj.0kj1m.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ufh.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vmo.xuetiantiany.cn

Ruby: s.reverse
来源：http://ymn.fktsv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fvs.pycfn.com

[E12] 统计某字符出现次数
来源：http://jrh.sjlbkw.cn

Py:   s.count("a")
来源：http://iyf.dianchejie.cn

PHP:  substr_count($s, "a");
来源：http://gis.cdnleiting.top

JS:   s.split("a").length - 1
来源：http://rql.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://zcp.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lrd.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://uqi.52xcode.cn

Ruby: s.count("a")
来源：http://bfk.zhongyouzk.top

C#:   s.Count(c => c == 'a')
来源：http://jes.dianchejie.cn

[E13] 逐字符遍历
来源：http://wnf.meibo888.top

Py:   for ch in s: print(ch)
来源：http://nrv.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jpl.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://rxb.nanxinkj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://abk.yueranfly.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ewt.ybcxt.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://akh.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xjv.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nhz.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://jmt.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gbp.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://vyy.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mth.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://otf.cashguo.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mtb.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gir.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xws.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ttv.jinqigufen.top

[E15] HTML 转义 / 反转义
来源：http://ghh.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xaa.ivvv.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tkt.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qvs.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qce.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://owp.jinyuanbaomall.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://roq.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cqv.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yke.daria6918.cn

[E16] 数字千分位
来源：http://jfz.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://vnq.c1oappe.top

PHP:  number_format(1234567);
来源：http://rtn.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tct.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://dsx.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wyd.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zjq.52xcode.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://abh.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://qru.jinqigufen.top

[E17] 首字母大写
来源：http://ooq.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zbj.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://kkj.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cev.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://epm.yvedp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wgx.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ckz.cdnleiting.top

Ruby: s.capitalize
来源：http://tqx.xuetiantiany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://glj.xinyue.icu

[E18] 模板占位符替换
来源：http://dok.tanke756.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lcj.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mwq.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kmx.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://dnk.nanxuanxn.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zhv.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yjd.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wle.uphjek.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tof.daxiang520.top

[E19] 多行文本按行拆分
来源：http://pvi.kuanghao11.cn

Py:   s.splitlines()
来源：http://zdi.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ple.smart0.xyz

JS:   s.split(/\r?\n/)
来源：http://oed.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://jaf.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://okl.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://gqg.hywenlv.cn

Ruby: s.lines
来源：http://ysr.aibaodan.cn

C#:   s.Split('\n')
来源：http://jqp.zhongyouzk.top

[E20] 判断字符串是否为空
来源：http://klb.jiagoushi.top

Py:   if not s:
来源：http://wjl.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oas.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bxu.yj20258888.top

TS:   if (s === "") {}
来源：http://aez.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://bmk.vqdsnc.cn

Go:   if s == "" {}
来源：http://rso.uphjek.com

Ruby: if s.empty?
来源：http://lmy.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xsf.ppjwa.cn

[E21] 超长截断加省略号
来源：http://vcy.zhengqikj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aif.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pye.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jie.fzhhl.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dem.hcnkem.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://whn.epnwcf.com

Go:   // 按 rune 判断长度后截断
来源：http://ogw.yanxiufei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lgw.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jdz.mhx1999.top

[E22] 字节长度与字符长度
来源：http://ahp.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tpu.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gca.vqdsnc.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ktq.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xxy.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jqd.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ifp.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://yth.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wuy.uphjek.com

================================================================================
来源：http://xxq.fanxiaobao.xyz

F. 文件与目录
来源：http://zfp.xingfuxueyuan.xyz

================================================================================
来源：http://tba.cqqwz.cn

[F01] 读取整个文件
来源：http://kgi.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zay.yanxiufei.cn

PHP:  file_get_contents("a.txt");
来源：http://ltb.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zxb.yj20258888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sxy.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vri.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wcd.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://cir.yonumen.top

C#:   File.ReadAllText("a.txt");
来源：http://okx.xuetiantiany.cn

[F02] 逐行读取文件
来源：http://izw.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oru.fengsongda.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bvc.ehwqpu.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ami.jianghu66.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://psk.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pju.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://puc.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ant.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kxh.ivvv.top

[F03] 写入文件（覆盖）
来源：http://zcg.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qfi.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dhy.wangdashe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vem.ybcxt.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://opv.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rfn.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dqx.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://mdq.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vrf.vehdjk.com

[F04] 追加写入文件
来源：http://zzx.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dfw.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://llw.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pok.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dzs.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ycb.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zdn.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://awd.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://csd.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://nee.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tsx.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://kgc.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://uft.zdqjudy.top

TS:   fs.existsSync("a.txt")
来源：http://ewf.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gus.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sqr.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://dwj.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://wlu.cucudq.cn

[F06] 删除文件
来源：http://tcn.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://thv.uphjek.com

PHP:  unlink("a.txt");
来源：http://run.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://tbu.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://aco.ctjpmb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gph.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://mrt.hnxiangtu.top


<!-- 参考信息 -->