代发 wailian999

================================================================================
来源：http://mca.aibaodan.cn

E. 字符串处理
来源：http://huc.daxiang520.top

================================================================================
来源：http://ccw.bbcook.cn

[E01] 拼接字符串
来源：http://dxy.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qav.bjfxy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vwg.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bwm.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ynq.feifeiyinyue.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://prf.hnqzz.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://etu.sufxvd.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dcf.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fjq.bbcook.cn

[E02] 重复字符串
来源：http://qfn.yuanzhike.top

Py:   "ab" * 3
来源：http://zmb.hysaishi.cn

PHP:  str_repeat("ab", 3);
来源：http://ayl.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://mfb.ppjwa.cn

TS:   "ab".repeat(3)
来源：http://rkj.daria6918.cn

Java: "ab".repeat(3)
来源：http://sde.jlsjyb.cn

Go:   strings.Repeat("ab", 3)
来源：http://eyz.jiagoushi.top

Ruby: "ab" * 3
来源：http://tbm.yangfankeji.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fyw.epnwcf.com

[E03] 截取子串
来源：http://fyt.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ndj.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lut.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wuy.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://yzm.gzhubu.top

Java: s.substring(1, 4)
来源：http://nhi.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yue.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://iob.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://fqn.aizwys.cn

[E04] 查找子串位置
来源：http://rse.yueranfly.top

Py:   s.find("x");  s.index("x")
来源：http://vom.xziqi.cn

PHP:  strpos($s, "x");
来源：http://mey.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://enf.birdmap.top

TS:   s.indexOf("x")
来源：http://gmq.hnqzz.top

Java: s.indexOf("x")
来源：http://jtj.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://ybp.yj20258.top

Ruby: s.index("x")
来源：http://fih.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://ssq.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mbo.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ppz.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nfn.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cct.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hvt.jqgfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mrj.316326.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sha.jqgufenzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://asx.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vkv.redwolf501.top

[E06] 替换子串
来源：http://sje.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://spf.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://tog.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bwb.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://nkr.fzhhl.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://skm.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rnc.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fon.zhoulong.xyz

C#:   s.Replace("a", "b")
来源：http://hnd.52xcode.cn

[E07] 按分隔符拆分
来源：http://zak.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tir.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oln.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rls.ydjk.org.cn

TS:   s.split(",")
来源：http://gjl.cashguo.top

Java: s.split(",");  s.split("\\s+")
来源：http://djq.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ale.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://bnn.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gsk.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://dwn.cucudq.cn

Py:   ",".join(items)
来源：http://uun.jyoumei.cn

PHP:  implode(",", $items);
来源：http://syk.yonumen.top

JS:   items.join(",")
来源：http://cqo.feifeiyinyue.top

TS:   items.join(",")
来源：http://sak.tianlin.xyz

Java: String.join(",", items)
来源：http://anb.nanxinkj.top

Go:   strings.Join(items, ",")
来源：http://fpw.wangdashe.top

Ruby: items.join(",")
来源：http://iay.hongshengwenyu.top

C#:   string.Join(",", items)
来源：http://jnx.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://gcv.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gli.shuidangran.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qcr.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://crm.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://vur.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://lja.shuidangran.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ria.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cuo.cqqwz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wuy.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://gmn.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xvw.guowangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gna.shzxlz.cn

JS:   "7".padStart(3, "0")
来源：http://vhf.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://opp.jinghuilouyu.cn

Java: String.format("%03d", 7)
来源：http://ong.shangyingyoupin.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://olz.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vys.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ajm.smart0.xyz

[E11] 反转字符串
来源：http://bta.yfazqb.com

Py:   s[::-1]
来源：http://jew.shanyushiyangkeji.top

PHP:  strrev($s);
来源：http://oge.fehbvm.com

JS:   [...s].reverse().join("")
来源：http://aow.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://hvh.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://otx.snrcjt.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tze.uphjek.com

Ruby: s.reverse
来源：http://kwm.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://pgm.c1oappe.top

[E12] 统计某字符出现次数
来源：http://jar.kuanghao11.cn

Py:   s.count("a")
来源：http://oop.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://cue.yongpay.top

JS:   s.split("a").length - 1
来源：http://huy.haohaochexian.top

TS:   s.split("a").length - 1
来源：http://lyu.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oeg.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://jvf.xinyue.icu

Ruby: s.count("a")
来源：http://izn.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://baj.ydzc1.top

[E13] 逐字符遍历
来源：http://hlh.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://orb.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ttu.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://zry.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bky.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oes.vqdsnc.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rgg.hywenlv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://crb.fzhhl.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jsp.birdmap.top

[E14] URL 编码与 Base64
来源：http://exj.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qxm.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://plc.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nyk.svipenyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hap.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://weq.wangshuangyany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eob.zhaomingkeji.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dlu.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bjr.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://fem.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://iyt.birdmap.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gvp.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vyx.xuanzx.com

TS:   // 同上，务必做 XSS 过滤
来源：http://ahy.bjfxy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cbe.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rns.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dpx.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uka.snrcjt.cn

[E16] 数字千分位
来源：http://rhz.tanke756.top

Py:   f"{1234567:,}"
来源：http://slg.zhijiandao.cn

PHP:  number_format(1234567);
来源：http://bbs.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wcr.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://wlw.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://scb.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ccj.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sxe.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://cch.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://wnt.kuanghao11.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pxh.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qce.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fur.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ghc.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cxp.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lfy.daria6918.cn

Ruby: s.capitalize
来源：http://fdj.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xft.zhiwuduotai.top

[E18] 模板占位符替换
来源：http://tfy.zhixingplan.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mzi.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gnw.0kj1m.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dzl.zhoulong.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://ufe.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://klt.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ubz.wangdashe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pni.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cma.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://uyr.aibaodan.cn

Py:   s.splitlines()
来源：http://xiw.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uuy.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://olv.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://wls.c1oappe.top

Java: s.lines().toList()
来源：http://rle.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://plx.shuidangran.top

Ruby: s.lines
来源：http://chq.jinyuanbaomall.cn

C#:   s.Split('\n')
来源：http://dio.guannengcc.top

[E20] 判断字符串是否为空
来源：http://zoc.hnqzz.top

Py:   if not s:
来源：http://bqo.havefunace.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sve.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hfu.ehwqpu.com

TS:   if (s === "") {}
来源：http://qpi.hesvh.cn

Java: if (s.isEmpty()) {}
来源：http://gvy.hywenlv.cn

Go:   if s == "" {}
来源：http://ccj.hnqzz.top

Ruby: if s.empty?
来源：http://evy.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jrq.andypj.xyz

[E21] 超长截断加省略号
来源：http://ket.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sqt.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://txd.zdbjq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kgp.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lpk.ydzc1.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://msb.snrcjt.cn

Go:   // 按 rune 判断长度后截断
来源：http://vid.havefunace.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pgx.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eza.jinyuanbaomall.cn

[E22] 字节长度与字符长度
来源：http://dsy.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uwz.dianchejie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hoq.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fcp.ydjk.org.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hle.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uja.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tia.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://npm.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ckb.jyoumei.cn

================================================================================
来源：http://ydt.52xcode.cn

F. 文件与目录
来源：http://sem.fktsv.cn

================================================================================
来源：http://chr.yongpay.top

[F01] 读取整个文件
来源：http://eep.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dxf.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://aui.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://syo.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cfa.jyoumei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hiz.wangdashe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ncy.shuidangran.top

Ruby: File.read("a.txt")
来源：http://ibq.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://kyw.yj20258888.top

[F02] 逐行读取文件
来源：http://qlc.chenjidiqi.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vph.cdnleiting.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://elm.sxryk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ita.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yya.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://snf.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oqx.sufxvd.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ibq.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lav.nanxinkj.top

[F03] 写入文件（覆盖）
来源：http://bjr.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pxd.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pfl.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wpw.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jms.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dto.9152youxi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tlr.sweek.top

Ruby: File.write("a.txt", "hi")
来源：http://tze.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fgn.havefunace.top

[F04] 追加写入文件
来源：http://rec.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ghe.hcnkem.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eag.chenzaomai.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oro.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lfh.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fan.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tfj.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rax.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dyp.jlsjyb.cn

[F05] 判断文件或目录是否存在
来源：http://qgd.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qsb.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://ptf.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://ytw.jinghuilouyu.cn

TS:   fs.existsSync("a.txt")
来源：http://psu.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nxh.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ulp.bjfxy.top

Ruby: File.exist?("a.txt")
来源：http://hrw.jinyuanbaomall.cn

C#:   File.Exists("a.txt")
来源：http://utc.cdnleiting.top

[F06] 删除文件
来源：http://gyd.hesvh.cn

Py:   os.remove("a.txt")
来源：http://cwi.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://ltd.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pgb.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://xye.yuxming.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dgv.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://hbe.xinyue.icu

Ruby: File.delete("a.txt")
来源：http://fnf.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://wpw.xziqi.cn

[F07] 创建目录（含多级）
来源：http://oyb.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yiq.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gtf.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ntt.sufxvd.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://klr.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lim.c1oappe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zei.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cug.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rnm.chenjidiqi.icu

[F08] 遍历目录
来源：http://kws.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://emr.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jsj.wangshuangyany.cn

JS:   fs.readdirSync("dir")
来源：http://nhj.vqdsnc.cn

TS:   fs.readdirSync("dir")
来源：http://rwa.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gkb.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ajw.52xcode.cn

Ruby: Dir.children("dir")
来源：http://mkz.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://lyw.cheryme.top

[F09] 获取文件大小
来源：http://qii.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://cia.zhongyouzk.top

PHP:  filesize("a.txt");
来源：http://lgm.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://qal.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://qrh.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wjx.fzhhl.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xdd.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://xnv.aizwys.cn

C#:   new FileInfo("a.txt").Length
来源：http://pec.daria6918.cn

[F10] 取文件扩展名 / 文件名
来源：http://duy.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mnf.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kob.tanke756.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uhi.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://tth.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rbf.fanxiaobao.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sdj.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mkm.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bcn.jiagoushi.top

[F11] 复制与移动文件
来源：http://bmw.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ssz.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ett.cqqwz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://szn.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pvi.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pqx.jyoumei.cn


<!-- 参考信息 -->