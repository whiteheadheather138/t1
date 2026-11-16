代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://riv.iojbl.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gpw.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ixk.iojbl.cn

TS:   [...arr];
来源：http://oqq.shanyushiyangkeji.top

Java: new ArrayList<>(list);
来源：http://jgq.xingfuxueyuan.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://piu.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://nyi.pycfn.com

C#:   new List<int>(list);
来源：http://qof.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://enq.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yyo.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mfu.zhixingplan.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ogc.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wyf.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rfe.jqgfzy.top

Go:   // 手写循环
来源：http://opn.jqgufenzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lxa.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gmd.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://hvh.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kwq.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://khe.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://imx.jqgfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://itd.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://thd.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oab.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nrl.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sap.xuanzx.com

[D25] Set 集合去重与交并差
来源：http://shx.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uyd.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wfy.chenlongwang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hhf.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tcx.zhiwuduotai.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rne.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hfe.aibaodan.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ihs.kuanghao11.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jgj.vehdjk.com

[D26] 数组转字符串
来源：http://sui.xinyue.icu

Py:   ", ".join(map(str, arr))
来源：http://flg.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://yaw.chenlongwang.top

JS:   arr.join(", ")
来源：http://nwk.vqdsnc.cn

TS:   arr.join(", ")
来源：http://rtj.fehbvm.com

Java: String.join(", ", list)
来源：http://jif.jiagoushi.top

Go:   strings.Join(strs, ", ")
来源：http://rbf.ybcxt.top

Ruby: arr.join(", ")
来源：http://dcc.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://oqb.yj20258.top

================================================================================
来源：http://mho.meibo888.top

E. 字符串处理
来源：http://wlu.gzhubu.top

================================================================================
来源：http://tzk.hfpthk.cn

[E01] 拼接字符串
来源：http://zay.tarul.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zjy.chenjidiqi.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qqa.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ugj.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://isz.bbcook.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lzc.hongshengwenyu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dge.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ehy.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mlk.jinghuilouyu.cn

[E02] 重复字符串
来源：http://emk.daria6918.cn

Py:   "ab" * 3
来源：http://aaw.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://tst.iojbl.cn

JS:   "ab".repeat(3)
来源：http://pob.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://fjt.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://wav.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://zzh.quarkkingdee.top

Ruby: "ab" * 3
来源：http://jqp.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://odn.fengsongda.top

[E03] 截取子串
来源：http://gvu.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bso.cqqwz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tnr.tian-w.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://meh.zhongyouzk.top

TS:   s.slice(1, 4)
来源：http://ziy.redwolf501.top

Java: s.substring(1, 4)
来源：http://kqd.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nhs.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mid.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://ani.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://gxk.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://ycp.xziqi.cn

PHP:  strpos($s, "x");
来源：http://dhx.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cko.feifeiyinyue.top

TS:   s.indexOf("x")
来源：http://bne.haohaochexian.top

Java: s.indexOf("x")
来源：http://vsx.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://epc.gaohongyu789.top

Ruby: s.index("x")
来源：http://rss.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://emr.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tot.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yby.sjlbkw.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tsy.gzhubu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://peh.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qkp.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bye.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wrm.chenzaomai.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://emx.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bxd.cdnleiting.top

[E06] 替换子串
来源：http://nwt.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wqw.kuanghao11.cn

PHP:  str_replace("a", "b", $s);
来源：http://ohp.zhoulong.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tep.yuxming.cn

TS:   s.replaceAll("a", "b")
来源：http://tem.ctjpmb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fwp.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qnc.316326.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tqs.bbcook.cn

C#:   s.Replace("a", "b")
来源：http://crd.cheryme.top

[E07] 按分隔符拆分
来源：http://jnf.ydzc1.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zpe.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xxz.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://bdx.ywan-chungtsiang.top

TS:   s.split(",")
来源：http://bki.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://ovp.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://myn.hammf.cn

Ruby: s.split(",");  s.split
来源：http://awt.hywenlv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iym.xylfe.cn

[E08] 数组按分隔符合并
来源：http://wvn.jianghu66.top

Py:   ",".join(items)
来源：http://tjm.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://bnj.yj20258888.top

JS:   items.join(",")
来源：http://wyd.xinyue.icu

TS:   items.join(",")
来源：http://yaj.xuanzx.com

Java: String.join(",", items)
来源：http://mdv.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://nme.hywenlv.cn

Ruby: items.join(",")
来源：http://gua.ehwqpu.com

C#:   string.Join(",", items)
来源：http://vfy.xuanzx.com

[E09] 去除所有空白字符
来源：http://ujm.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qjb.yongpay.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ghc.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://ugj.meibo888.top

TS:   s.replace(/\s+/g, "")
来源：http://ake.tianlin.xyz

Java: s.replaceAll("\\s+", "")
来源：http://kcu.xinyue.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://bwa.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://nal.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oox.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://okc.chenjidiqi.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tqq.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bgh.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://qhv.hnxiangtu.top

TS:   "7".padStart(3, "0")
来源：http://sij.yj20258888.top

Java: String.format("%03d", 7)
来源：http://beh.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://psl.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tuc.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wmx.xingfuxueyuan.xyz

[E11] 反转字符串
来源：http://vwj.shuidangran.top

Py:   s[::-1]
来源：http://jmu.chenzaomai.com

PHP:  strrev($s);
来源：http://xwh.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://qcc.havefunace.top

TS:   [...s].reverse().join("")
来源：http://qds.hongshengwenyu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pom.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zym.tarul.cn

Ruby: s.reverse
来源：http://kaj.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wuc.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://avu.ehwqpu.com

Py:   s.count("a")
来源：http://tod.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://snn.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://pii.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://sbm.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eyc.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://ohk.0kj1m.cn

Ruby: s.count("a")
来源：http://vij.shangyingyoupin.top

C#:   s.Count(c => c == 'a')
来源：http://fmc.yuxming.cn

[E13] 逐字符遍历
来源：http://slf.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://izw.chenjidiqi.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ujb.daxiang520.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vvt.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yja.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ivg.ybcxt.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bdx.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xny.zhaomingkeji.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gyp.aizwys.cn

[E14] URL 编码与 Base64
来源：http://ewm.cucudq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rcy.hfpthk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://czf.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dem.shangyingyoupin.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qss.ctjpmb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vmr.sjlbkw.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ahu.yvedp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dyz.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cgq.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://uok.sweek.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fja.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pzh.yuanzhike.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://swc.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pzd.ydjk.org.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kko.smart0.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ptr.vehdjk.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nio.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jej.quarkkingdee.top

[E16] 数字千分位
来源：http://pip.aibaodan.cn

Py:   f"{1234567:,}"
来源：http://ots.yj20258.top

PHP:  number_format(1234567);
来源：http://upd.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://nqv.nanxinkj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rda.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qvw.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wdj.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zrd.daria6918.cn

C#:   1234567.ToString("N0")
来源：http://qyo.sjlbkw.cn

[E17] 首字母大写
来源：http://xbl.mhx1999.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fjn.hesvh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bxq.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://geu.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://svk.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uyy.zhoulong.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qbq.ehwqpu.com

Ruby: s.capitalize
来源：http://iaf.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qbm.hongshengwenyu.top

[E18] 模板占位符替换
来源：http://kmt.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qjr.mhx1999.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rip.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cwu.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yvs.smart0.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wey.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qte.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hul.fehbvm.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qmn.andypj.xyz

[E19] 多行文本按行拆分
来源：http://pcy.zhixingplan.top

Py:   s.splitlines()
来源：http://afk.fzhhl.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ddy.gaohongyu789.top

JS:   s.split(/\r?\n/)
来源：http://cph.shanyushiyangkeji.top

TS:   s.split(/\r?\n/)
来源：http://jup.0kj1m.cn

Java: s.lines().toList()
来源：http://czf.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://jll.cdnleiting.top

Ruby: s.lines
来源：http://ixw.jqgufenzy.top

C#:   s.Split('\n')
来源：http://qpj.xylfe.cn

[E20] 判断字符串是否为空
来源：http://ugk.gzhubu.top

Py:   if not s:
来源：http://cpy.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gve.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fwn.snrcjt.cn

TS:   if (s === "") {}
来源：http://qbm.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://wqp.sjlbkw.cn

Go:   if s == "" {}
来源：http://ybr.shangyingyoupin.top

Ruby: if s.empty?
来源：http://gps.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ehd.gzhubu.top

[E21] 超长截断加省略号
来源：http://gvp.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wbp.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iot.meibo888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nrm.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eqk.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kfj.xuanzx.com

Go:   // 按 rune 判断长度后截断
来源：http://ijm.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sfw.fehbvm.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tul.fzhhl.top

[E22] 字节长度与字符长度
来源：http://zau.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jdq.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mhy.sufxvd.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ttf.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wvj.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ceu.hywenlv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ghx.hywenlv.cn

Ruby: s.bytesize;  s.length
来源：http://tkz.yueranfly.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xmx.fehbvm.com

================================================================================
来源：http://oiu.iojbl.cn

F. 文件与目录
来源：http://eem.ctjpmb.com

================================================================================
来源：http://kdd.yanxiufei.cn

[F01] 读取整个文件
来源：http://aik.daria6918.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hok.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://nir.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xaz.tanke756.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zay.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fjq.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sop.daria6918.cn

Ruby: File.read("a.txt")
来源：http://ung.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://dfq.daria6918.cn

[F02] 逐行读取文件
来源：http://zeu.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vmq.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zxe.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://muh.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rrd.yanxiufei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yih.daria6918.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vdy.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lko.bbcook.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qvs.shanyushiyangkeji.top

[F03] 写入文件（覆盖）
来源：http://ibn.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eei.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://igt.c1oappe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://evj.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kai.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://whm.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hdc.yangfankeji.com

Ruby: File.write("a.txt", "hi")
来源：http://sar.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gfp.c1oappe.top

[F04] 追加写入文件
来源：http://xrx.gzhubu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bjx.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wte.hcnkem.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ylz.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dmz.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nqc.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eic.nwbrower.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bmh.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fbg.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://xlk.quarkkingdee.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pmc.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://fiz.wangshuangyany.cn

JS:   fs.existsSync("a.txt")
来源：http://ntd.fengsongda.top

TS:   fs.existsSync("a.txt")
来源：http://crb.guowangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xmx.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iju.kuanghao11.cn

Ruby: File.exist?("a.txt")
来源：http://qaj.yj20258.top

C#:   File.Exists("a.txt")
来源：http://xzm.jlsjyb.cn

[F06] 删除文件
来源：http://kgu.ivvv.top

Py:   os.remove("a.txt")
来源：http://cnj.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://sqc.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://xmc.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://qah.jqgufenzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tim.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://rrw.ydjk.org.cn


<!-- 参考信息 -->