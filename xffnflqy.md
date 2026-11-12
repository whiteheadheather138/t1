代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://vkx.vqdsnc.cn

JS:   arr.includes(x)
来源：http://tkc.aizwys.cn

TS:   arr.includes(x)
来源：http://vxm.cashguo.top

Java: list.contains(x)
来源：http://qwu.cqqwz.cn

Go:   slices.Contains(arr, x)
来源：http://zql.guannengcc.top

Ruby: arr.include?(x)
来源：http://eff.gogol.net.cn

C#:   list.Contains(x)
来源：http://gsi.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://juf.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://weq.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xno.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ska.bjfxy.top

TS:   [...arr];
来源：http://nbq.haohaochexian.top

Java: new ArrayList<>(list);
来源：http://okj.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://huw.52xcode.cn

Ruby: arr.dup;  arr.clone
来源：http://qyn.zycfv.cn

C#:   new List<int>(list);
来源：http://cpk.vehdjk.com

[D23] reduce 累积计算
来源：http://chq.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ojj.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://osy.cashguo.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://syn.hywenlv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zmi.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wzr.uphjek.com

Go:   // 手写循环
来源：http://tjg.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rbr.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hgo.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://plo.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ogc.ybcxt.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lqe.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://egy.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://una.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lma.aizwys.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jmy.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://btg.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yja.fehbvm.com

[D25] Set 集合去重与交并差
来源：http://ojz.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rxf.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eid.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xcc.yongpay.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://njz.sysykeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qus.wangshuangyany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rgj.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vpo.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tch.316326.xyz

[D26] 数组转字符串
来源：http://wep.pengpengdd.cyou

Py:   ", ".join(map(str, arr))
来源：http://asx.yj20258.top

PHP:  implode(", ", $arr);
来源：http://xyk.pycfn.com

JS:   arr.join(", ")
来源：http://kgi.sweek.top

TS:   arr.join(", ")
来源：http://jzz.hongshengwenyu.top

Java: String.join(", ", list)
来源：http://dgb.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://mck.sysykeji.top

Ruby: arr.join(", ")
来源：http://ito.cqqwz.cn

C#:   string.Join(", ", list)
来源：http://ape.zycfv.cn

================================================================================
来源：http://qnx.bjfxy.top

E. 字符串处理
来源：http://cwp.gaohongyu789.top

================================================================================
来源：http://tib.yonumen.top

[E01] 拼接字符串
来源：http://fok.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qhn.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pdr.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://whw.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://brd.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gsk.sjlbkw.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://awf.yuanzhike.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tfy.yongpay.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://glv.vqdsnc.cn

[E02] 重复字符串
来源：http://qxi.yfazqb.com

Py:   "ab" * 3
来源：http://iuq.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://gjd.birdmap.top

JS:   "ab".repeat(3)
来源：http://uzu.ydzc1.top

TS:   "ab".repeat(3)
来源：http://tuc.cucudq.cn

Java: "ab".repeat(3)
来源：http://tqc.zhoulong.xyz

Go:   strings.Repeat("ab", 3)
来源：http://kvt.uphjek.com

Ruby: "ab" * 3
来源：http://rcp.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pkw.xylfe.cn

[E03] 截取子串
来源：http://ime.ywan-chungtsiang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gct.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qag.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://srd.ywan-chungtsiang.top

TS:   s.slice(1, 4)
来源：http://afq.aibaodan.cn

Java: s.substring(1, 4)
来源：http://ite.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jqc.fzhhl.top

Ruby: s[1, 3];  s[1..3]
来源：http://jip.zhijiandao.cn

C#:   s.Substring(1, 3)
来源：http://ljo.sjlbkw.cn

[E04] 查找子串位置
来源：http://jyi.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://hbi.zhijiandao.cn

PHP:  strpos($s, "x");
来源：http://zak.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gwm.aizwys.cn

TS:   s.indexOf("x")
来源：http://ygu.xuetiantiany.cn

Java: s.indexOf("x")
来源：http://dbp.ppjwa.cn

Go:   strings.Index(s, "x")
来源：http://vbr.zhengqikj.top

Ruby: s.index("x")
来源：http://zkv.gotoacloud.top

C#:   s.IndexOf("x")
来源：http://ttg.yonumen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hwt.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cca.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vtr.gzhubu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://glw.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yfd.xinyue.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ctd.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ebd.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://elt.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ink.nwbrower.top

[E06] 替换子串
来源：http://fpp.feifeiyinyue.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wsa.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://fej.0kj1m.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://acf.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://liz.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uhf.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jvi.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://agz.yj20258.top

C#:   s.Replace("a", "b")
来源：http://fme.cheryme.top

[E07] 按分隔符拆分
来源：http://obr.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eil.9152youxi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yik.zdbjq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sjd.shanyushiyangtech.top

TS:   s.split(",")
来源：http://yra.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://wmk.sweek.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://akx.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://ybb.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rvm.tian-w.cn

[E08] 数组按分隔符合并
来源：http://lek.chenzaomai.com

Py:   ",".join(items)
来源：http://rjp.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://eii.tarul.cn

JS:   items.join(",")
来源：http://agz.zhiwuduotai.top

TS:   items.join(",")
来源：http://lss.zhoulong.xyz

Java: String.join(",", items)
来源：http://prz.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://hfm.ivvv.top

Ruby: items.join(",")
来源：http://mdi.smart0.xyz

C#:   string.Join(",", items)
来源：http://wep.zhengqikj.top

[E09] 去除所有空白字符
来源：http://fdh.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dmw.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fik.fehbvm.com

JS:   s.replace(/\s+/g, "")
来源：http://bsb.cucudq.cn

TS:   s.replace(/\s+/g, "")
来源：http://jmh.aibaodan.cn

Java: s.replaceAll("\\s+", "")
来源：http://mjr.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xqt.zhijiandao.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hhn.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://svj.zhengqikj.top

[E10] 左侧补零 / 定长填充
来源：http://gxn.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://waf.cqqwz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gca.zhoulong.xyz

JS:   "7".padStart(3, "0")
来源：http://qut.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://dge.tarul.cn

Java: String.format("%03d", 7)
来源：http://wwf.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://man.fehbvm.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bjq.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dub.zdqjudy.top

[E11] 反转字符串
来源：http://krm.sxryk.cn

Py:   s[::-1]
来源：http://sop.yuxming.cn

PHP:  strrev($s);
来源：http://xit.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://ygd.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://ujf.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fpt.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://eqo.yfazqb.com

Ruby: s.reverse
来源：http://ldv.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://wqi.hnxiangtu.top

[E12] 统计某字符出现次数
来源：http://hci.yangfankeji.com

Py:   s.count("a")
来源：http://irj.zhengqikj.top

PHP:  substr_count($s, "a");
来源：http://ewi.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://jae.chenjidiqi.icu

TS:   s.split("a").length - 1
来源：http://qyb.yfazqb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hec.chenjidiqi.icu

Go:   strings.Count(s, "a")
来源：http://ukw.yfazqb.com

Ruby: s.count("a")
来源：http://hqt.zhongyouzk.top

C#:   s.Count(c => c == 'a')
来源：http://ayu.jqgufenzy.top

[E13] 逐字符遍历
来源：http://guk.meibo888.top

Py:   for ch in s: print(ch)
来源：http://ovk.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ktk.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eby.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fsc.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dnk.tarul.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://onp.zdbjq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tzg.fehbvm.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tcu.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://neh.sysykeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://goa.wangshuangyany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://srj.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kge.epnwcf.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://igj.gotoacloud.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ajn.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wft.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ywk.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fpr.bjfxy.top

[E15] HTML 转义 / 反转义
来源：http://wxw.yj20258.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ccx.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hyc.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wtq.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://mog.zhongyouzk.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pqa.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ppx.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dfe.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ycp.tianlin.xyz

[E16] 数字千分位
来源：http://hks.nwbrower.top

Py:   f"{1234567:,}"
来源：http://wtk.0kj1m.cn

PHP:  number_format(1234567);
来源：http://fcf.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kxj.hnxiangtu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bxk.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rjh.quarkkingdee.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cjk.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://itu.yvedp.cn

C#:   1234567.ToString("N0")
来源：http://wjf.epnwcf.com

[E17] 首字母大写
来源：http://krv.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aex.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://jkl.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xyq.yj20258.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pef.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qqk.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jgd.smart0.xyz

Ruby: s.capitalize
来源：http://msv.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://scb.hysaishi.cn

[E18] 模板占位符替换
来源：http://xpt.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kez.fehbvm.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zoq.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kmz.ydjk.org.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ixq.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rvd.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://csa.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vod.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eqs.guannengcc.top

[E19] 多行文本按行拆分
来源：http://gmc.tian-w.cn

Py:   s.splitlines()
来源：http://vbl.ydzc1.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lgt.shanyushiyangkeji.top

JS:   s.split(/\r?\n/)
来源：http://uec.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://dep.vehdjk.com

Java: s.lines().toList()
来源：http://ckn.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://yeo.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://sao.zdbjq.cn

C#:   s.Split('\n')
来源：http://ksy.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://tgg.dianchejie.cn

Py:   if not s:
来源：http://vws.xuanzx.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bky.xinyue.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ymf.ivvv.top

TS:   if (s === "") {}
来源：http://cpq.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://vqj.yuxming.cn

Go:   if s == "" {}
来源：http://kug.tianlin.xyz

Ruby: if s.empty?
来源：http://glx.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ozh.zhaomingkeji.xyz

[E21] 超长截断加省略号
来源：http://gwm.yj202588.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pqc.bbcook.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gjk.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wxr.shzxlz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qfg.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oqj.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://hha.xingfuxueyuan.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mev.ehwqpu.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ypv.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://wnr.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kiz.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xok.yanxiufei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jwy.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hgk.jiagoushi.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eqc.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dlp.zdqjudy.top

Ruby: s.bytesize;  s.length
来源：http://xbu.redwolf501.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fui.ydzc1.top

================================================================================
来源：http://cps.zhiwuduotai.top

F. 文件与目录
来源：http://oyf.ehwqpu.com

================================================================================
来源：http://zsl.cqqwz.cn

[F01] 读取整个文件
来源：http://iyx.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rdl.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://pki.cheryme.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kgm.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fva.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ukc.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nhm.yfazqb.com

Ruby: File.read("a.txt")
来源：http://yga.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://lbg.zhixingplan.top

[F02] 逐行读取文件
来源：http://aup.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oyp.zdqjudy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zac.smart0.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vwi.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dyw.zhixingplan.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://usn.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gfn.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jjo.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bbr.zhoulong.xyz

[F03] 写入文件（覆盖）
来源：http://dvl.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mtz.jlsjyb.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ila.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ois.sufxvd.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://naf.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ikr.jianghu66.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wrr.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://hbk.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rje.daxiang520.top

[F04] 追加写入文件
来源：http://ora.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ssp.c1oappe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mcg.zhixingplan.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bjo.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hae.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vci.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yna.sweek.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://puy.zhengqikj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bbp.cqqwz.cn

[F05] 判断文件或目录是否存在
来源：http://nxj.9152youxi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hpf.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://eds.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://qad.jqgfzy.top

TS:   fs.existsSync("a.txt")
来源：http://lxc.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sga.cqqwz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rao.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://wep.hywenlv.cn


<!-- 参考信息 -->