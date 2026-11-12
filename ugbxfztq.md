代发 wailian999

================================================================================
来源：http://yfs.hnqzz.top

E. 字符串处理
来源：http://elq.sufxvd.cn

================================================================================
来源：http://sxt.shuidangran.top

[E01] 拼接字符串
来源：http://gwq.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aez.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fsf.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jou.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kro.guannengcc.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cce.yvedp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aep.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://asn.jyoumei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uok.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://enj.wangdashe.top

Py:   "ab" * 3
来源：http://hok.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://xcw.c1oappe.top

JS:   "ab".repeat(3)
来源：http://fen.dianchejie.cn

TS:   "ab".repeat(3)
来源：http://jmi.ivvv.top

Java: "ab".repeat(3)
来源：http://jqj.yueranfly.top

Go:   strings.Repeat("ab", 3)
来源：http://xdy.yvedp.cn

Ruby: "ab" * 3
来源：http://bbj.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zau.nanxuanxn.top

[E03] 截取子串
来源：http://bts.smart0.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rzi.daxiang520.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oki.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://acd.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://fvo.smart0.xyz

Java: s.substring(1, 4)
来源：http://oom.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yee.pycfn.com

Ruby: s[1, 3];  s[1..3]
来源：http://bci.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://uju.jinyuanbaomall.cn

[E04] 查找子串位置
来源：http://eev.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://uuu.ctjpmb.com

PHP:  strpos($s, "x");
来源：http://gtg.vqdsnc.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ema.shuidangran.top

TS:   s.indexOf("x")
来源：http://lqw.sysykeji.top

Java: s.indexOf("x")
来源：http://ojq.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://svb.guannengcc.top

Ruby: s.index("x")
来源：http://nrg.fzhhl.top

C#:   s.IndexOf("x")
来源：http://roj.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://hlp.bbcook.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rcq.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hpl.shzxlz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vge.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://rbz.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://snc.feifeiyinyue.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aio.daria6918.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mig.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://edw.sufxvd.cn

[E06] 替换子串
来源：http://ejx.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eme.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://zuy.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://puf.chenjidiqi.icu

TS:   s.replaceAll("a", "b")
来源：http://aby.jianghu66.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eir.hammf.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rjy.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qak.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://jxz.yj202588.top

[E07] 按分隔符拆分
来源：http://dkb.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ndk.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jdv.xylfe.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qlu.vehdjk.com

TS:   s.split(",")
来源：http://uem.yfazqb.com

Java: s.split(",");  s.split("\\s+")
来源：http://shy.meibo888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lrt.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://tln.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yti.0kj1m.cn

[E08] 数组按分隔符合并
来源：http://wif.tarul.cn

Py:   ",".join(items)
来源：http://ywu.chenzaomai.com

PHP:  implode(",", $items);
来源：http://akn.hesvh.cn

JS:   items.join(",")
来源：http://ppm.hnxiangtu.top

TS:   items.join(",")
来源：http://adv.daria6918.cn

Java: String.join(",", items)
来源：http://wpj.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://ctn.aizwys.cn

Ruby: items.join(",")
来源：http://eto.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://qtp.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://bcg.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ptl.yongpay.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ayy.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://ids.yj20258888.top

TS:   s.replace(/\s+/g, "")
来源：http://wax.chenjidiqi.icu

Java: s.replaceAll("\\s+", "")
来源：http://cfr.sweek.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ifn.redwolf501.top

Ruby: s.gsub(/\s+/, "")
来源：http://usg.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ule.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://rhs.fzhhl.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jvx.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wlx.tian-w.cn

JS:   "7".padStart(3, "0")
来源：http://tpg.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://ogr.nanxinkj.top

Java: String.format("%03d", 7)
来源：http://mqu.daria6918.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rcg.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://glx.jinyuanbaomall.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bzv.yanxiufei.cn

[E11] 反转字符串
来源：http://lnh.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://hsa.cqqwz.cn

PHP:  strrev($s);
来源：http://dci.jinqigfzy.top

JS:   [...s].reverse().join("")
来源：http://vpl.zycfv.cn

TS:   [...s].reverse().join("")
来源：http://bhp.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://agy.c1oappe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://srb.hfpthk.cn

Ruby: s.reverse
来源：http://oxh.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://ose.nanxuanxn.top

[E12] 统计某字符出现次数
来源：http://ann.tanke756.top

Py:   s.count("a")
来源：http://agu.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://muj.shuidangran.top

JS:   s.split("a").length - 1
来源：http://vzn.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://bbz.mhx1999.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zvw.tianlin.xyz

Go:   strings.Count(s, "a")
来源：http://xor.ivvv.top

Ruby: s.count("a")
来源：http://yfm.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://wvd.epnwcf.com

[E13] 逐字符遍历
来源：http://pzz.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://jtv.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yeq.zdqjudy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tzx.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://cgc.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aas.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tcy.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ijk.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rjj.ppjwa.cn

[E14] URL 编码与 Base64
来源：http://etc.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://isx.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rhv.yj20258.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eqn.shzxlz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jvx.zhijiandao.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uvx.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dwv.chenlongwang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oqi.nwbrower.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yuo.dianchejie.cn

[E15] HTML 转义 / 反转义
来源：http://yjo.gaohongyu789.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cdp.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kbu.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kjp.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lhn.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wfw.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vmu.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pdj.smart0.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vyj.snrcjt.cn

[E16] 数字千分位
来源：http://ako.tanke756.top

Py:   f"{1234567:,}"
来源：http://xii.aizwys.cn

PHP:  number_format(1234567);
来源：http://qkb.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mvq.yueranfly.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lwd.fktsv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uln.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jvb.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gio.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://dui.tianlin.xyz

[E17] 首字母大写
来源：http://pvg.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://obf.nanxinkj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jrn.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yhk.dianchejie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fma.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jzu.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tpo.zhijiandao.cn

Ruby: s.capitalize
来源：http://jev.epnwcf.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ial.smart0.xyz

[E18] 模板占位符替换
来源：http://nah.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gbr.c1oappe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jpq.jinqigufen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ahg.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://juc.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ysx.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mzp.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nwm.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://upz.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://ren.yvedp.cn

Py:   s.splitlines()
来源：http://xyu.zdqjudy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zct.svipenyu.cn

JS:   s.split(/\r?\n/)
来源：http://sax.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://upy.ybcxt.top

Java: s.lines().toList()
来源：http://azd.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://idt.chenjidiqi.icu

Ruby: s.lines
来源：http://pjm.gzhubu.top

C#:   s.Split('\n')
来源：http://mov.fengsongda.top

[E20] 判断字符串是否为空
来源：http://tib.yongpay.top

Py:   if not s:
来源：http://dak.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pcs.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://duk.hnqzz.top

TS:   if (s === "") {}
来源：http://ydp.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://rwj.cucudq.cn

Go:   if s == "" {}
来源：http://ubu.xylfe.cn

Ruby: if s.empty?
来源：http://mvc.xingfuxueyuan.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zbh.chenzaomai.com

[E21] 超长截断加省略号
来源：http://sra.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zgx.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rrm.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bnv.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jjb.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://goo.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://zca.hesvh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qwi.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qed.c1oappe.top

[E22] 字节长度与字符长度
来源：http://ght.cucudq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eeu.tarul.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lhf.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wug.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oqs.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dex.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://raw.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://kyb.hfpthk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gmk.vehdjk.com

================================================================================
来源：http://oox.zhaomingkeji.xyz

F. 文件与目录
来源：http://xni.aibaodan.cn

================================================================================
来源：http://iaa.quarkkingdee.top

[F01] 读取整个文件
来源：http://drh.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yoo.meibo888.top

PHP:  file_get_contents("a.txt");
来源：http://kta.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kkx.zdbjq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tcp.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nky.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dxk.zycfv.cn

Ruby: File.read("a.txt")
来源：http://cvx.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://obd.sufxvd.cn

[F02] 逐行读取文件
来源：http://fbf.yuxming.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jic.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aol.hammf.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ele.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ceq.ybcxt.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dqr.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mvh.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jys.xuetiantiany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uhm.cashguo.top

[F03] 写入文件（覆盖）
来源：http://lhu.chenzaomai.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bxf.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ncx.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rjc.cqqwz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aly.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lrv.aizwys.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://knp.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://ccq.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://orf.smart0.xyz

[F04] 追加写入文件
来源：http://opr.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pfq.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jkj.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mze.snrcjt.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xlq.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tkm.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://djs.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rns.yongpay.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hzh.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://buz.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://atq.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://mbu.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://dzu.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://had.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://isu.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zkz.hfpthk.cn

Ruby: File.exist?("a.txt")
来源：http://oqh.jinyuanbaomall.cn

C#:   File.Exists("a.txt")
来源：http://crn.sysykeji.top

[F06] 删除文件
来源：http://ukz.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://ndp.yonumen.top

PHP:  unlink("a.txt");
来源：http://pky.fengsongda.top

JS:   fs.unlinkSync("a.txt")
来源：http://qrx.daria6918.cn

TS:   fs.unlinkSync("a.txt")
来源：http://igr.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yvy.yonumen.top

Go:   os.Remove("a.txt")
来源：http://lpo.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://pvw.tianlin.xyz

C#:   File.Delete("a.txt");
来源：http://fje.mhx1999.top

[F07] 创建目录（含多级）
来源：http://wcd.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cew.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zrn.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hnh.dashuyun.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://piw.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yys.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nya.jyoumei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xve.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gql.daria6918.cn

[F08] 遍历目录
来源：http://whj.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://tbe.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wfu.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://bky.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://xwx.yangfankeji.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iuj.52xcode.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rlw.yueranfly.top

Ruby: Dir.children("dir")
来源：http://wrv.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://kme.cdnleiting.top

[F09] 获取文件大小
来源：http://yxf.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://zfb.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://yyp.tanke756.top

JS:   fs.statSync("a.txt").size
来源：http://tay.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://cwo.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kjt.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tqt.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://mtx.yj20258888.top

C#:   new FileInfo("a.txt").Length
来源：http://zny.hnxiangtu.top

[F10] 取文件扩展名 / 文件名
来源：http://uia.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cek.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fnv.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ycw.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://oug.cqqwz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://epy.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ucf.svipenyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pfw.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rsj.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://vwv.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tuh.hcnkem.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://omc.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tdb.ybcxt.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qft.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://juj.vqdsnc.cn


<!-- 参考信息 -->