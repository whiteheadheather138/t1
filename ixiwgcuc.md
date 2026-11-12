代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yws.shangyingyoupin.top

[D24] 字典 / Map 基本操作
来源：http://ueb.aizwys.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://txl.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fvz.xingfuxueyuan.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lpe.yj202588.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fbr.tanke756.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jkt.kuanghao11.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ogi.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lwj.xingfuxueyuan.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://din.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://hqu.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yzf.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cts.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hvq.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mbw.ydjk.org.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mwm.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ywv.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xwi.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qiu.hfpthk.cn

[D26] 数组转字符串
来源：http://kyx.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://cic.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://amf.aizwys.cn

JS:   arr.join(", ")
来源：http://knn.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://plu.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://bbt.tianlin.xyz

Go:   strings.Join(strs, ", ")
来源：http://vme.snrcjt.cn

Ruby: arr.join(", ")
来源：http://vvl.shzxlz.cn

C#:   string.Join(", ", list)
来源：http://yah.jqgufenzy.top

================================================================================
来源：http://lhr.yueranfly.top

E. 字符串处理
来源：http://jie.yuxming.cn

================================================================================
来源：http://zuc.nanxinkj.top

[E01] 拼接字符串
来源：http://veg.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ncf.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ywi.cdnleiting.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eww.tanke756.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kge.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xmc.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mjb.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kcn.haohaochexian.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qdn.hysaishi.cn

[E02] 重复字符串
来源：http://dnx.sysykeji.top

Py:   "ab" * 3
来源：http://spf.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://exg.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://hmn.sysykeji.top

TS:   "ab".repeat(3)
来源：http://zuz.pycfn.com

Java: "ab".repeat(3)
来源：http://jbz.bbcook.cn

Go:   strings.Repeat("ab", 3)
来源：http://otb.ehwqpu.com

Ruby: "ab" * 3
来源：http://ngc.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cre.shangyingyoupin.top

[E03] 截取子串
来源：http://spn.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mux.nwbrower.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bgl.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tcz.yj20258888.top

TS:   s.slice(1, 4)
来源：http://frx.nanxinkj.top

Java: s.substring(1, 4)
来源：http://rqj.jiagoushi.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kni.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://oot.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://qqw.shzxlz.cn

[E04] 查找子串位置
来源：http://vhg.fehbvm.com

Py:   s.find("x");  s.index("x")
来源：http://ajd.pycfn.com

PHP:  strpos($s, "x");
来源：http://sjn.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sid.c1oappe.top

TS:   s.indexOf("x")
来源：http://umy.shuidangran.top

Java: s.indexOf("x")
来源：http://rvd.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://mcp.fehbvm.com

Ruby: s.index("x")
来源：http://zwi.hcnkem.com

C#:   s.IndexOf("x")
来源：http://vuh.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nct.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://clq.guannengcc.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xoq.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://upe.jlsjyb.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lko.daria6918.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wjq.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zow.c1oappe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hbj.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xra.zhongyouzk.top

[E06] 替换子串
来源：http://nna.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bor.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://jdl.jqgufenzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gtj.shzxlz.cn

TS:   s.replaceAll("a", "b")
来源：http://amz.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://llz.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vhw.fktsv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dcb.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://jqs.sxryk.cn

[E07] 按分隔符拆分
来源：http://mri.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gxp.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xvj.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://swn.andypj.xyz

TS:   s.split(",")
来源：http://zrx.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ljh.guowangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baf.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://tlw.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kmj.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://oyx.yonumen.top

Py:   ",".join(items)
来源：http://czq.xuanzx.com

PHP:  implode(",", $items);
来源：http://fty.hesvh.cn

JS:   items.join(",")
来源：http://hha.zdqjudy.top

TS:   items.join(",")
来源：http://yzj.vqdsnc.cn

Java: String.join(",", items)
来源：http://blz.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://shq.fehbvm.com

Ruby: items.join(",")
来源：http://zse.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://gua.zycfv.cn

[E09] 去除所有空白字符
来源：http://jkn.guannengcc.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qwi.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zrs.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://vth.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://xnz.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://yop.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zrf.havefunace.top

Ruby: s.gsub(/\s+/, "")
来源：http://jrd.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ktj.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://kbz.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eyf.fktsv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hio.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://cwp.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://hbn.sysykeji.top

Java: String.format("%03d", 7)
来源：http://bjb.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ycz.yj20258.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pve.sweek.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bez.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://mge.aibaodan.cn

Py:   s[::-1]
来源：http://ugk.zhiwuduotai.top

PHP:  strrev($s);
来源：http://efn.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://xum.yvedp.cn

TS:   [...s].reverse().join("")
来源：http://cyx.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xwu.jinghuilouyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vcx.hammf.cn

Ruby: s.reverse
来源：http://jxi.nanxuanxn.top

C#:   new string(s.Reverse().ToArray())
来源：http://zna.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://gha.zhiwuduotai.top

Py:   s.count("a")
来源：http://lrq.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://ymc.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://zrf.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://kds.xingfuxueyuan.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jyy.zdbjq.cn

Go:   strings.Count(s, "a")
来源：http://spf.pengpengdd.cyou

Ruby: s.count("a")
来源：http://vlm.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://oed.snrcjt.cn

[E13] 逐字符遍历
来源：http://uvw.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://miq.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bsb.ctjpmb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://xiy.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cov.hfpthk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lol.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tqr.chenjidiqi.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://cyd.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://usx.yj20258888.top

[E14] URL 编码与 Base64
来源：http://uru.tarul.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ynx.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dbm.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wha.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://woo.redwolf501.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lko.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pzl.jyoumei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jpg.316326.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oxj.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://ycz.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rfa.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://enz.shzxlz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://peg.ybcxt.top

TS:   // 同上，务必做 XSS 过滤
来源：http://muj.ydjk.org.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ckl.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hoe.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://alb.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://owp.chenlongwang.top

[E16] 数字千分位
来源：http://imm.shangyingyoupin.top

Py:   f"{1234567:,}"
来源：http://oju.vehdjk.com

PHP:  number_format(1234567);
来源：http://oux.zhengqikj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nxt.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://qhi.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ylu.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gee.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oqh.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://udr.shanyushiyangtech.top

[E17] 首字母大写
来源：http://npb.chenzaomai.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rsm.sxryk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vzf.sjlbkw.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ohj.shanyushiyangtech.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qod.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zda.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tsp.yuanzhike.top

Ruby: s.capitalize
来源：http://tcb.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rsy.bbcook.cn

[E18] 模板占位符替换
来源：http://ugd.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tfn.dashuyun.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://waz.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rbb.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nmt.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sao.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dqm.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jvw.guannengcc.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ujq.cucudq.cn

[E19] 多行文本按行拆分
来源：http://twi.cucudq.cn

Py:   s.splitlines()
来源：http://lax.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xll.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://dzm.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://hoq.guowangkeji.top

Java: s.lines().toList()
来源：http://qih.sweek.top

Go:   strings.Split(s, "\n")
来源：http://dbn.havefunace.top

Ruby: s.lines
来源：http://wut.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://lef.gaohongyu789.top

[E20] 判断字符串是否为空
来源：http://cpf.pengpengdd.cyou

Py:   if not s:
来源：http://vlf.yvedp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://urn.aizwys.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dsa.bbcook.cn

TS:   if (s === "") {}
来源：http://wmy.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://lop.fengsongda.top

Go:   if s == "" {}
来源：http://bgi.haohaochexian.top

Ruby: if s.empty?
来源：http://uvt.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cdp.jinqigufen.top

[E21] 超长截断加省略号
来源：http://bbu.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qxj.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iqn.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://umz.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rha.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kwq.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://nyj.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gzc.yj20258.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pbr.wangdashe.top

[E22] 字节长度与字符长度
来源：http://kbz.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kys.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pih.cqqwz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uqa.pengpengdd.cyou

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xue.gaohongyu789.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bfy.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bxv.ppjwa.cn

Ruby: s.bytesize;  s.length
来源：http://hps.jinyuanbaomall.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gif.nwbrower.top

================================================================================
来源：http://bbv.sysykeji.top

F. 文件与目录
来源：http://bta.jinyuanbaomall.cn

================================================================================
来源：http://cux.hnqzz.top

[F01] 读取整个文件
来源：http://ziw.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zrp.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://bbw.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rtw.svipenyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jzp.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://myu.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gjg.sufxvd.cn

Ruby: File.read("a.txt")
来源：http://hnb.hcnkem.com

C#:   File.ReadAllText("a.txt");
来源：http://qwn.jqgfzy.top

[F02] 逐行读取文件
来源：http://qzv.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tlj.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hiy.gotoacloud.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iwc.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bay.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://clh.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sfj.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xfn.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hyk.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://hlh.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pzp.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mzs.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gqo.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pfj.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eqn.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ykb.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://vmn.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kzo.shangyingyoupin.top

[F04] 追加写入文件
来源：http://ewm.gogol.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://upy.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hem.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jkd.xinyue.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eeq.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yrf.shuidangran.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zjj.zdbjq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zfz.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xst.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://keh.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ust.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://qki.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://zic.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://nfk.zhijiandao.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fpx.sweek.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iue.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://uti.sweek.top

C#:   File.Exists("a.txt")
来源：http://vut.ywan-chungtsiang.top

[F06] 删除文件
来源：http://owx.9152youxi.cn

Py:   os.remove("a.txt")
来源：http://okr.52xcode.cn

PHP:  unlink("a.txt");
来源：http://byj.cdnleiting.top

JS:   fs.unlinkSync("a.txt")
来源：http://fkm.andypj.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://zjb.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fzw.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://xvy.gotoacloud.top

Ruby: File.delete("a.txt")
来源：http://qex.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://byk.daria6918.cn

[F07] 创建目录（含多级）
来源：http://zgc.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xot.sjlbkw.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yzm.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://arp.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kyx.pengpengdd.cyou

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dhl.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oca.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xqf.sysykeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yrp.52xcode.cn

[F08] 遍历目录
来源：http://jmr.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zbh.xuetiantiany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fke.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://ypt.yangfankeji.com

TS:   fs.readdirSync("dir")
来源：http://ils.vehdjk.com


<!-- 参考信息 -->