代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sjl.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uiv.tarul.cn

Go:   // 手写循环
来源：http://dpj.jinyuanbaomall.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zxy.gaohongyu789.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pge.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://pxd.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://usb.ydjk.org.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qei.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kmk.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://thr.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lut.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ivc.yj20258.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://caz.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gjn.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://xiq.yueranfly.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jbd.hongshengwenyu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mjl.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bxp.zhaomingkeji.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yil.yj20258.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gni.fanxiaobao.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gkd.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jfz.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://odc.havefunace.top

[D26] 数组转字符串
来源：http://ybe.jyoumei.cn

Py:   ", ".join(map(str, arr))
来源：http://izx.yj20258888.top

PHP:  implode(", ", $arr);
来源：http://pnn.yj20258888.top

JS:   arr.join(", ")
来源：http://wor.bjfxy.top

TS:   arr.join(", ")
来源：http://ddm.kuanghao11.cn

Java: String.join(", ", list)
来源：http://mty.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://wjl.gotoacloud.top

Ruby: arr.join(", ")
来源：http://vbp.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://ady.snrcjt.cn

================================================================================
来源：http://dmd.fehbvm.com

E. 字符串处理
来源：http://mmn.hongshengwenyu.top

================================================================================
来源：http://oen.guowangkeji.top

[E01] 拼接字符串
来源：http://liu.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kar.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gvd.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ohf.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://thd.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fuw.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kvi.sweek.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hww.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ikm.epnwcf.com

[E02] 重复字符串
来源：http://kbu.meibo888.top

Py:   "ab" * 3
来源：http://nsj.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://ptq.cucudq.cn

JS:   "ab".repeat(3)
来源：http://xcj.nanxinkj.top

TS:   "ab".repeat(3)
来源：http://ise.hysaishi.cn

Java: "ab".repeat(3)
来源：http://ldo.smart0.xyz

Go:   strings.Repeat("ab", 3)
来源：http://dwv.fengsongda.top

Ruby: "ab" * 3
来源：http://wyr.jqgufenzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eqa.yj202588.top

[E03] 截取子串
来源：http://dlo.birdmap.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qtb.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nbg.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eir.yuxming.cn

TS:   s.slice(1, 4)
来源：http://dkg.jiagoushi.top

Java: s.substring(1, 4)
来源：http://evo.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://osy.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://sgw.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://tkb.meibo888.top

[E04] 查找子串位置
来源：http://huo.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://wlm.sweek.top

PHP:  strpos($s, "x");
来源：http://lgo.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zsq.zhaomingkeji.xyz

TS:   s.indexOf("x")
来源：http://rch.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://sux.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://ggg.ydjk.org.cn

Ruby: s.index("x")
来源：http://uiz.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://frd.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mvd.ctjpmb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ads.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ged.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jsv.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://erd.fzhhl.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zle.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uth.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cvy.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oox.cashguo.top

[E06] 替换子串
来源：http://bnn.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ntq.nanxuanxn.top

PHP:  str_replace("a", "b", $s);
来源：http://uwx.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qrj.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://dxb.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://glp.epnwcf.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fpc.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://scm.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://yzz.zdbjq.cn

[E07] 按分隔符拆分
来源：http://ujb.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iar.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aen.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://mmz.jinyuanbaomall.cn

TS:   s.split(",")
来源：http://dip.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://bce.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vpp.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://vjz.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://huc.jlsjyb.cn

[E08] 数组按分隔符合并
来源：http://rja.cashguo.top

Py:   ",".join(items)
来源：http://grr.fanxiaobao.xyz

PHP:  implode(",", $items);
来源：http://lca.meibo888.top

JS:   items.join(",")
来源：http://tlo.jlsjyb.cn

TS:   items.join(",")
来源：http://unm.xingfuxueyuan.xyz

Java: String.join(",", items)
来源：http://tno.zhengqikj.top

Go:   strings.Join(items, ",")
来源：http://jrg.hcnkem.com

Ruby: items.join(",")
来源：http://zby.ctjpmb.com

C#:   string.Join(",", items)
来源：http://bgx.epnwcf.com

[E09] 去除所有空白字符
来源：http://wvv.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jtr.zdbjq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yfc.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://qaq.mhx1999.top

TS:   s.replace(/\s+/g, "")
来源：http://amr.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://wad.yvedp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://plp.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://wxn.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pnb.hcnkem.com

[E10] 左侧补零 / 定长填充
来源：http://eml.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ckx.cashguo.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uba.quarkkingdee.top

JS:   "7".padStart(3, "0")
来源：http://cny.xinyue.icu

TS:   "7".padStart(3, "0")
来源：http://ifk.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://tin.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://ffv.zhongyouzk.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gzw.gogol.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://agi.yuanzhike.top

[E11] 反转字符串
来源：http://shx.wangdashe.top

Py:   s[::-1]
来源：http://mdd.hesvh.cn

PHP:  strrev($s);
来源：http://nuf.shangyingyoupin.top

JS:   [...s].reverse().join("")
来源：http://gmx.aizwys.cn

TS:   [...s].reverse().join("")
来源：http://szb.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yjd.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://dky.fktsv.cn

Ruby: s.reverse
来源：http://tjb.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://xjj.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://qpe.hysaishi.cn

Py:   s.count("a")
来源：http://uie.quarkkingdee.top

PHP:  substr_count($s, "a");
来源：http://bke.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://oss.yj20258.top

TS:   s.split("a").length - 1
来源：http://sjb.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aqd.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://axr.cheryme.top

Ruby: s.count("a")
来源：http://pxm.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://jhe.zhijiandao.cn

[E13] 逐字符遍历
来源：http://jqp.aizwys.cn

Py:   for ch in s: print(ch)
来源：http://isk.yongpay.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://otz.haohaochexian.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ajz.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://iqf.vqdsnc.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lax.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hfo.ehwqpu.com

Ruby: s.each_char { |ch| puts ch }
来源：http://twv.tianlin.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mvm.cucudq.cn

[E14] URL 编码与 Base64
来源：http://wgp.jinyuanbaomall.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zaj.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zld.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zkz.zhongyouzk.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fvs.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jap.jinqigufen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ctg.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://thw.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jkp.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://ska.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zuu.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fkg.uphjek.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mql.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://izc.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kow.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rfh.hesvh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mnz.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://piw.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://djh.xuanzx.com

Py:   f"{1234567:,}"
来源：http://zdt.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://sdk.hcnkem.com

JS:   (1234567).toLocaleString("en-US")
来源：http://htb.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hwm.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nxn.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cqh.xingfuxueyuan.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fug.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://wod.vehdjk.com

[E17] 首字母大写
来源：http://abs.hongshengwenyu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hdy.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ohl.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rrn.xingfuxueyuan.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zeb.sysykeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xem.cashguo.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lnf.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://pju.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qyj.jinqigfzy.top

[E18] 模板占位符替换
来源：http://muf.bbcook.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zzz.yueranfly.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ukc.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://qjb.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://aao.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yvy.hfpthk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://abo.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vbi.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bry.cashguo.top

[E19] 多行文本按行拆分
来源：http://vis.jinqigufen.top

Py:   s.splitlines()
来源：http://bov.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qbh.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://mwm.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://clx.nwbrower.top

Java: s.lines().toList()
来源：http://iro.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://grg.zdbjq.cn

Ruby: s.lines
来源：http://twv.jlsjyb.cn

C#:   s.Split('\n')
来源：http://ijj.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://amp.xuanzx.com

Py:   if not s:
来源：http://gug.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ffq.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bxj.zhongyouzk.top

TS:   if (s === "") {}
来源：http://nmr.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://cre.zycfv.cn

Go:   if s == "" {}
来源：http://otg.wangdashe.top

Ruby: if s.empty?
来源：http://fnd.smart0.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rgd.hysaishi.cn

[E21] 超长截断加省略号
来源：http://hxz.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pxf.yuxming.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uhx.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pts.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nuj.zhijiandao.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kyz.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://vbj.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dgf.jyoumei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ztm.hnxiangtu.top

[E22] 字节长度与字符长度
来源：http://tre.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://igj.smart0.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nxz.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pse.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cdb.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xee.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cra.yonumen.top

Ruby: s.bytesize;  s.length
来源：http://dil.hfpthk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ctz.sjlbkw.cn

================================================================================
来源：http://qxd.chenzaomai.com

F. 文件与目录
来源：http://flp.gzhubu.top

================================================================================
来源：http://gxp.meibo888.top

[F01] 读取整个文件
来源：http://hjc.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fvc.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://dxi.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jgn.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yay.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sql.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jxd.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://ocz.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://ird.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://zin.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ydi.yuanzhike.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rzv.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://doj.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iiu.birdmap.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pjj.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eds.xuetiantiany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jsy.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://isj.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://tka.ehwqpu.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eig.kuanghao11.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hur.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wup.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qhv.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fnv.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ase.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://hsn.yj20258888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tkd.chenjidiqi.icu

[F04] 追加写入文件
来源：http://vbx.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qih.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wet.zdbjq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wlm.bbcook.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eqc.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gdl.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qrg.52xcode.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jga.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kyj.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://aog.haohaochexian.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tkg.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://vip.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://pii.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://jzo.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jaz.yvedp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wfg.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://tus.wangdashe.top

C#:   File.Exists("a.txt")
来源：http://yhh.hammf.cn

[F06] 删除文件
来源：http://rxa.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://zfo.gogol.net.cn

PHP:  unlink("a.txt");
来源：http://fvb.aizwys.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iqp.chenjidiqi.icu

TS:   fs.unlinkSync("a.txt")
来源：http://muq.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ojo.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://vmh.yangfankeji.com

Ruby: File.delete("a.txt")
来源：http://bao.zdqjudy.top

C#:   File.Delete("a.txt");
来源：http://wsy.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://fxr.yj202588.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pwj.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ihl.havefunace.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sng.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://peu.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pui.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://avv.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gzx.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wrz.chenzaomai.com

[F08] 遍历目录
来源：http://pce.zdqjudy.top


<!-- 参考信息 -->