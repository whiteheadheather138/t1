代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://zqg.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://wvn.epnwcf.com

JS:   arr.join(", ")
来源：http://zhi.9152youxi.cn

TS:   arr.join(", ")
来源：http://arg.tanke756.top

Java: String.join(", ", list)
来源：http://qtq.yuxming.cn

Go:   strings.Join(strs, ", ")
来源：http://shz.wangdashe.top

Ruby: arr.join(", ")
来源：http://kst.tarul.cn

C#:   string.Join(", ", list)
来源：http://zax.yvedp.cn

================================================================================
来源：http://mfb.uphjek.com

E. 字符串处理
来源：http://pyk.shzxlz.cn

================================================================================
来源：http://due.tarul.cn

[E01] 拼接字符串
来源：http://cqc.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bmb.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://spt.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vwo.feifeiyinyue.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yed.svipenyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mzy.zhixingplan.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yvz.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pid.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kes.zycfv.cn

[E02] 重复字符串
来源：http://bqa.fktsv.cn

Py:   "ab" * 3
来源：http://ddg.cashguo.top

PHP:  str_repeat("ab", 3);
来源：http://tdu.yvedp.cn

JS:   "ab".repeat(3)
来源：http://mwn.hnqzz.top

TS:   "ab".repeat(3)
来源：http://igv.yj202588.top

Java: "ab".repeat(3)
来源：http://qot.quarkkingdee.top

Go:   strings.Repeat("ab", 3)
来源：http://psz.ctjpmb.com

Ruby: "ab" * 3
来源：http://kjm.xinyue.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aht.jqgfzy.top

[E03] 截取子串
来源：http://cqs.hammf.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rsv.yuanzhike.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iqm.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cln.cashguo.top

TS:   s.slice(1, 4)
来源：http://gbt.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://wrl.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ana.xziqi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fyo.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://vhj.hcnkem.com

[E04] 查找子串位置
来源：http://uwo.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://rql.xziqi.cn

PHP:  strpos($s, "x");
来源：http://xhy.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ggs.andypj.xyz

TS:   s.indexOf("x")
来源：http://hwx.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://tke.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://edi.gotoacloud.top

Ruby: s.index("x")
来源：http://gxt.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://fvr.bjfxy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zgu.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nxd.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yxk.fengsongda.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bob.yj20258888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://opl.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wud.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jbq.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fkx.cdnleiting.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eyi.guannengcc.top

[E06] 替换子串
来源：http://aus.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ciq.bjfxy.top

PHP:  str_replace("a", "b", $s);
来源：http://oip.hongshengwenyu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zhh.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://xyw.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://roy.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dtr.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ftq.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://uww.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://fwe.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cyo.9152youxi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kcl.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ggz.yj20258.top

TS:   s.split(",")
来源：http://qhi.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tss.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xtb.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://oel.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wsy.cashguo.top

[E08] 数组按分隔符合并
来源：http://aaw.wangshuangyany.cn

Py:   ",".join(items)
来源：http://twh.hesvh.cn

PHP:  implode(",", $items);
来源：http://wzi.hywenlv.cn

JS:   items.join(",")
来源：http://tvs.ctjpmb.com

TS:   items.join(",")
来源：http://gre.jianghu66.top

Java: String.join(",", items)
来源：http://jur.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://jja.ehwqpu.com

Ruby: items.join(",")
来源：http://swt.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://nag.tarul.cn

[E09] 去除所有空白字符
来源：http://qyy.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cbr.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fvm.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://lqj.yangfankeji.com

TS:   s.replace(/\s+/g, "")
来源：http://frx.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://ebj.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://myj.mhx1999.top

Ruby: s.gsub(/\s+/, "")
来源：http://nok.snrcjt.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oju.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://ium.zhoulong.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://otl.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hus.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://hqk.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://bbc.zhiwuduotai.top

Java: String.format("%03d", 7)
来源：http://uwb.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://uve.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://naf.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nok.yj20258.top

[E11] 反转字符串
来源：http://kng.guannengcc.top

Py:   s[::-1]
来源：http://kaz.jiagoushi.top

PHP:  strrev($s);
来源：http://lmm.meibo888.top

JS:   [...s].reverse().join("")
来源：http://bim.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://uud.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zfi.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://idy.bbcook.cn

Ruby: s.reverse
来源：http://ufk.cashguo.top

C#:   new string(s.Reverse().ToArray())
来源：http://vqj.fktsv.cn

[E12] 统计某字符出现次数
来源：http://dsh.sufxvd.cn

Py:   s.count("a")
来源：http://fqt.zhengqikj.top

PHP:  substr_count($s, "a");
来源：http://fln.ivvv.top

JS:   s.split("a").length - 1
来源：http://asp.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://yxm.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tkg.vqdsnc.cn

Go:   strings.Count(s, "a")
来源：http://cjw.hongshengwenyu.top

Ruby: s.count("a")
来源：http://ysn.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://ejj.gogol.net.cn

[E13] 逐字符遍历
来源：http://tfi.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://bbx.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lhc.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gxv.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lte.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gog.52xcode.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oqx.zhengqikj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hyb.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://uoi.birdmap.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jpv.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yif.tarul.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lap.jqgfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://spn.jinqigufen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://exv.jinqigfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cdq.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bns.gaohongyu789.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nmm.dianchejie.cn

[E15] HTML 转义 / 反转义
来源：http://uqh.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://aje.gzhubu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cxf.redwolf501.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qlh.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lep.nwbrower.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mkf.jinghuilouyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jpy.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://exp.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://egf.hcnkem.com

[E16] 数字千分位
来源：http://gfv.cheryme.top

Py:   f"{1234567:,}"
来源：http://mfj.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://xtm.fehbvm.com

JS:   (1234567).toLocaleString("en-US")
来源：http://iks.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://htl.bbcook.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://emk.guannengcc.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vqc.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kzq.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://oof.hnxiangtu.top

[E17] 首字母大写
来源：http://asy.hongshengwenyu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nva.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://idy.yfazqb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nll.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fus.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qxu.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yjh.xylfe.cn

Ruby: s.capitalize
来源：http://bsw.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pwu.redwolf501.top

[E18] 模板占位符替换
来源：http://sti.daria6918.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vds.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cxh.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qiu.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gsj.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sip.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kgt.nwbrower.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dhd.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blo.yongpay.top

[E19] 多行文本按行拆分
来源：http://gcr.sufxvd.cn

Py:   s.splitlines()
来源：http://wrg.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gbq.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://tuf.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://xfv.tian-w.cn

Java: s.lines().toList()
来源：http://txo.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://dfz.hysaishi.cn

Ruby: s.lines
来源：http://syf.chenzaomai.com

C#:   s.Split('\n')
来源：http://sxn.jiagoushi.top

[E20] 判断字符串是否为空
来源：http://xep.kuanghao11.cn

Py:   if not s:
来源：http://ymi.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mcp.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xdc.jyoumei.cn

TS:   if (s === "") {}
来源：http://hed.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://wzz.shzxlz.cn

Go:   if s == "" {}
来源：http://bjj.sufxvd.cn

Ruby: if s.empty?
来源：http://waz.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ljw.gzhubu.top

[E21] 超长截断加省略号
来源：http://aqj.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bck.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yrv.haohaochexian.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kzs.zhengqikj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://acg.jyoumei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dlh.hfpthk.cn

Go:   // 按 rune 判断长度后截断
来源：http://tmv.hesvh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pur.hysaishi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fup.hammf.cn

[E22] 字节长度与字符长度
来源：http://pdn.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pzt.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://roi.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aaq.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ulp.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ozn.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mpw.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://vjp.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gyv.cheryme.top

================================================================================
来源：http://kce.jyoumei.cn

F. 文件与目录
来源：http://bdt.birdmap.top

================================================================================
来源：http://jof.tarul.cn

[F01] 读取整个文件
来源：http://yto.ywan-chungtsiang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lbn.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://elk.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oxb.sjlbkw.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wlu.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://txc.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dmz.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://smg.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://ghk.yfazqb.com

[F02] 逐行读取文件
来源：http://tho.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oar.jlsjyb.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vay.tian-w.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ifv.daxiang520.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ort.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gpt.svipenyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lpm.pengpengdd.cyou

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sfb.ctjpmb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gqz.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://ciq.cheryme.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yer.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://rtm.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dbr.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wxa.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bso.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mgl.zhongyouzk.top

Ruby: File.write("a.txt", "hi")
来源：http://lyh.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nle.gzhubu.top

[F04] 追加写入文件
来源：http://zfj.cdnleiting.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rrm.316326.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ell.fanxiaobao.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kpe.jinqigufen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xdu.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dee.hesvh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ats.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aly.nanxuanxn.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gnd.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://fwf.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vta.pycfn.com

PHP:  file_exists("a.txt");
来源：http://lnu.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://yov.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://cub.tian-w.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hai.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://upy.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://uhi.cheryme.top

C#:   File.Exists("a.txt")
来源：http://fjp.haohaochexian.top

[F06] 删除文件
来源：http://nwm.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://osa.yonumen.top

PHP:  unlink("a.txt");
来源：http://wdq.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://bmb.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://yqs.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qba.epnwcf.com

Go:   os.Remove("a.txt")
来源：http://sjg.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://liu.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://esz.ydzc1.top

[F07] 创建目录（含多级）
来源：http://cch.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://buy.ctjpmb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ovq.yvedp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xyw.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qlq.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qwy.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xnf.smart0.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jxx.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sve.jlsjyb.cn

[F08] 遍历目录
来源：http://usx.sjlbkw.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ooh.yanxiufei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wxw.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://nir.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://rhz.xuetiantiany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wwj.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xuc.havefunace.top

Ruby: Dir.children("dir")
来源：http://fub.chenlongwang.top

C#:   Directory.GetFiles("dir")
来源：http://xzz.zhoulong.xyz

[F09] 获取文件大小
来源：http://lnk.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://bit.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://sxf.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://nen.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://xgh.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nrv.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yjf.hongshengwenyu.top

Ruby: File.size("a.txt")
来源：http://ond.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://jwx.gogol.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://gfj.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://svn.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://spl.sxryk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vyz.shuidangran.top

TS:   path.extname("a.txt")
来源：http://nrv.9152youxi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mqr.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eol.tian-w.cn


<!-- 参考信息 -->