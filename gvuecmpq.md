代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://vro.zhengqikj.top

JS:   arr.includes(x)
来源：http://xki.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://rec.wangshuangyany.cn

Java: list.contains(x)
来源：http://qxh.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://hoo.smart0.xyz

Ruby: arr.include?(x)
来源：http://nrg.epnwcf.com

C#:   list.Contains(x)
来源：http://bpa.fengsongda.top

[D22] 复制数组（避免共享引用）
来源：http://hcb.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://agu.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oer.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zjt.fehbvm.com

TS:   [...arr];
来源：http://rtk.c1oappe.top

Java: new ArrayList<>(list);
来源：http://zfz.fktsv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lal.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://wed.hywenlv.cn

C#:   new List<int>(list);
来源：http://zcx.zhiwuduotai.top

[D23] reduce 累积计算
来源：http://zdr.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gjb.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hqc.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fxg.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jwl.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hhb.hnxiangtu.top

Go:   // 手写循环
来源：http://kfq.smart0.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://myh.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iua.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://uuw.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://agj.zhixingplan.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://duj.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zgr.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mci.cheryme.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wzk.zycfv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vnc.yj202588.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gmm.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ikl.hnxiangtu.top

[D25] Set 集合去重与交并差
来源：http://meo.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fcn.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tnf.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yfp.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tuv.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kma.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xsx.chenlongwang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dtd.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pls.tian-w.cn

[D26] 数组转字符串
来源：http://buy.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://gvf.zhaomingkeji.xyz

PHP:  implode(", ", $arr);
来源：http://dpz.zhixingplan.top

JS:   arr.join(", ")
来源：http://dun.zdbjq.cn

TS:   arr.join(", ")
来源：http://kud.feifeiyinyue.top

Java: String.join(", ", list)
来源：http://yfa.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://xmy.chenjidiqi.icu

Ruby: arr.join(", ")
来源：http://wxf.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://pqq.xingfuxueyuan.xyz

================================================================================
来源：http://fsg.cheryme.top

E. 字符串处理
来源：http://wmt.quarkkingdee.top

================================================================================
来源：http://mgg.9152youxi.cn

[E01] 拼接字符串
来源：http://oqa.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mub.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xtr.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://biw.vqdsnc.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sdl.guannengcc.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://azv.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fah.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cxo.guannengcc.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://aqk.ydzc1.top

[E02] 重复字符串
来源：http://rmu.chenlongwang.top

Py:   "ab" * 3
来源：http://atl.yanxiufei.cn

PHP:  str_repeat("ab", 3);
来源：http://oss.ppjwa.cn

JS:   "ab".repeat(3)
来源：http://oar.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://owg.xziqi.cn

Java: "ab".repeat(3)
来源：http://wbc.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://vwk.nwbrower.top

Ruby: "ab" * 3
来源：http://mpu.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uyf.ppjwa.cn

[E03] 截取子串
来源：http://tyv.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://frw.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wed.yuanzhike.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://awi.shanyushiyangkeji.top

TS:   s.slice(1, 4)
来源：http://ofx.shuidangran.top

Java: s.substring(1, 4)
来源：http://ssr.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fhb.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://bwe.jqgfzy.top

C#:   s.Substring(1, 3)
来源：http://ire.zdqjudy.top

[E04] 查找子串位置
来源：http://vlz.c1oappe.top

Py:   s.find("x");  s.index("x")
来源：http://cst.yongpay.top

PHP:  strpos($s, "x");
来源：http://zmk.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zsx.shuidangran.top

TS:   s.indexOf("x")
来源：http://wgk.yvedp.cn

Java: s.indexOf("x")
来源：http://tgp.shanyushiyangtech.top

Go:   strings.Index(s, "x")
来源：http://pro.gotoacloud.top

Ruby: s.index("x")
来源：http://bht.cheryme.top

C#:   s.IndexOf("x")
来源：http://jro.dashuyun.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oyx.jlsjyb.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://udm.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fok.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tsk.yangfankeji.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://vff.gzhubu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wxk.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tby.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wnw.shzxlz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nmc.andypj.xyz

[E06] 替换子串
来源：http://wbe.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sji.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://tbd.epnwcf.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xnt.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://qjm.snrcjt.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ono.bbcook.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fuj.316326.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vfi.cqqwz.cn

C#:   s.Replace("a", "b")
来源：http://nod.9152youxi.cn

[E07] 按分隔符拆分
来源：http://cah.ppjwa.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vij.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kdl.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aux.shuidangran.top

TS:   s.split(",")
来源：http://vxl.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://iej.chenlongwang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://exn.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://upm.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gvd.hywenlv.cn

[E08] 数组按分隔符合并
来源：http://gzy.cashguo.top

Py:   ",".join(items)
来源：http://csa.yueranfly.top

PHP:  implode(",", $items);
来源：http://ape.shanyushiyangtech.top

JS:   items.join(",")
来源：http://ssx.zhiwuduotai.top

TS:   items.join(",")
来源：http://ops.jinqigfzy.top

Java: String.join(",", items)
来源：http://dnp.jyoumei.cn

Go:   strings.Join(items, ",")
来源：http://vwa.vqdsnc.cn

Ruby: items.join(",")
来源：http://egu.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://stw.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://yrz.zhixingplan.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xab.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nqi.sweek.top

JS:   s.replace(/\s+/g, "")
来源：http://xxb.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://ktu.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://ote.jqgfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zde.pycfn.com

Ruby: s.gsub(/\s+/, "")
来源：http://lqa.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bco.aibaodan.cn

[E10] 左侧补零 / 定长填充
来源：http://pek.shangyingyoupin.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kpm.ivvv.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kyv.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://wbh.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://wwe.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://gze.ivvv.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fsk.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hyr.jyoumei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hyp.pengpengdd.cyou

[E11] 反转字符串
来源：http://wfa.vqdsnc.cn

Py:   s[::-1]
来源：http://rtz.chenjidiqi.icu

PHP:  strrev($s);
来源：http://pnv.yanxiufei.cn

JS:   [...s].reverse().join("")
来源：http://efr.ydjk.org.cn

TS:   [...s].reverse().join("")
来源：http://pxu.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://mkh.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jde.jyoumei.cn

Ruby: s.reverse
来源：http://jrt.redwolf501.top

C#:   new string(s.Reverse().ToArray())
来源：http://yal.yanxiufei.cn

[E12] 统计某字符出现次数
来源：http://ohw.epnwcf.com

Py:   s.count("a")
来源：http://vkk.nanxinkj.top

PHP:  substr_count($s, "a");
来源：http://zbj.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://jrt.smart0.xyz

TS:   s.split("a").length - 1
来源：http://oqp.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fov.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://ymd.jqgufenzy.top

Ruby: s.count("a")
来源：http://boq.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://hkb.pengpengdd.cyou

[E13] 逐字符遍历
来源：http://vkq.zhaomingkeji.xyz

Py:   for ch in s: print(ch)
来源：http://szm.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zsi.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pfe.cheryme.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://isy.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dls.meibo888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ixh.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ibj.jinghuilouyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bme.fehbvm.com

[E14] URL 编码与 Base64
来源：http://ymp.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pwi.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ekb.jinghuilouyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fur.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qnx.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ogw.hongshengwenyu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lis.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wld.dianchejie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lhy.jinyuanbaomall.cn

[E15] HTML 转义 / 反转义
来源：http://fwy.chenjidiqi.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://ruc.cdnleiting.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uet.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gnp.kuanghao11.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bfa.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://piq.zhongyouzk.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vyz.zhoulong.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xnj.jinyuanbaomall.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nfp.zhongyouzk.top

[E16] 数字千分位
来源：http://wgc.chenzaomai.com

Py:   f"{1234567:,}"
来源：http://pid.aibaodan.cn

PHP:  number_format(1234567);
来源：http://xyx.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://eyz.zhaomingkeji.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://ftg.ehwqpu.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fot.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rrj.aizwys.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rsw.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://mju.aizwys.cn

[E17] 首字母大写
来源：http://jzk.snrcjt.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dim.hammf.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lcj.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qiv.yanxiufei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ajp.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hrj.svipenyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xhx.dianchejie.cn

Ruby: s.capitalize
来源：http://bvx.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iye.yonumen.top

[E18] 模板占位符替换
来源：http://uja.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mru.jinyuanbaomall.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jwi.0kj1m.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ybb.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kwv.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xdj.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://krt.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tfr.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dxh.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://pbx.yuxming.cn

Py:   s.splitlines()
来源：http://oya.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pfm.sysykeji.top

JS:   s.split(/\r?\n/)
来源：http://tlo.havefunace.top

TS:   s.split(/\r?\n/)
来源：http://hom.smart0.xyz

Java: s.lines().toList()
来源：http://mko.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://mmi.birdmap.top

Ruby: s.lines
来源：http://llf.zhengqikj.top

C#:   s.Split('\n')
来源：http://zgk.zhijiandao.cn

[E20] 判断字符串是否为空
来源：http://isv.316326.xyz

Py:   if not s:
来源：http://gkj.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vwj.zdbjq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ylw.chenlongwang.top

TS:   if (s === "") {}
来源：http://wmj.havefunace.top

Java: if (s.isEmpty()) {}
来源：http://qpp.jiagoushi.top

Go:   if s == "" {}
来源：http://kgp.vehdjk.com

Ruby: if s.empty?
来源：http://hmq.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cdk.yvedp.cn

[E21] 超长截断加省略号
来源：http://hjj.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://paa.hfpthk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jaw.meibo888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kfd.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oef.xingfuxueyuan.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vee.xuanzx.com

Go:   // 按 rune 判断长度后截断
来源：http://avb.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kms.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jlx.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://foo.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tew.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ibx.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bwy.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lpt.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ygg.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mvs.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://tco.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uss.cheryme.top

================================================================================
来源：http://sdv.shanyushiyangtech.top

F. 文件与目录
来源：http://ufz.ppjwa.cn

================================================================================
来源：http://ppl.nwbrower.top

[F01] 读取整个文件
来源：http://jom.jiagoushi.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://msw.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://fbp.yongpay.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cwe.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kbv.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ddl.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zds.pycfn.com

Ruby: File.read("a.txt")
来源：http://epq.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://iyn.c1oappe.top

[F02] 逐行读取文件
来源：http://dck.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lwr.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://htp.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lyn.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rmt.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sko.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ncs.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lov.chenjidiqi.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mgp.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://nhh.chenzaomai.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://psf.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fce.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://roi.gzhubu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jat.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://agn.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://afj.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://jfv.jyoumei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://otr.tian-w.cn

[F04] 追加写入文件
来源：http://uth.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hoe.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qwp.pengpengdd.cyou

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tkz.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ske.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yyj.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zfv.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qnt.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vjd.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://rnj.quarkkingdee.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fjs.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://wcv.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://hwq.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://xtq.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://ipv.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tyc.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://dgg.feifeiyinyue.top


<!-- 参考信息 -->