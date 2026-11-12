代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://kvk.yvedp.cn

JS:   arr.includes(x)
来源：http://dpp.nanxuanxn.top

TS:   arr.includes(x)
来源：http://mne.hammf.cn

Java: list.contains(x)
来源：http://mou.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://yjb.sweek.top

Ruby: arr.include?(x)
来源：http://ewi.yj20258888.top

C#:   list.Contains(x)
来源：http://gno.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://hxg.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zlm.daxiang520.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://giz.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ybh.daxiang520.top

TS:   [...arr];
来源：http://urq.iojbl.cn

Java: new ArrayList<>(list);
来源：http://ifo.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gsj.cucudq.cn

Ruby: arr.dup;  arr.clone
来源：http://csv.gotoacloud.top

C#:   new List<int>(list);
来源：http://dfd.0kj1m.cn

[D23] reduce 累积计算
来源：http://kib.shanyushiyangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pqk.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zpi.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://msf.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eaz.xziqi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zjy.jianghu66.top

Go:   // 手写循环
来源：http://ben.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oux.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://umr.nanxuanxn.top

[D24] 字典 / Map 基本操作
来源：http://mjw.0kj1m.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iwu.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cad.bjfxy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qot.uphjek.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eis.xylfe.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rjc.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eva.yonumen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ulu.zhengqikj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jcc.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://wjy.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yxp.tarul.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yec.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bkr.0kj1m.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fml.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uxr.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://whc.tanke756.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://amo.fzhhl.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://inv.snrcjt.cn

[D26] 数组转字符串
来源：http://lme.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://irw.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://mnt.yvedp.cn

JS:   arr.join(", ")
来源：http://rxb.wangshuangyany.cn

TS:   arr.join(", ")
来源：http://hvu.yanxiufei.cn

Java: String.join(", ", list)
来源：http://vzl.yj20258888.top

Go:   strings.Join(strs, ", ")
来源：http://gtq.fzhhl.top

Ruby: arr.join(", ")
来源：http://tff.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://chp.zhongyouzk.top

================================================================================
来源：http://bml.guowangkeji.top

E. 字符串处理
来源：http://tth.zdqjudy.top

================================================================================
来源：http://ikk.gotoacloud.top

[E01] 拼接字符串
来源：http://dya.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://peh.shanyushiyangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hay.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rwm.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mpl.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ksv.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lut.xylfe.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gjj.birdmap.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sys.guannengcc.top

[E02] 重复字符串
来源：http://saj.c1oappe.top

Py:   "ab" * 3
来源：http://doe.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://cia.yvedp.cn

JS:   "ab".repeat(3)
来源：http://rjc.hammf.cn

TS:   "ab".repeat(3)
来源：http://xcf.yongpay.top

Java: "ab".repeat(3)
来源：http://owa.vqdsnc.cn

Go:   strings.Repeat("ab", 3)
来源：http://jqr.yj20258.top

Ruby: "ab" * 3
来源：http://mrp.zhixingplan.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eve.hywenlv.cn

[E03] 截取子串
来源：http://gji.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bzp.vqdsnc.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fer.cashguo.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vvc.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://nlb.yuanzhike.top

Java: s.substring(1, 4)
来源：http://dfs.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zmi.quarkkingdee.top

Ruby: s[1, 3];  s[1..3]
来源：http://sfd.jianghu66.top

C#:   s.Substring(1, 3)
来源：http://yhn.tarul.cn

[E04] 查找子串位置
来源：http://rvu.jinqigufen.top

Py:   s.find("x");  s.index("x")
来源：http://jcc.fktsv.cn

PHP:  strpos($s, "x");
来源：http://ogp.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bwd.dianchejie.cn

TS:   s.indexOf("x")
来源：http://rhq.snrcjt.cn

Java: s.indexOf("x")
来源：http://qnk.smart0.xyz

Go:   strings.Index(s, "x")
来源：http://mhc.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://nzi.fzhhl.top

C#:   s.IndexOf("x")
来源：http://udj.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xzx.zdqjudy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ojt.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wpx.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ejw.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://gms.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xeb.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ygr.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eai.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://och.nwbrower.top

[E06] 替换子串
来源：http://aut.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oif.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://izk.yonumen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pje.zdbjq.cn

TS:   s.replaceAll("a", "b")
来源：http://clm.uphjek.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ger.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mwf.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qrp.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://nmi.pycfn.com

[E07] 按分隔符拆分
来源：http://adf.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qjt.jinghuilouyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://idg.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://nxt.chenlongwang.top

TS:   s.split(",")
来源：http://hbw.yangfankeji.com

Java: s.split(",");  s.split("\\s+")
来源：http://seo.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ebx.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://dos.cqqwz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wvj.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://rhr.jiagoushi.top

Py:   ",".join(items)
来源：http://rfc.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://vou.iojbl.cn

JS:   items.join(",")
来源：http://uyd.yangfankeji.com

TS:   items.join(",")
来源：http://dtt.ctjpmb.com

Java: String.join(",", items)
来源：http://vjo.xuetiantiany.cn

Go:   strings.Join(items, ",")
来源：http://kfb.cashguo.top

Ruby: items.join(",")
来源：http://ygf.xuanzx.com

C#:   string.Join(",", items)
来源：http://lif.xingfuxueyuan.xyz

[E09] 去除所有空白字符
来源：http://blp.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pwf.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mqz.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://ept.tarul.cn

TS:   s.replace(/\s+/g, "")
来源：http://nyp.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://hiq.nanxinkj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lzq.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://klf.hesvh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hjl.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://fla.zhijiandao.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://scu.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pwi.yuanzhike.top

JS:   "7".padStart(3, "0")
来源：http://ncg.daria6918.cn

TS:   "7".padStart(3, "0")
来源：http://yaz.sysykeji.top

Java: String.format("%03d", 7)
来源：http://yvn.fanxiaobao.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://qrb.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gnm.ywan-chungtsiang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qnn.shzxlz.cn

[E11] 反转字符串
来源：http://hyj.shzxlz.cn

Py:   s[::-1]
来源：http://fij.svipenyu.cn

PHP:  strrev($s);
来源：http://jwr.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://kwy.jyoumei.cn

TS:   [...s].reverse().join("")
来源：http://gbl.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uhp.tarul.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nah.guowangkeji.top

Ruby: s.reverse
来源：http://ght.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://orh.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://ivq.zhoulong.xyz

Py:   s.count("a")
来源：http://oex.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://emp.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://yyl.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://noz.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ewz.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://sfq.birdmap.top

Ruby: s.count("a")
来源：http://cfo.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://mxv.pengpengdd.cyou

[E13] 逐字符遍历
来源：http://zpw.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://fxu.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://exa.uphjek.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://vat.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yql.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://neo.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://umq.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ezm.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wtz.zhaomingkeji.xyz

[E14] URL 编码与 Base64
来源：http://byq.jinyuanbaomall.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fvp.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tno.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://goh.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bbv.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nwb.sysykeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tpp.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qlj.sjlbkw.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hia.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://foh.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vah.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cgx.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qtd.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ymd.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xxf.fanxiaobao.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rlw.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ftx.chenjidiqi.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ggi.hnxiangtu.top

[E16] 数字千分位
来源：http://egd.yj202588.top

Py:   f"{1234567:,}"
来源：http://fft.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://mhb.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://uxe.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://eds.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zmz.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cwb.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pqq.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://wrf.tian-w.cn

[E17] 首字母大写
来源：http://mcz.fktsv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nqp.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://gnn.smart0.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nib.guannengcc.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pfc.ydjk.org.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fcz.daria6918.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://elt.316326.xyz

Ruby: s.capitalize
来源：http://xya.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kfn.hammf.cn

[E18] 模板占位符替换
来源：http://wmk.tanke756.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ijp.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qnz.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bxo.uphjek.com

TS:   tpl.replaceAll("{name}", name)
来源：http://qfd.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ccc.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://njf.hysaishi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mvo.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ldz.yfazqb.com

[E19] 多行文本按行拆分
来源：http://ucz.vehdjk.com

Py:   s.splitlines()
来源：http://shk.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qtu.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://jbp.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://txq.uphjek.com

Java: s.lines().toList()
来源：http://cks.mhx1999.top

Go:   strings.Split(s, "\n")
来源：http://jnr.jianghu66.top

Ruby: s.lines
来源：http://whz.nanxuanxn.top

C#:   s.Split('\n')
来源：http://dsm.sweek.top

[E20] 判断字符串是否为空
来源：http://wiz.yonumen.top

Py:   if not s:
来源：http://ryv.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ktb.ppjwa.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vxw.zdqjudy.top

TS:   if (s === "") {}
来源：http://skf.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://ame.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://kgf.zhoulong.xyz

Ruby: if s.empty?
来源：http://zfm.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sgk.sweek.top

[E21] 超长截断加省略号
来源：http://vvf.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://olm.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bgp.jinqigfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kui.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vlh.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fya.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://xbf.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://avg.0kj1m.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hcx.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://ati.sjlbkw.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yrc.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://exf.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://plf.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hnc.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qjj.gzhubu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ien.shanyushiyangkeji.top

Ruby: s.bytesize;  s.length
来源：http://mxq.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zlw.jqgfzy.top

================================================================================
来源：http://xma.guowangkeji.top

F. 文件与目录
来源：http://glv.chenjidiqi.icu

================================================================================
来源：http://skz.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://ixj.fengsongda.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://trv.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://weh.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bap.316326.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gvs.xziqi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tjs.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mha.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://esv.sxryk.cn

C#:   File.ReadAllText("a.txt");
来源：http://wmr.zhengqikj.top

[F02] 逐行读取文件
来源：http://ygy.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rme.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pfw.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wke.zhaomingkeji.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gxc.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wwu.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pbh.shzxlz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iff.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fvo.yuanzhike.top

[F03] 写入文件（覆盖）
来源：http://kve.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nkh.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ynb.haohaochexian.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://psc.fengsongda.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hpp.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bws.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nfx.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://zzd.vqdsnc.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yca.shangyingyoupin.top

[F04] 追加写入文件
来源：http://eye.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nwy.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qgj.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hld.hammf.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sia.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vli.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ohu.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yff.cqqwz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fxp.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://fxn.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xir.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://gwi.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://phc.yfazqb.com

TS:   fs.existsSync("a.txt")
来源：http://aqp.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rgd.gaohongyu789.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ytz.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://hcw.ydjk.org.cn


<!-- 参考信息 -->