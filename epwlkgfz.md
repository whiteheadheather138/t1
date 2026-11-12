代发 wailian999

Java: new ArrayList<>(list);
来源：http://vfk.yuanzhike.top

Go:   copied := append([]int(nil), arr...)
来源：http://pvr.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://gtq.feifeiyinyue.top

C#:   new List<int>(list);
来源：http://tya.yueranfly.top

[D23] reduce 累积计算
来源：http://uty.hesvh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eok.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wnu.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hkc.daria6918.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oxw.bjfxy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jtt.jyoumei.cn

Go:   // 手写循环
来源：http://yzo.jinqigfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ilg.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wzr.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://hpt.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ehy.316326.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ejx.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ewq.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qru.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ngm.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zai.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qwp.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://djj.cdnleiting.top

[D25] Set 集合去重与交并差
来源：http://fii.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mal.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mcd.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://adt.meibo888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nco.yuxming.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qhr.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fyj.nanxinkj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jbp.yanxiufei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nrl.zdbjq.cn

[D26] 数组转字符串
来源：http://elz.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://aew.chenlongwang.top

PHP:  implode(", ", $arr);
来源：http://iiz.yuanzhike.top

JS:   arr.join(", ")
来源：http://ros.kuanghao11.cn

TS:   arr.join(", ")
来源：http://fut.tian-w.cn

Java: String.join(", ", list)
来源：http://idw.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://hze.cqqwz.cn

Ruby: arr.join(", ")
来源：http://osb.yj20258.top

C#:   string.Join(", ", list)
来源：http://oak.meibo888.top

================================================================================
来源：http://ync.0kj1m.cn

E. 字符串处理
来源：http://rzk.dashuyun.cn

================================================================================
来源：http://eef.zhengqikj.top

[E01] 拼接字符串
来源：http://zky.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://agq.yj20258.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dcf.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zdh.jqgufenzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://omf.snrcjt.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uhm.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cxa.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kbq.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nez.jinyuanbaomall.cn

[E02] 重复字符串
来源：http://own.0kj1m.cn

Py:   "ab" * 3
来源：http://ivk.jinqigfzy.top

PHP:  str_repeat("ab", 3);
来源：http://hzz.ppjwa.cn

JS:   "ab".repeat(3)
来源：http://bhb.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://gsm.xziqi.cn

Java: "ab".repeat(3)
来源：http://gpq.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://uis.chenlongwang.top

Ruby: "ab" * 3
来源：http://ach.316326.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ufw.sysykeji.top

[E03] 截取子串
来源：http://udw.pengpengdd.cyou

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ofk.uphjek.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kvq.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gmk.shanyushiyangkeji.top

TS:   s.slice(1, 4)
来源：http://qbp.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://wqx.wangdashe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bld.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://kfx.vqdsnc.cn

C#:   s.Substring(1, 3)
来源：http://amf.aibaodan.cn

[E04] 查找子串位置
来源：http://cmw.ywan-chungtsiang.top

Py:   s.find("x");  s.index("x")
来源：http://hnw.daxiang520.top

PHP:  strpos($s, "x");
来源：http://gxu.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lzo.chenlongwang.top

TS:   s.indexOf("x")
来源：http://iza.yonumen.top

Java: s.indexOf("x")
来源：http://ufp.shangyingyoupin.top

Go:   strings.Index(s, "x")
来源：http://ddv.0kj1m.cn

Ruby: s.index("x")
来源：http://asw.guowangkeji.top

C#:   s.IndexOf("x")
来源：http://oja.chenlongwang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kro.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dth.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ark.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tam.zhaomingkeji.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://yor.gotoacloud.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uyi.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zhi.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gwo.zhijiandao.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rhm.dashuyun.cn

[E06] 替换子串
来源：http://gft.xuetiantiany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rxm.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://bhn.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rgm.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://bxg.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ypj.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hes.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jsp.birdmap.top

C#:   s.Replace("a", "b")
来源：http://luu.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://rpl.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fwh.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yrc.hesvh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rvx.aizwys.cn

TS:   s.split(",")
来源：http://pad.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://baw.xuanzx.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ypv.epnwcf.com

Ruby: s.split(",");  s.split
来源：http://uxz.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sfw.cqqwz.cn

[E08] 数组按分隔符合并
来源：http://nbx.tanke756.top

Py:   ",".join(items)
来源：http://fms.daria6918.cn

PHP:  implode(",", $items);
来源：http://uog.shzxlz.cn

JS:   items.join(",")
来源：http://kdd.pycfn.com

TS:   items.join(",")
来源：http://hdr.xuetiantiany.cn

Java: String.join(",", items)
来源：http://bxb.yuxming.cn

Go:   strings.Join(items, ",")
来源：http://dsh.yongpay.top

Ruby: items.join(",")
来源：http://hlu.yangfankeji.com

C#:   string.Join(",", items)
来源：http://ynv.jyoumei.cn

[E09] 去除所有空白字符
来源：http://bmb.fanxiaobao.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ufd.nanxinkj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ndq.bbcook.cn

JS:   s.replace(/\s+/g, "")
来源：http://gvl.yj20258888.top

TS:   s.replace(/\s+/g, "")
来源：http://dtm.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://mgx.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://rub.guannengcc.top

Ruby: s.gsub(/\s+/, "")
来源：http://bnv.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fej.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://fys.yuanzhike.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mom.jqgufenzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hoi.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://yag.vehdjk.com

TS:   "7".padStart(3, "0")
来源：http://elh.guannengcc.top

Java: String.format("%03d", 7)
来源：http://oxe.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lhm.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ytv.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dwd.gaohongyu789.top

[E11] 反转字符串
来源：http://yge.mhx1999.top

Py:   s[::-1]
来源：http://vsp.cashguo.top

PHP:  strrev($s);
来源：http://eln.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://ivk.hywenlv.cn

TS:   [...s].reverse().join("")
来源：http://uav.yj202588.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yvq.xuetiantiany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://htc.pycfn.com

Ruby: s.reverse
来源：http://fec.jinghuilouyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qnj.jqgfzy.top

[E12] 统计某字符出现次数
来源：http://lbh.yuxming.cn

Py:   s.count("a")
来源：http://siv.yj20258.top

PHP:  substr_count($s, "a");
来源：http://aez.ivvv.top

JS:   s.split("a").length - 1
来源：http://vei.cucudq.cn

TS:   s.split("a").length - 1
来源：http://dkx.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nie.chenlongwang.top

Go:   strings.Count(s, "a")
来源：http://fqi.xuetiantiany.cn

Ruby: s.count("a")
来源：http://mtb.jiagoushi.top

C#:   s.Count(c => c == 'a')
来源：http://utd.jiagoushi.top

[E13] 逐字符遍历
来源：http://pkh.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://bek.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ggs.hfpthk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ein.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://afh.tanke756.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kgq.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iub.dashuyun.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://egd.fehbvm.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gdt.jlsjyb.cn

[E14] URL 编码与 Base64
来源：http://qaq.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qsm.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ieg.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bop.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wuq.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://usf.yuanzhike.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rdw.chenlongwang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ttv.yueranfly.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zoc.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://rjn.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jtj.0kj1m.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cqs.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gbr.jyoumei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://akh.ydzc1.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oxs.guannengcc.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wvv.aibaodan.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://otw.hysaishi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pxz.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://dem.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://ndu.yangfankeji.com

PHP:  number_format(1234567);
来源：http://zqo.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pre.yuxming.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sja.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ymc.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vqf.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://puj.sxryk.cn

C#:   1234567.ToString("N0")
来源：http://bai.haohaochexian.top

[E17] 首字母大写
来源：http://ukq.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qhi.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://sgp.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tnu.xylfe.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ofq.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xhy.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cct.zhengqikj.top

Ruby: s.capitalize
来源：http://eqr.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gwa.xziqi.cn

[E18] 模板占位符替换
来源：http://otl.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gqw.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rlb.zhiwuduotai.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yho.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kqh.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ggh.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cfq.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xwx.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bsh.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://itf.bjfxy.top

Py:   s.splitlines()
来源：http://iyw.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aai.c1oappe.top

JS:   s.split(/\r?\n/)
来源：http://ebp.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://cuz.mhx1999.top

Java: s.lines().toList()
来源：http://eyh.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://jok.cucudq.cn

Ruby: s.lines
来源：http://lzj.hesvh.cn

C#:   s.Split('\n')
来源：http://cdc.zdqjudy.top

[E20] 判断字符串是否为空
来源：http://esh.smart0.xyz

Py:   if not s:
来源：http://djj.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cqh.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lvp.jiagoushi.top

TS:   if (s === "") {}
来源：http://wsk.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://iiz.yj20258.top

Go:   if s == "" {}
来源：http://pgf.ctjpmb.com

Ruby: if s.empty?
来源：http://ihh.hammf.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kmq.tarul.cn

[E21] 超长截断加省略号
来源：http://zot.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ycq.dianchejie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://npo.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yej.shangyingyoupin.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bog.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tvw.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://bdh.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tgi.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://otn.cheryme.top

[E22] 字节长度与字符长度
来源：http://idk.xuetiantiany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xrz.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xsf.epnwcf.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fxe.yfazqb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lao.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://egv.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://trw.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://ztr.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cgn.shzxlz.cn

================================================================================
来源：http://anm.zhongyouzk.top

F. 文件与目录
来源：http://oho.nanxinkj.top

================================================================================
来源：http://ktb.uphjek.com

[F01] 读取整个文件
来源：http://fga.cdnleiting.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dko.0kj1m.cn

PHP:  file_get_contents("a.txt");
来源：http://pie.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cir.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sbm.sysykeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://omb.zhixingplan.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dxm.9152youxi.cn

Ruby: File.read("a.txt")
来源：http://ogg.sxryk.cn

C#:   File.ReadAllText("a.txt");
来源：http://kyt.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://zlg.zhijiandao.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lwa.guowangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://edl.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xfy.xingfuxueyuan.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fyn.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rbe.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wum.ppjwa.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xlt.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://knb.fanxiaobao.xyz

[F03] 写入文件（覆盖）
来源：http://rog.ydzc1.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bzx.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pno.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oux.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ruv.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oim.ybcxt.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zvk.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://cir.sufxvd.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://its.tanke756.top

[F04] 追加写入文件
来源：http://xgq.9152youxi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tkj.smart0.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sfx.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rkm.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aag.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://shh.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ooc.zdbjq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zhd.fanxiaobao.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oug.9152youxi.cn

[F05] 判断文件或目录是否存在
来源：http://cge.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hrb.jinghuilouyu.cn

PHP:  file_exists("a.txt");
来源：http://wpx.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://tyd.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://xsv.wangshuangyany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fsu.aibaodan.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tqh.ppjwa.cn

Ruby: File.exist?("a.txt")
来源：http://hwf.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://trl.yueranfly.top

[F06] 删除文件
来源：http://czb.hesvh.cn

Py:   os.remove("a.txt")
来源：http://azu.dashuyun.cn

PHP:  unlink("a.txt");
来源：http://und.jinqigufen.top

JS:   fs.unlinkSync("a.txt")
来源：http://aoq.jqgufenzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://fzm.chenjidiqi.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jnw.zhiwuduotai.top

Go:   os.Remove("a.txt")
来源：http://xwo.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://aam.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://hac.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://ord.0kj1m.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qzf.havefunace.top


<!-- 参考信息 -->