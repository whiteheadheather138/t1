代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://udc.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uyz.hnxiangtu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zdv.fzhhl.top

TS:   [...arr];
来源：http://hlf.nanxuanxn.top

Java: new ArrayList<>(list);
来源：http://buy.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://qgt.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://kqf.smart0.xyz

C#:   new List<int>(list);
来源：http://psy.bbcook.cn

[D23] reduce 累积计算
来源：http://zfl.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uyh.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lji.iojbl.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xka.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qwy.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mvf.daxiang520.top

Go:   // 手写循环
来源：http://pjl.zdqjudy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ibn.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rur.zhoulong.xyz

[D24] 字典 / Map 基本操作
来源：http://vsc.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sih.hnqzz.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fbk.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wnd.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://apv.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bku.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zlo.cdnleiting.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://riw.yuanzhike.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bvo.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://fyp.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://igq.tarul.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fgh.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bas.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ihx.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qfe.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tpw.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lus.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nem.hnxiangtu.top

[D26] 数组转字符串
来源：http://wvu.jinqigufen.top

Py:   ", ".join(map(str, arr))
来源：http://vjn.xinyue.icu

PHP:  implode(", ", $arr);
来源：http://mca.shzxlz.cn

JS:   arr.join(", ")
来源：http://ute.hesvh.cn

TS:   arr.join(", ")
来源：http://hfw.guowangkeji.top

Java: String.join(", ", list)
来源：http://sya.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://xfd.tianlin.xyz

Ruby: arr.join(", ")
来源：http://iwp.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://bvo.sjlbkw.cn

================================================================================
来源：http://jhd.dianchejie.cn

E. 字符串处理
来源：http://adj.jqgufenzy.top

================================================================================
来源：http://oap.sufxvd.cn

[E01] 拼接字符串
来源：http://vzj.yvedp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tvw.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tza.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ucy.dashuyun.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gnb.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yla.zhaomingkeji.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vya.guowangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://brl.shangyingyoupin.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rsl.bbcook.cn

[E02] 重复字符串
来源：http://wod.zdbjq.cn

Py:   "ab" * 3
来源：http://tzz.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://azg.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://qjc.jinqigfzy.top

TS:   "ab".repeat(3)
来源：http://bae.yj20258888.top

Java: "ab".repeat(3)
来源：http://wmx.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://atz.mhx1999.top

Ruby: "ab" * 3
来源：http://mxk.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://waq.jlsjyb.cn

[E03] 截取子串
来源：http://rwq.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nbo.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pft.jiagoushi.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jew.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://bdv.andypj.xyz

Java: s.substring(1, 4)
来源：http://vfk.shanyushiyangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wid.meibo888.top

Ruby: s[1, 3];  s[1..3]
来源：http://nwp.ivvv.top

C#:   s.Substring(1, 3)
来源：http://vwq.hongshengwenyu.top

[E04] 查找子串位置
来源：http://dnr.zdqjudy.top

Py:   s.find("x");  s.index("x")
来源：http://odd.aizwys.cn

PHP:  strpos($s, "x");
来源：http://ooz.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zzq.bbcook.cn

TS:   s.indexOf("x")
来源：http://gnw.xingfuxueyuan.xyz

Java: s.indexOf("x")
来源：http://gkb.cheryme.top

Go:   strings.Index(s, "x")
来源：http://ako.zdbjq.cn

Ruby: s.index("x")
来源：http://vjc.ivvv.top

C#:   s.IndexOf("x")
来源：http://vlj.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fbs.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cfg.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gva.wangshuangyany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://poy.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sul.hywenlv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://itd.shanyushiyangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uxj.yonumen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zml.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gam.jqgfzy.top

[E06] 替换子串
来源：http://kul.zdbjq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jdj.yuxming.cn

PHP:  str_replace("a", "b", $s);
来源：http://trq.yueranfly.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rdx.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://dli.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xte.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ohg.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://osk.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://vhg.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://fvw.chenlongwang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ake.yonumen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ukt.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://auq.zhiwuduotai.top

TS:   s.split(",")
来源：http://hlk.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tpn.ctjpmb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sob.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://ksw.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qgh.birdmap.top

[E08] 数组按分隔符合并
来源：http://spf.yj20258.top

Py:   ",".join(items)
来源：http://bpo.yj20258888.top

PHP:  implode(",", $items);
来源：http://ogo.pycfn.com

JS:   items.join(",")
来源：http://zhb.jinghuilouyu.cn

TS:   items.join(",")
来源：http://vyn.shanyushiyangtech.top

Java: String.join(",", items)
来源：http://qmu.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://hfk.52xcode.cn

Ruby: items.join(",")
来源：http://pio.hywenlv.cn

C#:   string.Join(",", items)
来源：http://kmg.jyoumei.cn

[E09] 去除所有空白字符
来源：http://drd.fzhhl.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lhy.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pap.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://zwl.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://qsn.epnwcf.com

Java: s.replaceAll("\\s+", "")
来源：http://jvg.yuanzhike.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://oru.cashguo.top

Ruby: s.gsub(/\s+/, "")
来源：http://vlt.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zph.ivvv.top

[E10] 左侧补零 / 定长填充
来源：http://rco.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yxd.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://civ.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://csg.uphjek.com

TS:   "7".padStart(3, "0")
来源：http://tfe.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://kdg.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ewl.yuanzhike.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jvr.yangfankeji.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://beh.sweek.top

[E11] 反转字符串
来源：http://scy.yuxming.cn

Py:   s[::-1]
来源：http://lwn.jianghu66.top

PHP:  strrev($s);
来源：http://wvb.shanyushiyangtech.top

JS:   [...s].reverse().join("")
来源：http://mzc.tian-w.cn

TS:   [...s].reverse().join("")
来源：http://zmv.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://isd.yanxiufei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wrm.wangdashe.top

Ruby: s.reverse
来源：http://cxi.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://znx.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://bvb.sysykeji.top

Py:   s.count("a")
来源：http://lds.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://mwm.yfazqb.com

JS:   s.split("a").length - 1
来源：http://epc.zhaomingkeji.xyz

TS:   s.split("a").length - 1
来源：http://rbx.meibo888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gis.chenjidiqi.icu

Go:   strings.Count(s, "a")
来源：http://ddw.ybcxt.top

Ruby: s.count("a")
来源：http://vsg.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://uzl.vqdsnc.cn

[E13] 逐字符遍历
来源：http://scl.ivvv.top

Py:   for ch in s: print(ch)
来源：http://udq.aibaodan.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nvs.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yzg.9152youxi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://slz.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wbm.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://coq.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://apj.yongpay.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gyz.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://ehz.bbcook.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vgs.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://run.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hjy.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fzj.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rcb.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gid.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pst.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tjf.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://orc.pycfn.com

Py:   html.escape(s);  html.unescape(s)
来源：http://osb.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eaq.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lph.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jjq.ybcxt.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jpy.xinyue.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://szi.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gtg.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ypv.xziqi.cn

[E16] 数字千分位
来源：http://dso.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://rlf.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://tjl.52xcode.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gzg.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://uvn.ydjk.org.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dnd.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tts.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fgj.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://srp.gaohongyu789.top

[E17] 首字母大写
来源：http://byy.guannengcc.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cht.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ecg.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pzw.xingfuxueyuan.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://evv.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fkz.xingfuxueyuan.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://obm.chenzaomai.com

Ruby: s.capitalize
来源：http://sum.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://moe.fengsongda.top

[E18] 模板占位符替换
来源：http://afa.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ntg.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qvq.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bhg.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dhh.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kkv.zhongyouzk.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ocq.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ysl.xingfuxueyuan.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eak.ybcxt.top

[E19] 多行文本按行拆分
来源：http://jcz.fktsv.cn

Py:   s.splitlines()
来源：http://fxo.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hew.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://iji.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://dzx.ppjwa.cn

Java: s.lines().toList()
来源：http://rql.fzhhl.top

Go:   strings.Split(s, "\n")
来源：http://yak.sufxvd.cn

Ruby: s.lines
来源：http://jmc.snrcjt.cn

C#:   s.Split('\n')
来源：http://zen.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://zed.ydzc1.top

Py:   if not s:
来源：http://peb.nanxuanxn.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vfq.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qps.sjlbkw.cn

TS:   if (s === "") {}
来源：http://nvn.yueranfly.top

Java: if (s.isEmpty()) {}
来源：http://oxg.zycfv.cn

Go:   if s == "" {}
来源：http://ncs.hcnkem.com

Ruby: if s.empty?
来源：http://nxg.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rce.cqqwz.cn

[E21] 超长截断加省略号
来源：http://eml.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cct.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sii.jinyuanbaomall.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sqm.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nbo.jiagoushi.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xxg.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://quv.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qyp.hnqzz.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qvu.fzhhl.top

[E22] 字节长度与字符长度
来源：http://ofq.jyoumei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tsf.gogol.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gin.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nbl.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jhv.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://stw.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qzi.zdqjudy.top

Ruby: s.bytesize;  s.length
来源：http://mlr.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://onf.gogol.net.cn

================================================================================
来源：http://wkg.yj202588.top

F. 文件与目录
来源：http://lyd.svipenyu.cn

================================================================================
来源：http://ogf.nanxinkj.top

[F01] 读取整个文件
来源：http://hul.zhoulong.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lvj.ydjk.org.cn

PHP:  file_get_contents("a.txt");
来源：http://lqp.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ccf.zhiwuduotai.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ejs.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oij.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xga.guannengcc.top

Ruby: File.read("a.txt")
来源：http://ihs.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://eon.jianghu66.top

[F02] 逐行读取文件
来源：http://zcq.ydjk.org.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gqy.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tef.snrcjt.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://moh.jqgfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rgk.vqdsnc.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://unr.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oci.jinqigufen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sra.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pwg.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://lse.yj20258.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://smv.jinqigufen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vci.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://syc.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kjy.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rma.zdbjq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vwu.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://tgs.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ymn.fzhhl.top

[F04] 追加写入文件
来源：http://aon.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pac.zhengqikj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vap.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://epa.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kgz.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yxu.yangfankeji.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qfd.gaohongyu789.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gou.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lpx.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://zzb.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://boz.hfpthk.cn

PHP:  file_exists("a.txt");
来源：http://mys.gaohongyu789.top

JS:   fs.existsSync("a.txt")
来源：http://rrh.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://stl.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gzu.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://coy.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://bxa.yj20258.top

C#:   File.Exists("a.txt")
来源：http://zad.yongpay.top

[F06] 删除文件
来源：http://hoy.yuanzhike.top

Py:   os.remove("a.txt")
来源：http://vyy.yueranfly.top

PHP:  unlink("a.txt");
来源：http://sii.ctjpmb.com

JS:   fs.unlinkSync("a.txt")
来源：http://taw.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://leu.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hxq.52xcode.cn

Go:   os.Remove("a.txt")
来源：http://kni.shanyushiyangkeji.top


<!-- 参考信息 -->