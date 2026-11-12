代发 wailian999

[D23] reduce 累积计算
来源：http://hdq.shanyushiyangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xhc.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jdd.quarkkingdee.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sem.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://opp.aizwys.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oda.mhx1999.top

Go:   // 手写循环
来源：http://rfc.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xnd.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tvu.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://jfp.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hnj.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lum.dashuyun.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bpy.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vbc.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vxm.shzxlz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://quy.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mlx.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rvt.yvedp.cn

[D25] Set 集合去重与交并差
来源：http://lun.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qic.fehbvm.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zcl.cashguo.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vrh.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jxd.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qtn.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ubg.jqgufenzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tak.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gnm.kuanghao11.cn

[D26] 数组转字符串
来源：http://izl.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://ruf.feifeiyinyue.top

PHP:  implode(", ", $arr);
来源：http://max.xingfuxueyuan.xyz

JS:   arr.join(", ")
来源：http://pup.pengpengdd.cyou

TS:   arr.join(", ")
来源：http://gsb.nanxinkj.top

Java: String.join(", ", list)
来源：http://ztx.gzhubu.top

Go:   strings.Join(strs, ", ")
来源：http://dbx.zhijiandao.cn

Ruby: arr.join(", ")
来源：http://izv.fengsongda.top

C#:   string.Join(", ", list)
来源：http://utg.chenlongwang.top

================================================================================
来源：http://kfv.jinghuilouyu.cn

E. 字符串处理
来源：http://nxc.kuanghao11.cn

================================================================================
来源：http://epm.snrcjt.cn

[E01] 拼接字符串
来源：http://wqe.yuxming.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yxv.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zlr.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://scq.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zeq.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sne.yj20258888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ipo.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vbn.zhijiandao.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://urs.hywenlv.cn

[E02] 重复字符串
来源：http://eat.snrcjt.cn

Py:   "ab" * 3
来源：http://jpv.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://cwv.haohaochexian.top

JS:   "ab".repeat(3)
来源：http://pog.cucudq.cn

TS:   "ab".repeat(3)
来源：http://hbg.tian-w.cn

Java: "ab".repeat(3)
来源：http://aps.zhiwuduotai.top

Go:   strings.Repeat("ab", 3)
来源：http://kma.tarul.cn

Ruby: "ab" * 3
来源：http://soa.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lss.yongpay.top

[E03] 截取子串
来源：http://prg.ctjpmb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://edg.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zqg.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kab.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://ehx.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://vlo.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://say.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://jma.meibo888.top

C#:   s.Substring(1, 3)
来源：http://tos.jinqigufen.top

[E04] 查找子串位置
来源：http://ihj.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://ohd.jiagoushi.top

PHP:  strpos($s, "x");
来源：http://aoc.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lmj.yj20258888.top

TS:   s.indexOf("x")
来源：http://bnf.vqdsnc.cn

Java: s.indexOf("x")
来源：http://ggr.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://mbh.yanxiufei.cn

Ruby: s.index("x")
来源：http://icj.c1oappe.top

C#:   s.IndexOf("x")
来源：http://kfn.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ybn.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://htl.uphjek.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fiv.aizwys.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gnr.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://fjq.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fbp.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yqb.dashuyun.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lly.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uvw.yanxiufei.cn

[E06] 替换子串
来源：http://egs.zhijiandao.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aon.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://jxf.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ude.feifeiyinyue.top

TS:   s.replaceAll("a", "b")
来源：http://zbq.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eyn.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pai.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://osw.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://yrx.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://euy.uphjek.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xav.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fzx.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lyk.hywenlv.cn

TS:   s.split(",")
来源：http://nkq.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://ckt.vehdjk.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jpp.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://ltb.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pug.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://rsv.hcnkem.com

Py:   ",".join(items)
来源：http://wor.tianlin.xyz

PHP:  implode(",", $items);
来源：http://kkw.vqdsnc.cn

JS:   items.join(",")
来源：http://ksa.jinqigfzy.top

TS:   items.join(",")
来源：http://wtb.yj20258.top

Java: String.join(",", items)
来源：http://udh.xuetiantiany.cn

Go:   strings.Join(items, ",")
来源：http://qdv.ydzc1.top

Ruby: items.join(",")
来源：http://cmq.iojbl.cn

C#:   string.Join(",", items)
来源：http://via.9152youxi.cn

[E09] 去除所有空白字符
来源：http://ogv.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vnn.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jxl.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://qii.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://jpp.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://rfr.xinyue.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://xwu.cqqwz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://acf.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pnd.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://rsl.kuanghao11.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tta.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jwu.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://mgw.jinqigufen.top

TS:   "7".padStart(3, "0")
来源：http://dxz.jianghu66.top

Java: String.format("%03d", 7)
来源：http://ixo.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nlm.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jjg.yfazqb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tkj.sufxvd.cn

[E11] 反转字符串
来源：http://vzz.yuxming.cn

Py:   s[::-1]
来源：http://tkk.hysaishi.cn

PHP:  strrev($s);
来源：http://mba.dashuyun.cn

JS:   [...s].reverse().join("")
来源：http://mga.hnxiangtu.top

TS:   [...s].reverse().join("")
来源：http://ycb.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mfz.uphjek.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ahy.yuanzhike.top

Ruby: s.reverse
来源：http://yvm.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://cer.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://win.shzxlz.cn

Py:   s.count("a")
来源：http://ygz.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://gxn.guowangkeji.top

JS:   s.split("a").length - 1
来源：http://vwf.hcnkem.com

TS:   s.split("a").length - 1
来源：http://dmn.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vkj.uphjek.com

Go:   strings.Count(s, "a")
来源：http://lpi.fanxiaobao.xyz

Ruby: s.count("a")
来源：http://xvu.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://jfu.yfazqb.com

[E13] 逐字符遍历
来源：http://rbi.quarkkingdee.top

Py:   for ch in s: print(ch)
来源：http://khw.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qjr.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zpb.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://enz.yongpay.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://alr.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ynw.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://iwp.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zmp.ydjk.org.cn

[E14] URL 编码与 Base64
来源：http://zkw.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gxt.tarul.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mae.zdbjq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://muj.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hkb.zdqjudy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lnu.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wka.fktsv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://boc.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jvk.sysykeji.top

[E15] HTML 转义 / 反转义
来源：http://aze.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xmt.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qqx.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fpz.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tlb.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cdj.jinqigufen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://znt.vehdjk.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aua.tanke756.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mjh.jqgfzy.top

[E16] 数字千分位
来源：http://xqe.mhx1999.top

Py:   f"{1234567:,}"
来源：http://tob.gzhubu.top

PHP:  number_format(1234567);
来源：http://xbd.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ucg.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qni.zhoulong.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hzo.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zjj.jinqigfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nuq.cheryme.top

C#:   1234567.ToString("N0")
来源：http://dlc.cashguo.top

[E17] 首字母大写
来源：http://git.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ons.52xcode.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hjk.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://epc.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wzw.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ozq.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iro.52xcode.cn

Ruby: s.capitalize
来源：http://uce.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qui.tanke756.top

[E18] 模板占位符替换
来源：http://qro.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dno.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kia.hongshengwenyu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ocx.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://elf.jiagoushi.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gmw.nwbrower.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eru.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ejs.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bzs.pycfn.com

[E19] 多行文本按行拆分
来源：http://ydw.hcnkem.com

Py:   s.splitlines()
来源：http://xvb.quarkkingdee.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://edd.hongshengwenyu.top

JS:   s.split(/\r?\n/)
来源：http://fbm.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://qbe.birdmap.top

Java: s.lines().toList()
来源：http://dht.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://pyw.pycfn.com

Ruby: s.lines
来源：http://ccv.yuxming.cn

C#:   s.Split('\n')
来源：http://uir.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://nhm.aizwys.cn

Py:   if not s:
来源：http://ymd.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gay.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gky.nanxinkj.top

TS:   if (s === "") {}
来源：http://kpz.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://uuy.gogol.net.cn

Go:   if s == "" {}
来源：http://buy.tianlin.xyz

Ruby: if s.empty?
来源：http://evp.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xhz.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://bpg.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://smz.xingfuxueyuan.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jnc.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wkw.ehwqpu.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gye.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://btq.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://cfd.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jme.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wbn.ehwqpu.com

[E22] 字节长度与字符长度
来源：http://aws.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rmi.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bko.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aay.yonumen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vdh.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://plh.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aul.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://zup.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jnb.yongpay.top

================================================================================
来源：http://uay.yongpay.top

F. 文件与目录
来源：http://jyj.ppjwa.cn

================================================================================
来源：http://ebb.xinyue.icu

[F01] 读取整个文件
来源：http://hvh.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rro.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://blt.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eag.dashuyun.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bnq.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://jjh.aizwys.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lbv.c1oappe.top

Ruby: File.read("a.txt")
来源：http://hua.hongshengwenyu.top

C#:   File.ReadAllText("a.txt");
来源：http://mkn.cdnleiting.top

[F02] 逐行读取文件
来源：http://yug.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fac.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yor.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vuy.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xoa.ybcxt.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://myj.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qdh.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cjo.pengpengdd.cyou

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gib.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://cxs.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dpl.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wre.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://inu.fktsv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://faj.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://poa.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zka.316326.xyz

Ruby: File.write("a.txt", "hi")
来源：http://nct.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xwh.gzhubu.top

[F04] 追加写入文件
来源：http://fxp.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://llb.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yxb.yj20258888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ztf.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zcg.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qbp.aibaodan.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://csa.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bvd.zhoulong.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wrw.jinghuilouyu.cn

[F05] 判断文件或目录是否存在
来源：http://jof.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sho.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://gwe.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://tgn.yj20258.top

TS:   fs.existsSync("a.txt")
来源：http://adb.bbcook.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aot.xylfe.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ylz.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://sdd.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://tku.shuidangran.top

[F06] 删除文件
来源：http://cfg.sweek.top

Py:   os.remove("a.txt")
来源：http://hej.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://kdt.zhixingplan.top

JS:   fs.unlinkSync("a.txt")
来源：http://qxe.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://gem.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://huo.yj202588.top

Go:   os.Remove("a.txt")
来源：http://xfb.sysykeji.top

Ruby: File.delete("a.txt")
来源：http://zff.havefunace.top

C#:   File.Delete("a.txt");
来源：http://gkm.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://zhw.jqgufenzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gxc.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qxu.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pbf.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kgf.316326.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pbo.yueranfly.top


<!-- 参考信息 -->