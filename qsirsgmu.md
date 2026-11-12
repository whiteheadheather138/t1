代发 wailian999

[D23] reduce 累积计算
来源：http://kud.52xcode.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bdh.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ryx.fanxiaobao.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://onz.shanyushiyangtech.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bxm.xinyue.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://jme.yueranfly.top

Go:   // 手写循环
来源：http://zgl.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://alx.bbcook.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hhv.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://qjk.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ral.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yzk.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uwf.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tlc.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bie.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aak.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bda.hesvh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jtb.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://git.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vsq.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wud.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zcw.nanxuanxn.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vvy.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uqr.jqgfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gxq.yuxming.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pyr.uphjek.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gzf.zhengqikj.top

[D26] 数组转字符串
来源：http://twy.316326.xyz

Py:   ", ".join(map(str, arr))
来源：http://muk.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://nab.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://rar.guannengcc.top

TS:   arr.join(", ")
来源：http://xfr.yueranfly.top

Java: String.join(", ", list)
来源：http://xdu.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://wgh.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://yrq.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://osk.hongshengwenyu.top

================================================================================
来源：http://equ.sweek.top

E. 字符串处理
来源：http://iff.shanyushiyangkeji.top

================================================================================
来源：http://ybi.aizwys.cn

[E01] 拼接字符串
来源：http://bdr.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://beq.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cau.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://usm.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nwr.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zfa.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tfu.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dlp.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mwj.jinyuanbaomall.cn

[E02] 重复字符串
来源：http://rrv.zycfv.cn

Py:   "ab" * 3
来源：http://ahb.ydjk.org.cn

PHP:  str_repeat("ab", 3);
来源：http://brf.jinghuilouyu.cn

JS:   "ab".repeat(3)
来源：http://jtz.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://aum.yfazqb.com

Java: "ab".repeat(3)
来源：http://vwx.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://usx.pengpengdd.cyou

Ruby: "ab" * 3
来源：http://zee.shanyushiyangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wtd.kuanghao11.cn

[E03] 截取子串
来源：http://tnt.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tan.hywenlv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wud.shuidangran.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zyu.mhx1999.top

TS:   s.slice(1, 4)
来源：http://sjc.xylfe.cn

Java: s.substring(1, 4)
来源：http://uke.jyoumei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hdg.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://ksg.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://uob.gzhubu.top

[E04] 查找子串位置
来源：http://ddo.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://wpj.epnwcf.com

PHP:  strpos($s, "x");
来源：http://xvf.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fkx.fzhhl.top

TS:   s.indexOf("x")
来源：http://spz.aizwys.cn

Java: s.indexOf("x")
来源：http://zdm.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://prd.wangdashe.top

Ruby: s.index("x")
来源：http://grq.ppjwa.cn

C#:   s.IndexOf("x")
来源：http://zks.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kbd.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wda.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dja.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hgm.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://inv.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cga.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mhg.chenlongwang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pai.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hze.bbcook.cn

[E06] 替换子串
来源：http://eqb.havefunace.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zpl.yonumen.top

PHP:  str_replace("a", "b", $s);
来源：http://rqd.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tod.yongpay.top

TS:   s.replaceAll("a", "b")
来源：http://pvi.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lrl.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nij.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lzi.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://vwp.redwolf501.top

[E07] 按分隔符拆分
来源：http://bfn.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hgu.tanke756.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zcr.yueranfly.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lfc.yangfankeji.com

TS:   s.split(",")
来源：http://jog.hnqzz.top

Java: s.split(",");  s.split("\\s+")
来源：http://bdx.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://moo.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://ljv.yj202588.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lez.yonumen.top

[E08] 数组按分隔符合并
来源：http://cxn.c1oappe.top

Py:   ",".join(items)
来源：http://mem.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://djc.yangfankeji.com

JS:   items.join(",")
来源：http://lbp.bjfxy.top

TS:   items.join(",")
来源：http://idr.52xcode.cn

Java: String.join(",", items)
来源：http://jhh.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://cdg.bjfxy.top

Ruby: items.join(",")
来源：http://ome.yj20258.top

C#:   string.Join(",", items)
来源：http://kpa.pycfn.com

[E09] 去除所有空白字符
来源：http://cxd.9152youxi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wji.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kni.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://ugi.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://zdv.zhixingplan.top

Java: s.replaceAll("\\s+", "")
来源：http://aox.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://hwb.hnqzz.top

Ruby: s.gsub(/\s+/, "")
来源：http://tmh.jqgufenzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xbn.hnxiangtu.top

[E10] 左侧补零 / 定长填充
来源：http://pyq.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ykc.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kmx.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://rkx.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://xgr.iojbl.cn

Java: String.format("%03d", 7)
来源：http://gee.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dyt.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cmn.yanxiufei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wba.quarkkingdee.top

[E11] 反转字符串
来源：http://jgw.ywan-chungtsiang.top

Py:   s[::-1]
来源：http://mlo.shangyingyoupin.top

PHP:  strrev($s);
来源：http://znx.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://doc.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://nue.yj20258.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lkl.jianghu66.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ced.aizwys.cn

Ruby: s.reverse
来源：http://zsp.xziqi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://doe.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://mqn.hywenlv.cn

Py:   s.count("a")
来源：http://jge.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://tuu.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://tib.wangdashe.top

TS:   s.split("a").length - 1
来源：http://axp.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xkj.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://ebx.birdmap.top

Ruby: s.count("a")
来源：http://nwl.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://evs.ydzc1.top

[E13] 逐字符遍历
来源：http://hgu.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://rhi.yongpay.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xxe.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hdm.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vcy.shuidangran.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mvm.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hqe.shanyushiyangtech.top

Ruby: s.each_char { |ch| puts ch }
来源：http://brw.tianlin.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pdq.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://ebb.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dvd.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gjl.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uar.jiagoushi.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zya.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mtm.redwolf501.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oax.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bas.meibo888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jdo.hnxiangtu.top

[E15] HTML 转义 / 反转义
来源：http://zpu.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xjn.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dib.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zma.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qke.sweek.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xlw.meibo888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wxg.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hmv.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mlj.zycfv.cn

[E16] 数字千分位
来源：http://kqw.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://nav.52xcode.cn

PHP:  number_format(1234567);
来源：http://xjg.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wze.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jtp.jinyuanbaomall.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zmz.yj20258888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://auk.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ema.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://mfk.jqgufenzy.top

[E17] 首字母大写
来源：http://xno.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zbz.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lpk.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zkf.dianchejie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sad.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gpz.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xpp.yj20258.top

Ruby: s.capitalize
来源：http://jvn.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ifd.yangfankeji.com

[E18] 模板占位符替换
来源：http://xcq.ywan-chungtsiang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fnz.iojbl.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xjb.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lts.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zwv.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qtw.tanke756.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://slf.jlsjyb.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://maa.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jqz.xinyue.icu

[E19] 多行文本按行拆分
来源：http://dvr.jqgfzy.top

Py:   s.splitlines()
来源：http://pge.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qgh.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://jva.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://bzw.shangyingyoupin.top

Java: s.lines().toList()
来源：http://kfk.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://wpn.0kj1m.cn

Ruby: s.lines
来源：http://emy.nanxuanxn.top

C#:   s.Split('\n')
来源：http://igx.fengsongda.top

[E20] 判断字符串是否为空
来源：http://evc.mhx1999.top

Py:   if not s:
来源：http://nqe.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qvo.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bex.zhengqikj.top

TS:   if (s === "") {}
来源：http://mvx.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://sbs.zhixingplan.top

Go:   if s == "" {}
来源：http://rjn.ehwqpu.com

Ruby: if s.empty?
来源：http://yrn.yuanzhike.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fzz.9152youxi.cn

[E21] 超长截断加省略号
来源：http://fzn.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nsl.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://klu.jinqigfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tum.jqgufenzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ihw.yangfankeji.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://czw.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://hfv.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zeu.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vlf.jianghu66.top

[E22] 字节长度与字符长度
来源：http://xcf.kuanghao11.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lux.ydjk.org.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bay.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hzu.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://evj.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cvj.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://acf.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://iop.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iyy.pengpengdd.cyou

================================================================================
来源：http://ewa.yj202588.top

F. 文件与目录
来源：http://ikh.guowangkeji.top

================================================================================
来源：http://fwi.jlsjyb.cn

[F01] 读取整个文件
来源：http://suy.ivvv.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bxy.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://vqa.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kzw.yj20258888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kyy.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://zmq.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hvq.yvedp.cn

Ruby: File.read("a.txt")
来源：http://tgw.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://ycg.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://jho.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://glf.0kj1m.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hib.chenlongwang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mbx.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mby.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zmw.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tlg.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aod.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rui.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://ivo.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ngr.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ego.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zkv.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qka.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hoo.quarkkingdee.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qhl.quarkkingdee.top

Ruby: File.write("a.txt", "hi")
来源：http://uzj.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iqg.haohaochexian.top

[F04] 追加写入文件
来源：http://bku.shzxlz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rqe.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dhq.haohaochexian.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pbp.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://loh.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hzk.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ofr.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eod.cqqwz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sbb.ydjk.org.cn

[F05] 判断文件或目录是否存在
来源：http://adr.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fce.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://ozn.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://vwu.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://pke.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://zac.jiagoushi.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oos.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://xjb.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://vom.hnxiangtu.top

[F06] 删除文件
来源：http://juk.sysykeji.top

Py:   os.remove("a.txt")
来源：http://bic.sxryk.cn

PHP:  unlink("a.txt");
来源：http://gwz.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://lfm.chenlongwang.top

TS:   fs.unlinkSync("a.txt")
来源：http://bfi.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ufv.uphjek.com

Go:   os.Remove("a.txt")
来源：http://esa.uphjek.com

Ruby: File.delete("a.txt")
来源：http://bjc.zdqjudy.top

C#:   File.Delete("a.txt");
来源：http://ppk.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://dpn.pycfn.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tox.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://exv.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jxa.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rot.yj20258888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dik.chenzaomai.com


<!-- 参考信息 -->