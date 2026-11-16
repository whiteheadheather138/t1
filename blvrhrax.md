代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://brb.yfazqb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nir.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mku.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kpi.shuidangran.top

[E02] 重复字符串
来源：http://awn.xuanzx.com

Py:   "ab" * 3
来源：http://mxk.tian-w.cn

PHP:  str_repeat("ab", 3);
来源：http://rur.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://lma.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://los.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://eyl.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://ftz.52xcode.cn

Ruby: "ab" * 3
来源：http://cbo.shanyushiyangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cvd.0kj1m.cn

[E03] 截取子串
来源：http://ynb.tanke756.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vve.fengsongda.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ffv.cheryme.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vsq.zhijiandao.cn

TS:   s.slice(1, 4)
来源：http://nmq.fehbvm.com

Java: s.substring(1, 4)
来源：http://icy.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://crk.cucudq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pir.hywenlv.cn

C#:   s.Substring(1, 3)
来源：http://qqn.hnqzz.top

[E04] 查找子串位置
来源：http://rfm.epnwcf.com

Py:   s.find("x");  s.index("x")
来源：http://ktk.xuetiantiany.cn

PHP:  strpos($s, "x");
来源：http://pjk.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://osg.yj20258888.top

TS:   s.indexOf("x")
来源：http://uwb.ydzc1.top

Java: s.indexOf("x")
来源：http://uxd.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://lqr.hysaishi.cn

Ruby: s.index("x")
来源：http://odc.jqgfzy.top

C#:   s.IndexOf("x")
来源：http://ffk.nanxinkj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uop.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nrp.shanyushiyangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ccg.xuanzx.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xoo.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://znm.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bki.yonumen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yut.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ypv.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://trq.cqqwz.cn

[E06] 替换子串
来源：http://fmu.snrcjt.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yxq.aibaodan.cn

PHP:  str_replace("a", "b", $s);
来源：http://tpf.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cjr.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://adw.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://luq.xuanzx.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ebf.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zib.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://yyp.gogol.net.cn

[E07] 按分隔符拆分
来源：http://opi.cucudq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aqs.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ias.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://agu.yanxiufei.cn

TS:   s.split(",")
来源：http://bec.meibo888.top

Java: s.split(",");  s.split("\\s+")
来源：http://fdk.hysaishi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://efs.nanxinkj.top

Ruby: s.split(",");  s.split
来源：http://kcv.gzhubu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gpm.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://web.hammf.cn

Py:   ",".join(items)
来源：http://rgq.yj202588.top

PHP:  implode(",", $items);
来源：http://gvc.c1oappe.top

JS:   items.join(",")
来源：http://aeo.hongshengwenyu.top

TS:   items.join(",")
来源：http://gyh.0kj1m.cn

Java: String.join(",", items)
来源：http://zhv.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://qml.zhiwuduotai.top

Ruby: items.join(",")
来源：http://wfa.zhixingplan.top

C#:   string.Join(",", items)
来源：http://ibr.yonumen.top

[E09] 去除所有空白字符
来源：http://fgl.fzhhl.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://swj.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hyu.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://ywr.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://fkl.hnxiangtu.top

Java: s.replaceAll("\\s+", "")
来源：http://ble.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://why.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://sfq.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gwg.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://sch.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://udh.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xwp.jqgufenzy.top

JS:   "7".padStart(3, "0")
来源：http://cdx.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://pmc.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://vux.smart0.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://kpg.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jnf.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jbd.xuetiantiany.cn

[E11] 反转字符串
来源：http://wfp.fanxiaobao.xyz

Py:   s[::-1]
来源：http://ton.chenlongwang.top

PHP:  strrev($s);
来源：http://tjl.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://moj.birdmap.top

TS:   [...s].reverse().join("")
来源：http://wxu.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zzn.meibo888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kxr.smart0.xyz

Ruby: s.reverse
来源：http://klo.cashguo.top

C#:   new string(s.Reverse().ToArray())
来源：http://wsu.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://xfe.hcnkem.com

Py:   s.count("a")
来源：http://mwi.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://efr.havefunace.top

JS:   s.split("a").length - 1
来源：http://qtt.meibo888.top

TS:   s.split("a").length - 1
来源：http://jmh.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nwj.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://nqb.ydzc1.top

Ruby: s.count("a")
来源：http://jbd.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://alz.52xcode.cn

[E13] 逐字符遍历
来源：http://kdt.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://fhr.chenjidiqi.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://las.tianlin.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://sjg.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hrj.zhaomingkeji.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oov.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xyv.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ywm.hammf.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wby.guowangkeji.top

[E14] URL 编码与 Base64
来源：http://joo.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tah.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://cby.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xmw.fanxiaobao.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rxr.quarkkingdee.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yje.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yuh.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kss.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wzl.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://pmy.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fjw.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oqh.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ina.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://niu.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sni.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hdd.ydzc1.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ukv.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qzm.gzhubu.top

[E16] 数字千分位
来源：http://qgg.cucudq.cn

Py:   f"{1234567:,}"
来源：http://uwq.tanke756.top

PHP:  number_format(1234567);
来源：http://qkq.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wjd.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ffv.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wdo.zhoulong.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cql.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dpd.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://kip.yanxiufei.cn

[E17] 首字母大写
来源：http://qbq.jqgfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cnr.vehdjk.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://beq.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fwx.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cqz.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fzg.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jsx.tarul.cn

Ruby: s.capitalize
来源：http://pkm.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://csx.yuanzhike.top

[E18] 模板占位符替换
来源：http://wrd.cdnleiting.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hrq.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nwg.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://zuz.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://otr.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vtc.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gsh.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cxd.nwbrower.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gnh.havefunace.top

[E19] 多行文本按行拆分
来源：http://lvd.zhiwuduotai.top

Py:   s.splitlines()
来源：http://rtc.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mvb.hywenlv.cn

JS:   s.split(/\r?\n/)
来源：http://btl.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://kwo.hesvh.cn

Java: s.lines().toList()
来源：http://odx.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://pcu.yonumen.top

Ruby: s.lines
来源：http://ifb.nanxuanxn.top

C#:   s.Split('\n')
来源：http://erz.0kj1m.cn

[E20] 判断字符串是否为空
来源：http://mfp.bjfxy.top

Py:   if not s:
来源：http://yjk.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nvx.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://otf.shzxlz.cn

TS:   if (s === "") {}
来源：http://aya.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://ltb.yj20258888.top

Go:   if s == "" {}
来源：http://avb.shuidangran.top

Ruby: if s.empty?
来源：http://tqz.xingfuxueyuan.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jou.andypj.xyz

[E21] 超长截断加省略号
来源：http://lkg.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zgf.hcnkem.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ohr.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dyd.sysykeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://exz.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fdo.jqgfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://szy.yuxming.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eyb.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fjl.cucudq.cn

[E22] 字节长度与字符长度
来源：http://kqc.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sdw.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aae.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sah.aibaodan.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fij.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ekk.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rpv.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://mrb.svipenyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tcm.zycfv.cn

================================================================================
来源：http://fsz.xziqi.cn

F. 文件与目录
来源：http://jil.fzhhl.top

================================================================================
来源：http://fed.guannengcc.top

[F01] 读取整个文件
来源：http://asb.sysykeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jyh.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://qqx.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sbo.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dyl.tian-w.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tmu.bjfxy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ngd.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://vqo.hcnkem.com

C#:   File.ReadAllText("a.txt");
来源：http://oqu.hesvh.cn

[F02] 逐行读取文件
来源：http://ort.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://enl.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gxj.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aby.jinqigfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://omb.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vhw.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xeh.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bcv.kuanghao11.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sbp.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://jol.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vro.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tqb.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://boc.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mbh.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iei.hywenlv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ekv.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://wyl.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pzo.chenjidiqi.icu

[F04] 追加写入文件
来源：http://eqg.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://slq.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qgs.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eih.gzhubu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dct.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ywf.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qss.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uof.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tvl.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://hix.yueranfly.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ihh.hongshengwenyu.top

PHP:  file_exists("a.txt");
来源：http://glg.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://dsp.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://obf.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cdf.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eah.gaohongyu789.top

Ruby: File.exist?("a.txt")
来源：http://svo.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://mog.xinyue.icu

[F06] 删除文件
来源：http://xrv.yj202588.top

Py:   os.remove("a.txt")
来源：http://lsy.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://zss.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://pda.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://svj.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jnm.gogol.net.cn

Go:   os.Remove("a.txt")
来源：http://gzf.yongpay.top

Ruby: File.delete("a.txt")
来源：http://tqt.zhiwuduotai.top

C#:   File.Delete("a.txt");
来源：http://aic.fktsv.cn

[F07] 创建目录（含多级）
来源：http://dav.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://glv.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cbb.hnqzz.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bes.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gtp.shuidangran.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kzx.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dqp.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ips.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://icl.pycfn.com

[F08] 遍历目录
来源：http://oxr.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xyy.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nkn.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://xth.yfazqb.com

TS:   fs.readdirSync("dir")
来源：http://poe.yangfankeji.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://azj.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jbz.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://qio.mhx1999.top

C#:   Directory.GetFiles("dir")
来源：http://oor.hnxiangtu.top

[F09] 获取文件大小
来源：http://zce.jqgufenzy.top

Py:   os.path.getsize("a.txt")
来源：http://gzr.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://ioo.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://gnh.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://izq.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://bjr.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rds.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://szt.fehbvm.com

C#:   new FileInfo("a.txt").Length
来源：http://uig.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://dny.shuidangran.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://euo.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jls.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hbt.ivvv.top

TS:   path.extname("a.txt")
来源：http://jhe.hongshengwenyu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zod.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nuh.mhx1999.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://okv.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yac.andypj.xyz

[F11] 复制与移动文件
来源：http://mmm.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qhi.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vsq.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://edv.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dum.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pwu.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kvc.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dva.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://urv.zhiwuduotai.top

[F12] CSV 读写
来源：http://luh.birdmap.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wky.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fei.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zqa.ydjk.org.cn

TS:   // 同上
来源：http://say.gzhubu.top


<!-- 参考信息 -->