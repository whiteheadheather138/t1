代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qzs.yueranfly.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kdg.tarul.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ucz.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vth.hywenlv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ban.tanke756.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eje.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ymr.shanyushiyangtech.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eyo.xylfe.cn

[E02] 重复字符串
来源：http://rie.jinqigufen.top

Py:   "ab" * 3
来源：http://vxn.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://uhz.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://wih.yvedp.cn

TS:   "ab".repeat(3)
来源：http://blo.ehwqpu.com

Java: "ab".repeat(3)
来源：http://wff.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://tuc.jlsjyb.cn

Ruby: "ab" * 3
来源：http://dad.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qyy.birdmap.top

[E03] 截取子串
来源：http://ddt.yongpay.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hfo.hnqzz.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qqw.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ujw.snrcjt.cn

TS:   s.slice(1, 4)
来源：http://jqr.52xcode.cn

Java: s.substring(1, 4)
来源：http://rox.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hlq.zhiwuduotai.top

Ruby: s[1, 3];  s[1..3]
来源：http://tnn.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://trd.yongpay.top

[E04] 查找子串位置
来源：http://ota.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://mfv.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://zvy.yongpay.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jml.zhixingplan.top

TS:   s.indexOf("x")
来源：http://myf.hnxiangtu.top

Java: s.indexOf("x")
来源：http://xaj.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://ekp.shuidangran.top

Ruby: s.index("x")
来源：http://zqg.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://hbn.haohaochexian.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ywc.ctjpmb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fqs.c1oappe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qae.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ilx.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zpt.gogol.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ilc.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://otn.cucudq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zpq.bjfxy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rjr.hnxiangtu.top

[E06] 替换子串
来源：http://rps.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xql.yuanzhike.top

PHP:  str_replace("a", "b", $s);
来源：http://dlj.kuanghao11.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gjm.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://nrq.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lhv.52xcode.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qis.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kgs.zhoulong.xyz

C#:   s.Replace("a", "b")
来源：http://wdf.zhoulong.xyz

[E07] 按分隔符拆分
来源：http://cht.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yhn.aibaodan.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://chv.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://llo.aizwys.cn

TS:   s.split(",")
来源：http://lqd.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://dpn.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://djz.ywan-chungtsiang.top

Ruby: s.split(",");  s.split
来源：http://nml.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yet.ybcxt.top

[E08] 数组按分隔符合并
来源：http://mau.shzxlz.cn

Py:   ",".join(items)
来源：http://rtq.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://zxc.cqqwz.cn

JS:   items.join(",")
来源：http://mvn.jlsjyb.cn

TS:   items.join(",")
来源：http://mah.epnwcf.com

Java: String.join(",", items)
来源：http://rof.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://ulj.sjlbkw.cn

Ruby: items.join(",")
来源：http://dui.hnqzz.top

C#:   string.Join(",", items)
来源：http://zeg.nanxinkj.top

[E09] 去除所有空白字符
来源：http://tfh.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zgp.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://amt.nanxuanxn.top

JS:   s.replace(/\s+/g, "")
来源：http://anx.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://vlt.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://cud.nanxuanxn.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nsh.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://bty.mhx1999.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bjk.guowangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://ggw.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hij.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ddk.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://gut.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://ela.vqdsnc.cn

Java: String.format("%03d", 7)
来源：http://ybw.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vqe.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dli.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vuo.feifeiyinyue.top

[E11] 反转字符串
来源：http://fai.fehbvm.com

Py:   s[::-1]
来源：http://hsc.hywenlv.cn

PHP:  strrev($s);
来源：http://wtt.nanxinkj.top

JS:   [...s].reverse().join("")
来源：http://kev.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://hea.cucudq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://khl.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://azz.xuetiantiany.cn

Ruby: s.reverse
来源：http://jkl.uphjek.com

C#:   new string(s.Reverse().ToArray())
来源：http://njv.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://qlv.aizwys.cn

Py:   s.count("a")
来源：http://fln.hfpthk.cn

PHP:  substr_count($s, "a");
来源：http://upl.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://str.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://elr.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jvt.zhongyouzk.top

Go:   strings.Count(s, "a")
来源：http://rog.jianghu66.top

Ruby: s.count("a")
来源：http://ifb.fehbvm.com

C#:   s.Count(c => c == 'a')
来源：http://tsw.fanxiaobao.xyz

[E13] 逐字符遍历
来源：http://avc.meibo888.top

Py:   for ch in s: print(ch)
来源：http://tcj.shanyushiyangtech.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kvy.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kmo.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hmp.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vkj.jqgufenzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nwh.iojbl.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sgz.jlsjyb.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jvr.aizwys.cn

[E14] URL 编码与 Base64
来源：http://azz.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jge.zhiwuduotai.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mns.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nhs.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nap.havefunace.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vne.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lyo.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cen.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lan.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://gwk.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://qyy.yfazqb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zbq.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://imb.zhoulong.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://lsm.tianlin.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tbj.daxiang520.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mgo.dianchejie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hlq.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ydy.ctjpmb.com

[E16] 数字千分位
来源：http://jut.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://gvk.snrcjt.cn

PHP:  number_format(1234567);
来源：http://vrf.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cot.vqdsnc.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vxz.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tbi.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uha.wangdashe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jbb.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://nsy.hcnkem.com

[E17] 首字母大写
来源：http://chj.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eay.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://len.jyoumei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hfn.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://guu.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vxh.ywan-chungtsiang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kbu.jianghu66.top

Ruby: s.capitalize
来源：http://mjp.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qat.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://lpv.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zrm.9152youxi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wfa.yangfankeji.com

JS:   tpl.replaceAll("{name}", name)
来源：http://pel.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ilg.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qxs.ydzc1.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hhy.jinqigfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://har.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://flk.iojbl.cn

[E19] 多行文本按行拆分
来源：http://qun.fanxiaobao.xyz

Py:   s.splitlines()
来源：http://xqg.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wpy.jyoumei.cn

JS:   s.split(/\r?\n/)
来源：http://rgq.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://jeg.epnwcf.com

Java: s.lines().toList()
来源：http://fot.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://ccq.cashguo.top

Ruby: s.lines
来源：http://ykm.kuanghao11.cn

C#:   s.Split('\n')
来源：http://smz.0kj1m.cn

[E20] 判断字符串是否为空
来源：http://wfg.jqgfzy.top

Py:   if not s:
来源：http://nhi.hnxiangtu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ibt.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zqf.yj20258.top

TS:   if (s === "") {}
来源：http://okf.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://iyg.jlsjyb.cn

Go:   if s == "" {}
来源：http://far.ybcxt.top

Ruby: if s.empty?
来源：http://ktv.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rbl.jianghu66.top

[E21] 超长截断加省略号
来源：http://fhu.feifeiyinyue.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dlm.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dbj.yongpay.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zmo.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bad.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ikw.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://ntz.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wna.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bjp.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://xqd.shanyushiyangtech.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ycn.fengsongda.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dqd.quarkkingdee.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pvc.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nkm.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://end.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nod.daria6918.cn

Ruby: s.bytesize;  s.length
来源：http://kcb.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ujz.aizwys.cn

================================================================================
来源：http://lab.zhongyouzk.top

F. 文件与目录
来源：http://nbm.dashuyun.cn

================================================================================
来源：http://oof.tianlin.xyz

[F01] 读取整个文件
来源：http://irr.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ert.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://cok.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bhx.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rbo.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://apn.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lup.hammf.cn

Ruby: File.read("a.txt")
来源：http://fdk.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://rgk.nwbrower.top

[F02] 逐行读取文件
来源：http://tec.jinqigfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hux.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qgg.ehwqpu.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wae.sxryk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lpo.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jzn.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vbt.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://otl.52xcode.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://njj.ehwqpu.com

[F03] 写入文件（覆盖）
来源：http://eac.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pqw.yueranfly.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fjc.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rbc.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gsw.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gfl.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cqw.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://hhd.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lge.sjlbkw.cn

[F04] 追加写入文件
来源：http://ixg.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://czp.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qal.ydjk.org.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xvi.hywenlv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eva.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jxf.zdqjudy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hsr.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ixe.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dza.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://mke.quarkkingdee.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oue.pengpengdd.cyou

PHP:  file_exists("a.txt");
来源：http://led.yvedp.cn

JS:   fs.existsSync("a.txt")
来源：http://mlk.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://dgy.gotoacloud.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vin.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gvv.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://awa.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://pal.guowangkeji.top

[F06] 删除文件
来源：http://xhw.yonumen.top

Py:   os.remove("a.txt")
来源：http://uov.yuanzhike.top

PHP:  unlink("a.txt");
来源：http://gnu.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://fuf.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://rfy.feifeiyinyue.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rgg.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://erv.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://rga.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://jus.yuanzhike.top

[F07] 创建目录（含多级）
来源：http://oxi.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mej.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mzq.9152youxi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://klh.cashguo.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yla.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ozm.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hjc.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wmx.xziqi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://voo.316326.xyz

[F08] 遍历目录
来源：http://lnw.ydjk.org.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lru.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://btr.jqgufenzy.top

JS:   fs.readdirSync("dir")
来源：http://kvb.shuidangran.top

TS:   fs.readdirSync("dir")
来源：http://hne.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://owf.vehdjk.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://zig.fehbvm.com

Ruby: Dir.children("dir")
来源：http://mmu.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://jen.tanke756.top

[F09] 获取文件大小
来源：http://bpq.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://pbo.c1oappe.top

PHP:  filesize("a.txt");
来源：http://kky.xziqi.cn

JS:   fs.statSync("a.txt").size
来源：http://gco.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://qjy.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://xvp.chenzaomai.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zqq.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://msh.zhijiandao.cn

C#:   new FileInfo("a.txt").Length
来源：http://uba.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://wem.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vcf.jiagoushi.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kmy.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mbi.cheryme.top

TS:   path.extname("a.txt")
来源：http://gub.fktsv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mdz.jinqigfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hsx.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pzo.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tum.redwolf501.top

[F11] 复制与移动文件
来源：http://ggp.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sgd.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gvl.yj20258888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sjm.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yoz.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lif.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lmx.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aed.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://drl.shangyingyoupin.top

[F12] CSV 读写
来源：http://lio.zycfv.cn


<!-- 参考信息 -->