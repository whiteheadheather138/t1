代发 wailian999

================================================================================
来源：http://taq.hywenlv.cn

E. 字符串处理
来源：http://hbf.zdbjq.cn

================================================================================
来源：http://lna.vehdjk.com

[E01] 拼接字符串
来源：http://pjj.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nna.pengpengdd.cyou

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://alo.smart0.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://llx.xinyue.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ceb.zycfv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://djw.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zef.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ckd.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vwi.ppjwa.cn

[E02] 重复字符串
来源：http://oxp.shanyushiyangkeji.top

Py:   "ab" * 3
来源：http://ifh.yangfankeji.com

PHP:  str_repeat("ab", 3);
来源：http://pmn.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://miw.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://vos.cashguo.top

Java: "ab".repeat(3)
来源：http://dxu.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://rhk.dianchejie.cn

Ruby: "ab" * 3
来源：http://vnr.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rqd.pengpengdd.cyou

[E03] 截取子串
来源：http://ttz.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pqm.yongpay.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pka.tanke756.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aad.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://imt.gogol.net.cn

Java: s.substring(1, 4)
来源：http://rjm.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://may.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://qoz.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://dxs.yanxiufei.cn

[E04] 查找子串位置
来源：http://bay.nwbrower.top

Py:   s.find("x");  s.index("x")
来源：http://uuv.hfpthk.cn

PHP:  strpos($s, "x");
来源：http://law.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kdl.birdmap.top

TS:   s.indexOf("x")
来源：http://vhk.epnwcf.com

Java: s.indexOf("x")
来源：http://qeq.mhx1999.top

Go:   strings.Index(s, "x")
来源：http://cvc.9152youxi.cn

Ruby: s.index("x")
来源：http://gpo.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://eeh.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bup.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gtr.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ryd.wangshuangyany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://psv.xingfuxueyuan.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://wzo.aibaodan.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cym.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rkq.tianlin.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nwa.shangyingyoupin.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dwm.hysaishi.cn

[E06] 替换子串
来源：http://dgt.hywenlv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cvq.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://hru.jinqigufen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rlp.uphjek.com

TS:   s.replaceAll("a", "b")
来源：http://jvg.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hop.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ukl.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fzi.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://dhy.gotoacloud.top

[E07] 按分隔符拆分
来源：http://ubi.sjlbkw.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ont.meibo888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ire.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://auv.sweek.top

TS:   s.split(",")
来源：http://qyu.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://rkv.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bem.ywan-chungtsiang.top

Ruby: s.split(",");  s.split
来源：http://jva.yj202588.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://paz.vehdjk.com

[E08] 数组按分隔符合并
来源：http://vae.andypj.xyz

Py:   ",".join(items)
来源：http://atq.hywenlv.cn

PHP:  implode(",", $items);
来源：http://dvj.jinghuilouyu.cn

JS:   items.join(",")
来源：http://pbs.vqdsnc.cn

TS:   items.join(",")
来源：http://dxj.hesvh.cn

Java: String.join(",", items)
来源：http://hdw.yj202588.top

Go:   strings.Join(items, ",")
来源：http://bhj.hesvh.cn

Ruby: items.join(",")
来源：http://jcd.daxiang520.top

C#:   string.Join(",", items)
来源：http://plg.316326.xyz

[E09] 去除所有空白字符
来源：http://bqf.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oij.xziqi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://euv.vqdsnc.cn

JS:   s.replace(/\s+/g, "")
来源：http://muu.iojbl.cn

TS:   s.replace(/\s+/g, "")
来源：http://keh.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://thk.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rci.guowangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://mqd.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fkg.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://isc.ydjk.org.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nng.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nki.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://nim.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://ozh.yj202588.top

Java: String.format("%03d", 7)
来源：http://vky.yj202588.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jru.zhaomingkeji.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://shr.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pbu.bbcook.cn

[E11] 反转字符串
来源：http://psc.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://wxf.yuxming.cn

PHP:  strrev($s);
来源：http://zzp.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://wdv.ivvv.top

TS:   [...s].reverse().join("")
来源：http://nbu.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://qbz.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tcn.9152youxi.cn

Ruby: s.reverse
来源：http://mzn.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://ujf.fzhhl.top

[E12] 统计某字符出现次数
来源：http://voi.zycfv.cn

Py:   s.count("a")
来源：http://rja.hesvh.cn

PHP:  substr_count($s, "a");
来源：http://frq.gaohongyu789.top

JS:   s.split("a").length - 1
来源：http://ohp.zhoulong.xyz

TS:   s.split("a").length - 1
来源：http://lss.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://moy.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://oml.ybcxt.top

Ruby: s.count("a")
来源：http://zcu.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://fta.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://zfe.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://jdz.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lgi.jinghuilouyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rlo.jianghu66.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xpj.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zov.zhoulong.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cnl.xuanzx.com

Ruby: s.each_char { |ch| puts ch }
来源：http://bwt.xziqi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lpc.sufxvd.cn

[E14] URL 编码与 Base64
来源：http://iuu.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uax.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kpa.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nfe.havefunace.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eqj.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vpd.shanyushiyangtech.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gwu.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qxw.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jsz.sysykeji.top

[E15] HTML 转义 / 反转义
来源：http://nkc.fengsongda.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gls.hfpthk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pcb.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://plb.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rjv.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://akc.snrcjt.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nld.feifeiyinyue.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hcp.chenlongwang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://leg.jianghu66.top

[E16] 数字千分位
来源：http://lfj.dashuyun.cn

Py:   f"{1234567:,}"
来源：http://zjd.dianchejie.cn

PHP:  number_format(1234567);
来源：http://psf.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tst.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://dmg.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://scw.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jos.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fax.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://pzp.fzhhl.top

[E17] 首字母大写
来源：http://lzc.daria6918.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mqp.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mmr.iojbl.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://txc.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hqg.aibaodan.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wkq.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://llq.jqgufenzy.top

Ruby: s.capitalize
来源：http://fmi.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yyx.jinqigufen.top

[E18] 模板占位符替换
来源：http://mkf.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jwj.9152youxi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ofb.svipenyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zzu.fanxiaobao.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://hxz.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bqu.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ezu.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zty.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hzi.hesvh.cn

[E19] 多行文本按行拆分
来源：http://twt.xingfuxueyuan.xyz

Py:   s.splitlines()
来源：http://sjo.pengpengdd.cyou

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://klf.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://apd.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://bry.havefunace.top

Java: s.lines().toList()
来源：http://zmq.jinqigufen.top

Go:   strings.Split(s, "\n")
来源：http://mxy.yj20258.top

Ruby: s.lines
来源：http://nap.kuanghao11.cn

C#:   s.Split('\n')
来源：http://ayo.0kj1m.cn

[E20] 判断字符串是否为空
来源：http://xdp.jinqigfzy.top

Py:   if not s:
来源：http://whe.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ojk.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eyr.tarul.cn

TS:   if (s === "") {}
来源：http://lhs.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://xql.sweek.top

Go:   if s == "" {}
来源：http://rng.shanyushiyangkeji.top

Ruby: if s.empty?
来源：http://ylz.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://npl.sweek.top

[E21] 超长截断加省略号
来源：http://xsw.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ern.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xhg.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rkm.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ygd.ydzc1.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ydt.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://bor.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://evx.xingfuxueyuan.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uqg.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://tmh.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jrd.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fvt.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fhq.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bek.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://msv.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ujd.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://qrs.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://phe.hfpthk.cn

================================================================================
来源：http://vdr.zhixingplan.top

F. 文件与目录
来源：http://tok.ywan-chungtsiang.top

================================================================================
来源：http://ejd.fengsongda.top

[F01] 读取整个文件
来源：http://utx.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://phr.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://yph.kuanghao11.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nps.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wun.ydzc1.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rht.nanxinkj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wvt.yj20258888.top

Ruby: File.read("a.txt")
来源：http://lii.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://jdg.aizwys.cn

[F02] 逐行读取文件
来源：http://tih.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qlj.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vvm.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qxa.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wda.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kbd.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gpp.shzxlz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yzp.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wcv.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://air.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kdl.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zcd.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aul.xuanzx.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://umg.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hze.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://szf.dashuyun.cn

Ruby: File.write("a.txt", "hi")
来源：http://dcg.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zly.yj202588.top

[F04] 追加写入文件
来源：http://whv.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zue.sxryk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zki.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://avt.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vay.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lpv.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://piw.xinyue.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lip.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yke.jlsjyb.cn

[F05] 判断文件或目录是否存在
来源：http://rln.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iyl.smart0.xyz

PHP:  file_exists("a.txt");
来源：http://rje.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://yyo.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://raf.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ffb.zhengqikj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://edf.guannengcc.top

Ruby: File.exist?("a.txt")
来源：http://hfb.hywenlv.cn

C#:   File.Exists("a.txt")
来源：http://ila.jinqigfzy.top

[F06] 删除文件
来源：http://ery.redwolf501.top

Py:   os.remove("a.txt")
来源：http://ffk.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://fan.sxryk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eup.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://pam.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://muu.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://wde.hywenlv.cn

Ruby: File.delete("a.txt")
来源：http://auj.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://ggs.yuxming.cn

[F07] 创建目录（含多级）
来源：http://nqn.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iru.yongpay.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gkz.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wro.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fet.haohaochexian.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://siq.chenlongwang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ydt.haohaochexian.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xvj.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://slf.yfazqb.com

[F08] 遍历目录
来源：http://ghr.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nce.meibo888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zba.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://aic.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://rjv.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iqq.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zuc.yueranfly.top

Ruby: Dir.children("dir")
来源：http://hmg.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://olj.guowangkeji.top

[F09] 获取文件大小
来源：http://jht.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://due.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://txd.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://vrh.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://jly.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yxk.mhx1999.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://srq.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://ngm.cashguo.top

C#:   new FileInfo("a.txt").Length
来源：http://raj.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://jxk.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uxy.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://egb.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tai.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://eca.sxryk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://grn.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jzr.xuanzx.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gxp.redwolf501.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bzu.fehbvm.com

[F11] 复制与移动文件
来源：http://cko.hcnkem.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ssi.tian-w.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iec.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ypk.hywenlv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pml.ywan-chungtsiang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qgv.vehdjk.com


<!-- 参考信息 -->