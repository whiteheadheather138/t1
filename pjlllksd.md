代发 wailian999

Java: new ArrayList<>(list);
来源：http://hzi.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://rcf.shanyushiyangtech.top

Ruby: arr.dup;  arr.clone
来源：http://kxq.nwbrower.top

C#:   new List<int>(list);
来源：http://zpd.yj20258.top

[D23] reduce 累积计算
来源：http://rro.jinqigfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xjl.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nct.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fdq.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lfm.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mjg.fengsongda.top

Go:   // 手写循环
来源：http://kcv.nanxinkj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uhv.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nxn.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://ghv.yj202588.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://muu.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ejg.xuetiantiany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kan.yanxiufei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tui.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://byv.xingfuxueyuan.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ify.fzhhl.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://srn.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://okp.hysaishi.cn

[D25] Set 集合去重与交并差
来源：http://wmm.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://whz.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wnt.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yfv.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zlp.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gjo.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zrc.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lkc.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kop.daxiang520.top

[D26] 数组转字符串
来源：http://hor.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://cyq.zhengqikj.top

PHP:  implode(", ", $arr);
来源：http://kye.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://yqr.chenlongwang.top

TS:   arr.join(", ")
来源：http://cba.yanxiufei.cn

Java: String.join(", ", list)
来源：http://osj.kuanghao11.cn

Go:   strings.Join(strs, ", ")
来源：http://bnc.smart0.xyz

Ruby: arr.join(", ")
来源：http://kog.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://ilw.snrcjt.cn

================================================================================
来源：http://frf.fktsv.cn

E. 字符串处理
来源：http://fzn.yj20258888.top

================================================================================
来源：http://gom.ybcxt.top

[E01] 拼接字符串
来源：http://egu.hammf.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cwd.chenjidiqi.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tuw.birdmap.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sme.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cqe.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yik.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kqt.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://plo.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rid.chenzaomai.com

[E02] 重复字符串
来源：http://mvc.yj20258888.top

Py:   "ab" * 3
来源：http://smt.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://xhe.shuidangran.top

JS:   "ab".repeat(3)
来源：http://xqi.hcnkem.com

TS:   "ab".repeat(3)
来源：http://oav.yj202588.top

Java: "ab".repeat(3)
来源：http://xzs.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://ele.xziqi.cn

Ruby: "ab" * 3
来源：http://ahq.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://edq.yuanzhike.top

[E03] 截取子串
来源：http://dxz.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xor.tianlin.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cdy.tarul.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kxm.cdnleiting.top

TS:   s.slice(1, 4)
来源：http://ldy.xuanzx.com

Java: s.substring(1, 4)
来源：http://inf.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gcu.yanxiufei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bsg.nanxuanxn.top

C#:   s.Substring(1, 3)
来源：http://hzg.hnxiangtu.top

[E04] 查找子串位置
来源：http://iaz.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://gke.cheryme.top

PHP:  strpos($s, "x");
来源：http://dht.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://soa.havefunace.top

TS:   s.indexOf("x")
来源：http://ndu.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://hpl.pengpengdd.cyou

Go:   strings.Index(s, "x")
来源：http://mhz.52xcode.cn

Ruby: s.index("x")
来源：http://aih.52xcode.cn

C#:   s.IndexOf("x")
来源：http://qtv.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vgq.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mje.nanxuanxn.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mdy.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wya.meibo888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://aty.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fcu.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uuv.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jbb.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vxz.tian-w.cn

[E06] 替换子串
来源：http://lgl.nanxuanxn.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ete.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://ain.aibaodan.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hfa.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://hif.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://coh.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zss.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nmu.ivvv.top

C#:   s.Replace("a", "b")
来源：http://gje.mhx1999.top

[E07] 按分隔符拆分
来源：http://ido.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kru.sufxvd.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nyx.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://eoc.yuanzhike.top

TS:   s.split(",")
来源：http://ddh.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://rjz.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mia.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://xta.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pxy.0kj1m.cn

[E08] 数组按分隔符合并
来源：http://hwm.zhijiandao.cn

Py:   ",".join(items)
来源：http://drg.hywenlv.cn

PHP:  implode(",", $items);
来源：http://hrv.xingfuxueyuan.xyz

JS:   items.join(",")
来源：http://dlu.gaohongyu789.top

TS:   items.join(",")
来源：http://ijz.snrcjt.cn

Java: String.join(",", items)
来源：http://ssz.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://etu.gzhubu.top

Ruby: items.join(",")
来源：http://kfx.vehdjk.com

C#:   string.Join(",", items)
来源：http://xqv.hfpthk.cn

[E09] 去除所有空白字符
来源：http://dlr.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dsb.fengsongda.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kez.jqgufenzy.top

JS:   s.replace(/\s+/g, "")
来源：http://hcm.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://yzn.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://cck.aibaodan.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zje.xingfuxueyuan.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://klt.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kbx.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://mec.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xtt.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kxd.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://css.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://vlk.xylfe.cn

Java: String.format("%03d", 7)
来源：http://elv.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://sgp.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cdv.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://udr.c1oappe.top

[E11] 反转字符串
来源：http://wlz.jqgfzy.top

Py:   s[::-1]
来源：http://mvq.hnxiangtu.top

PHP:  strrev($s);
来源：http://oxo.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://iqm.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://ggy.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cae.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://crn.zhengqikj.top

Ruby: s.reverse
来源：http://ppc.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://cxc.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://hjn.aizwys.cn

Py:   s.count("a")
来源：http://noi.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://szn.xziqi.cn

JS:   s.split("a").length - 1
来源：http://uqy.yj202588.top

TS:   s.split("a").length - 1
来源：http://mxt.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uvy.tarul.cn

Go:   strings.Count(s, "a")
来源：http://oth.vqdsnc.cn

Ruby: s.count("a")
来源：http://kok.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://sch.fehbvm.com

[E13] 逐字符遍历
来源：http://nlt.smart0.xyz

Py:   for ch in s: print(ch)
来源：http://hwk.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lhq.kuanghao11.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dcw.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://vxu.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wen.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://apz.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://lma.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cxa.ivvv.top

[E14] URL 编码与 Base64
来源：http://rov.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ker.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://szt.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vjz.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://edm.xingfuxueyuan.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://woh.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pmr.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zts.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bwn.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://hdt.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://kmj.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ccb.hfpthk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uws.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ebv.fktsv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rbo.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dcc.xuanzx.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://arh.zhiwuduotai.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kdx.cashguo.top

[E16] 数字千分位
来源：http://vza.cucudq.cn

Py:   f"{1234567:,}"
来源：http://sct.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://ubm.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://usb.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ron.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nbg.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hum.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jqi.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://twq.aizwys.cn

[E17] 首字母大写
来源：http://epa.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cjo.vqdsnc.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://csx.52xcode.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://juk.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qia.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mph.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://btn.jlsjyb.cn

Ruby: s.capitalize
来源：http://tdt.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mvu.cucudq.cn

[E18] 模板占位符替换
来源：http://wdn.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zkf.yonumen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://avr.daria6918.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xcf.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://prd.guowangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mdl.birdmap.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zmr.zhixingplan.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qym.guannengcc.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mmf.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://tml.redwolf501.top

Py:   s.splitlines()
来源：http://qbe.jinqigfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://chf.havefunace.top

JS:   s.split(/\r?\n/)
来源：http://jod.cdnleiting.top

TS:   s.split(/\r?\n/)
来源：http://pkb.xinyue.icu

Java: s.lines().toList()
来源：http://xuj.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://isz.feifeiyinyue.top

Ruby: s.lines
来源：http://gcn.zdqjudy.top

C#:   s.Split('\n')
来源：http://xfy.xinyue.icu

[E20] 判断字符串是否为空
来源：http://hax.hywenlv.cn

Py:   if not s:
来源：http://yjx.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://svc.hongshengwenyu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fcs.zhaomingkeji.xyz

TS:   if (s === "") {}
来源：http://nir.kuanghao11.cn

Java: if (s.isEmpty()) {}
来源：http://zjg.fehbvm.com

Go:   if s == "" {}
来源：http://hyt.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://nje.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cnx.chenlongwang.top

[E21] 超长截断加省略号
来源：http://ixt.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://why.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ggf.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xeb.shangyingyoupin.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xoq.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vhl.cdnleiting.top

Go:   // 按 rune 判断长度后截断
来源：http://xac.xuetiantiany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dtd.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://adv.ctjpmb.com

[E22] 字节长度与字符长度
来源：http://qgv.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kph.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qyr.xuetiantiany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fox.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hfj.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jrk.ivvv.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aud.cheryme.top

Ruby: s.bytesize;  s.length
来源：http://uiw.fktsv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://snp.epnwcf.com

================================================================================
来源：http://ogn.jinghuilouyu.cn

F. 文件与目录
来源：http://evb.iojbl.cn

================================================================================
来源：http://fbv.xuetiantiany.cn

[F01] 读取整个文件
来源：http://xxv.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sbe.fktsv.cn

PHP:  file_get_contents("a.txt");
来源：http://uju.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qfj.hammf.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://imd.nanxuanxn.top

Java: Files.readString(Path.of("a.txt"))
来源：http://swr.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sik.smart0.xyz

Ruby: File.read("a.txt")
来源：http://wgt.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://hjm.sweek.top

[F02] 逐行读取文件
来源：http://byo.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wha.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mnx.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hcv.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vts.birdmap.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pwt.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wnt.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mjl.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ipg.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://hvx.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://njk.yuxming.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yva.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xfj.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lrq.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uod.tanke756.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://glr.jinghuilouyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://qno.shuidangran.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gkq.aibaodan.cn

[F04] 追加写入文件
来源：http://wvt.dianchejie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hdi.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bov.jinghuilouyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iyg.zhijiandao.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dub.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zgr.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kpf.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yzr.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://per.jinghuilouyu.cn

[F05] 判断文件或目录是否存在
来源：http://rio.zycfv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kbz.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://del.fanxiaobao.xyz

JS:   fs.existsSync("a.txt")
来源：http://qtn.yvedp.cn

TS:   fs.existsSync("a.txt")
来源：http://big.haohaochexian.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bdg.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hvh.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://ers.uphjek.com

C#:   File.Exists("a.txt")
来源：http://tfz.0kj1m.cn

[F06] 删除文件
来源：http://pvr.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://fcd.uphjek.com

PHP:  unlink("a.txt");
来源：http://drk.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ufq.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://fsy.zhongyouzk.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://txi.havefunace.top

Go:   os.Remove("a.txt")
来源：http://yyh.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://sho.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://mzx.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://yix.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uuy.gzhubu.top


<!-- 参考信息 -->