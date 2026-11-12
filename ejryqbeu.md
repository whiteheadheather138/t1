代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xex.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vzt.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ygg.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wvx.guannengcc.top

[E02] 重复字符串
来源：http://ajz.nanxuanxn.top

Py:   "ab" * 3
来源：http://xsv.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://wzl.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://goj.guowangkeji.top

TS:   "ab".repeat(3)
来源：http://kqv.yonumen.top

Java: "ab".repeat(3)
来源：http://fjx.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://mop.jianghu66.top

Ruby: "ab" * 3
来源：http://lpv.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yct.vqdsnc.cn

[E03] 截取子串
来源：http://ozt.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ray.jinqigufen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mhu.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://krq.dashuyun.cn

TS:   s.slice(1, 4)
来源：http://jkk.mhx1999.top

Java: s.substring(1, 4)
来源：http://rhd.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bms.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://xxa.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://gdp.sufxvd.cn

[E04] 查找子串位置
来源：http://vph.redwolf501.top

Py:   s.find("x");  s.index("x")
来源：http://jzq.nanxinkj.top

PHP:  strpos($s, "x");
来源：http://ucp.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ldo.yvedp.cn

TS:   s.indexOf("x")
来源：http://ean.zhongyouzk.top

Java: s.indexOf("x")
来源：http://aks.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://sin.redwolf501.top

Ruby: s.index("x")
来源：http://axc.andypj.xyz

C#:   s.IndexOf("x")
来源：http://teg.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ylr.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://etn.ydjk.org.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://okv.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lek.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://unj.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zvp.zdbjq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://icz.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ayd.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pap.xuanzx.com

[E06] 替换子串
来源：http://mlo.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://edb.xuetiantiany.cn

PHP:  str_replace("a", "b", $s);
来源：http://mit.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dwr.pengpengdd.cyou

TS:   s.replaceAll("a", "b")
来源：http://mkr.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hvd.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fvz.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hsk.zhijiandao.cn

C#:   s.Replace("a", "b")
来源：http://ead.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://ohr.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wax.ivvv.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://odm.guannengcc.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jib.birdmap.top

TS:   s.split(",")
来源：http://lch.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sqj.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xyf.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://sia.zhoulong.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://avd.tian-w.cn

[E08] 数组按分隔符合并
来源：http://pbf.feifeiyinyue.top

Py:   ",".join(items)
来源：http://zpv.cdnleiting.top

PHP:  implode(",", $items);
来源：http://qaa.xziqi.cn

JS:   items.join(",")
来源：http://vzu.zhiwuduotai.top

TS:   items.join(",")
来源：http://xks.gogol.net.cn

Java: String.join(",", items)
来源：http://asg.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://bjg.snrcjt.cn

Ruby: items.join(",")
来源：http://kcw.gotoacloud.top

C#:   string.Join(",", items)
来源：http://etd.tianlin.xyz

[E09] 去除所有空白字符
来源：http://uhl.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lwr.aizwys.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ocv.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://puu.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://ibl.fehbvm.com

Java: s.replaceAll("\\s+", "")
来源：http://sig.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://omy.daria6918.cn

Ruby: s.gsub(/\s+/, "")
来源：http://suh.aizwys.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ifd.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://phx.nanxuanxn.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tgk.jyoumei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wpn.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://wcb.sufxvd.cn

TS:   "7".padStart(3, "0")
来源：http://aaa.chenjidiqi.icu

Java: String.format("%03d", 7)
来源：http://lwl.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://peg.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://adh.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mcb.cdnleiting.top

[E11] 反转字符串
来源：http://xwa.tarul.cn

Py:   s[::-1]
来源：http://sxz.hammf.cn

PHP:  strrev($s);
来源：http://lrp.jlsjyb.cn

JS:   [...s].reverse().join("")
来源：http://viy.tarul.cn

TS:   [...s].reverse().join("")
来源：http://csh.cucudq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zgp.tianlin.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://czx.hywenlv.cn

Ruby: s.reverse
来源：http://vpr.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bpv.fktsv.cn

[E12] 统计某字符出现次数
来源：http://bzi.fzhhl.top

Py:   s.count("a")
来源：http://cfa.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://sbh.daria6918.cn

JS:   s.split("a").length - 1
来源：http://mrg.birdmap.top

TS:   s.split("a").length - 1
来源：http://vkp.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aqy.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://fdg.sxryk.cn

Ruby: s.count("a")
来源：http://vit.gogol.net.cn

C#:   s.Count(c => c == 'a')
来源：http://vab.jinqigufen.top

[E13] 逐字符遍历
来源：http://fra.cheryme.top

Py:   for ch in s: print(ch)
来源：http://rhg.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ffr.wangdashe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xry.fanxiaobao.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://ibd.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jnh.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hrl.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://whu.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://exj.tarul.cn

[E14] URL 编码与 Base64
来源：http://qio.svipenyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://buz.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://snn.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://llw.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ovc.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tvw.xylfe.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cfo.feifeiyinyue.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gan.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aly.jinqigufen.top

[E15] HTML 转义 / 反转义
来源：http://dgo.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://npn.yfazqb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qfz.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yox.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hrs.yuanzhike.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fhm.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://omz.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lvz.sufxvd.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://abv.yangfankeji.com

[E16] 数字千分位
来源：http://uqa.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://rum.yj202588.top

PHP:  number_format(1234567);
来源：http://zxu.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xov.xuanzx.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ayj.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zki.aibaodan.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gkq.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tti.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://epy.fktsv.cn

[E17] 首字母大写
来源：http://lby.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ukz.bbcook.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://meb.smart0.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mqc.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uwq.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://prf.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ngx.mhx1999.top

Ruby: s.capitalize
来源：http://wcw.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yzm.zhongyouzk.top

[E18] 模板占位符替换
来源：http://nrv.andypj.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ocf.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eog.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lnc.hcnkem.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ynj.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dhd.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kzt.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uil.yj202588.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fhk.shuidangran.top

[E19] 多行文本按行拆分
来源：http://uje.feifeiyinyue.top

Py:   s.splitlines()
来源：http://tgg.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sdh.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://efz.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://ozi.dashuyun.cn

Java: s.lines().toList()
来源：http://iof.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://npo.jianghu66.top

Ruby: s.lines
来源：http://gxj.yangfankeji.com

C#:   s.Split('\n')
来源：http://iul.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://fst.ydjk.org.cn

Py:   if not s:
来源：http://arz.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zaj.shzxlz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wta.pengpengdd.cyou

TS:   if (s === "") {}
来源：http://beg.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://fmh.jianghu66.top

Go:   if s == "" {}
来源：http://hhz.hnqzz.top

Ruby: if s.empty?
来源：http://rmc.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qmm.zdbjq.cn

[E21] 超长截断加省略号
来源：http://nvf.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kvg.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ddp.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nep.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bnv.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eur.epnwcf.com

Go:   // 按 rune 判断长度后截断
来源：http://vib.hnxiangtu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ezu.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wxv.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://ach.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uyc.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jmy.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vwr.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fwl.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zsy.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://puh.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://rwr.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ves.chenzaomai.com

================================================================================
来源：http://wht.aibaodan.cn

F. 文件与目录
来源：http://wtz.zhoulong.xyz

================================================================================
来源：http://mop.chenzaomai.com

[F01] 读取整个文件
来源：http://rfk.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fzf.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://uqv.havefunace.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ohz.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ioj.hammf.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hbg.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rsp.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://wpq.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://epz.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://gdv.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qdh.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ezt.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ubg.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://euh.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wir.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vfk.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zbq.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ffy.meibo888.top

[F03] 写入文件（覆盖）
来源：http://bnh.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sbc.cdnleiting.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://prg.andypj.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hnl.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xni.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://btd.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ktz.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://may.yuxming.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rua.zdbjq.cn

[F04] 追加写入文件
来源：http://kcg.fehbvm.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://quw.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hcs.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yyl.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zke.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wfl.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lgq.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nib.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fyk.wangdashe.top

[F05] 判断文件或目录是否存在
来源：http://xdz.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://elx.shangyingyoupin.top

PHP:  file_exists("a.txt");
来源：http://ilq.guowangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://vvv.xziqi.cn

TS:   fs.existsSync("a.txt")
来源：http://pui.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fsj.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kri.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://yuc.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://dcz.quarkkingdee.top

[F06] 删除文件
来源：http://tcc.hnqzz.top

Py:   os.remove("a.txt")
来源：http://zap.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://abu.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://gnr.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rrr.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zwb.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://tyj.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://hxs.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://pot.snrcjt.cn

[F07] 创建目录（含多级）
来源：http://uas.yj20258888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cey.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qum.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jao.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cqe.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ooc.zhaomingkeji.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fjt.0kj1m.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://avl.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fjz.yueranfly.top

[F08] 遍历目录
来源：http://gjd.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://omp.shangyingyoupin.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eaq.xinyue.icu

JS:   fs.readdirSync("dir")
来源：http://srx.cqqwz.cn

TS:   fs.readdirSync("dir")
来源：http://vul.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rgk.vehdjk.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://bux.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://qdo.fanxiaobao.xyz

C#:   Directory.GetFiles("dir")
来源：http://dbn.xinyue.icu

[F09] 获取文件大小
来源：http://mjp.sysykeji.top

Py:   os.path.getsize("a.txt")
来源：http://mzv.hesvh.cn

PHP:  filesize("a.txt");
来源：http://crt.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://nxy.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://tva.epnwcf.com

Java: Files.size(Path.of("a.txt"))
来源：http://ran.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://syf.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://nap.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://edc.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://dhx.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qtv.ehwqpu.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tbd.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xxd.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://rzs.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ais.cheryme.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zqo.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://buq.ivvv.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zsd.hfpthk.cn

[F11] 复制与移动文件
来源：http://wvw.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ade.cdnleiting.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kfa.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jjn.fktsv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jem.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cim.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jxa.bjfxy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uwz.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://etj.xziqi.cn

[F12] CSV 读写
来源：http://car.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://beb.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rtf.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lin.jinyuanbaomall.cn

TS:   // 同上
来源：http://nsj.gogol.net.cn


<!-- 参考信息 -->