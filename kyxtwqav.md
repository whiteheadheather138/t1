代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mkb.havefunace.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://haq.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wsh.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dun.daxiang520.top

[E02] 重复字符串
来源：http://hhb.daria6918.cn

Py:   "ab" * 3
来源：http://rjh.ybcxt.top

PHP:  str_repeat("ab", 3);
来源：http://uvy.xuanzx.com

JS:   "ab".repeat(3)
来源：http://wxb.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://bik.cucudq.cn

Java: "ab".repeat(3)
来源：http://zju.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://xhe.yanxiufei.cn

Ruby: "ab" * 3
来源：http://exa.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://weg.dashuyun.cn

[E03] 截取子串
来源：http://pyi.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xnx.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://msm.yj20258888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gdr.zhaomingkeji.xyz

TS:   s.slice(1, 4)
来源：http://jet.epnwcf.com

Java: s.substring(1, 4)
来源：http://aiv.xuetiantiany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vkx.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://gcr.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://mms.hammf.cn

[E04] 查找子串位置
来源：http://biu.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://qbo.pycfn.com

PHP:  strpos($s, "x");
来源：http://vgg.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xtw.zhongyouzk.top

TS:   s.indexOf("x")
来源：http://awq.guannengcc.top

Java: s.indexOf("x")
来源：http://tdl.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://nmd.yj20258888.top

Ruby: s.index("x")
来源：http://twh.vehdjk.com

C#:   s.IndexOf("x")
来源：http://vlp.haohaochexian.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yfs.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kvn.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nwb.quarkkingdee.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sgd.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ioc.yj20258.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vzb.fengsongda.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eeo.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://spo.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tcj.cashguo.top

[E06] 替换子串
来源：http://wkj.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fkl.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://eih.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ije.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://eby.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tmh.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bfg.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nbl.fehbvm.com

C#:   s.Replace("a", "b")
来源：http://wng.hysaishi.cn

[E07] 按分隔符拆分
来源：http://rlw.cqqwz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://any.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wqc.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://oam.daxiang520.top

TS:   s.split(",")
来源：http://mvg.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://udf.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bio.jiagoushi.top

Ruby: s.split(",");  s.split
来源：http://wft.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ynm.yvedp.cn

[E08] 数组按分隔符合并
来源：http://tlr.hcnkem.com

Py:   ",".join(items)
来源：http://apv.sweek.top

PHP:  implode(",", $items);
来源：http://uir.hammf.cn

JS:   items.join(",")
来源：http://weo.yj20258888.top

TS:   items.join(",")
来源：http://zap.xziqi.cn

Java: String.join(",", items)
来源：http://cfk.ywan-chungtsiang.top

Go:   strings.Join(items, ",")
来源：http://wzc.yj202588.top

Ruby: items.join(",")
来源：http://ehe.hesvh.cn

C#:   string.Join(",", items)
来源：http://dol.wangshuangyany.cn

[E09] 去除所有空白字符
来源：http://vdm.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ocw.daxiang520.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gdg.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://fvr.tanke756.top

TS:   s.replace(/\s+/g, "")
来源：http://ptl.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://fjq.quarkkingdee.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ztx.daxiang520.top

Ruby: s.gsub(/\s+/, "")
来源：http://clf.pengpengdd.cyou

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wfg.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://rql.tian-w.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qhu.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uru.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://bsu.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://fel.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://oaq.hysaishi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yhg.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ger.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xlb.jlsjyb.cn

[E11] 反转字符串
来源：http://whg.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://izz.shanyushiyangtech.top

PHP:  strrev($s);
来源：http://flh.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://fgb.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://tvw.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ifq.cdnleiting.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://djy.hnxiangtu.top

Ruby: s.reverse
来源：http://lbo.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://lxo.zycfv.cn

[E12] 统计某字符出现次数
来源：http://egl.fktsv.cn

Py:   s.count("a")
来源：http://yjc.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://hik.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://hxb.tian-w.cn

TS:   s.split("a").length - 1
来源：http://aua.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gnk.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://gri.ctjpmb.com

Ruby: s.count("a")
来源：http://ied.bbcook.cn

C#:   s.Count(c => c == 'a')
来源：http://qwb.aibaodan.cn

[E13] 逐字符遍历
来源：http://gxj.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://khx.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mbs.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://xsy.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://iza.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xfb.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fth.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://cay.yj20258888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ceh.shanyushiyangtech.top

[E14] URL 编码与 Base64
来源：http://eox.jiagoushi.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fup.sysykeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uuk.andypj.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rtb.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vrg.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kfg.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aqz.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yyf.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ctt.nanxuanxn.top

[E15] HTML 转义 / 反转义
来源：http://tin.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pyh.guowangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wuz.jlsjyb.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sjf.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://esn.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fme.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wga.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eze.yj20258.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qgw.uphjek.com

[E16] 数字千分位
来源：http://guo.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://hqy.gzhubu.top

PHP:  number_format(1234567);
来源：http://rpo.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cgo.yuanzhike.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ceb.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://osl.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aup.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cow.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://mgn.zhengqikj.top

[E17] 首字母大写
来源：http://cxy.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ywe.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ggh.meibo888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kss.zhoulong.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aio.vehdjk.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hid.svipenyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xmg.shzxlz.cn

Ruby: s.capitalize
来源：http://anw.daxiang520.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://urc.epnwcf.com

[E18] 模板占位符替换
来源：http://baq.cashguo.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bhf.iojbl.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wjo.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ozp.pengpengdd.cyou

TS:   tpl.replaceAll("{name}", name)
来源：http://ixs.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xld.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lub.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://scf.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lvl.iojbl.cn

[E19] 多行文本按行拆分
来源：http://nby.yanxiufei.cn

Py:   s.splitlines()
来源：http://kpi.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xwa.jinqigfzy.top

JS:   s.split(/\r?\n/)
来源：http://gsk.tian-w.cn

TS:   s.split(/\r?\n/)
来源：http://vcf.hnqzz.top

Java: s.lines().toList()
来源：http://lpu.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://dbj.fanxiaobao.xyz

Ruby: s.lines
来源：http://jrf.redwolf501.top

C#:   s.Split('\n')
来源：http://ghv.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://vua.52xcode.cn

Py:   if not s:
来源：http://lfq.xylfe.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yvl.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dge.zdbjq.cn

TS:   if (s === "") {}
来源：http://qhg.cheryme.top

Java: if (s.isEmpty()) {}
来源：http://tzh.epnwcf.com

Go:   if s == "" {}
来源：http://hbw.tianlin.xyz

Ruby: if s.empty?
来源：http://rap.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://igf.birdmap.top

[E21] 超长截断加省略号
来源：http://uls.xylfe.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cyr.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xgu.fehbvm.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tgd.jlsjyb.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kze.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kvb.jiagoushi.top

Go:   // 按 rune 判断长度后截断
来源：http://aqh.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mag.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xdg.havefunace.top

[E22] 字节长度与字符长度
来源：http://uxv.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yds.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yjd.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blo.epnwcf.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://awu.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sfd.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://che.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://rpu.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lyw.jyoumei.cn

================================================================================
来源：http://ikk.hcnkem.com

F. 文件与目录
来源：http://bbb.yuxming.cn

================================================================================
来源：http://wrb.fengsongda.top

[F01] 读取整个文件
来源：http://tbd.ivvv.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lbw.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://txa.zycfv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://znk.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dmc.wangdashe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lvt.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gzg.yuanzhike.top

Ruby: File.read("a.txt")
来源：http://ppz.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://dgd.xylfe.cn

[F02] 逐行读取文件
来源：http://wqu.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://csm.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jgc.jqgufenzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://apo.sufxvd.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jya.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yrg.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zfm.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rcc.guannengcc.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fyj.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://xwe.quarkkingdee.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vze.birdmap.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xaa.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iam.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cib.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xhv.redwolf501.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://acd.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://pnf.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dio.tanke756.top

[F04] 追加写入文件
来源：http://bey.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gym.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ocb.shuidangran.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cde.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://woz.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ozp.ppjwa.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kvy.hcnkem.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zyl.nanxuanxn.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ntp.jianghu66.top

[F05] 判断文件或目录是否存在
来源：http://riy.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mam.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://ude.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://nqe.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://cyk.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://bwe.pengpengdd.cyou

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iwt.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://gko.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://hcw.vqdsnc.cn

[F06] 删除文件
来源：http://fra.yongpay.top

Py:   os.remove("a.txt")
来源：http://nhn.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://cmg.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sfu.c1oappe.top

TS:   fs.unlinkSync("a.txt")
来源：http://jvb.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aoy.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://zxx.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://fch.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://ojh.iojbl.cn

[F07] 创建目录（含多级）
来源：http://udv.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gzs.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rbg.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vgy.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lic.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://avj.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bsv.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zra.sjlbkw.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gnc.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://qry.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hmy.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gzn.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://ecp.jlsjyb.cn

TS:   fs.readdirSync("dir")
来源：http://kqq.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://siu.jianghu66.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zka.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://giw.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://yhz.hnqzz.top

[F09] 获取文件大小
来源：http://iph.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://ezl.hcnkem.com

PHP:  filesize("a.txt");
来源：http://xfj.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://oig.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://brc.hnxiangtu.top

Java: Files.size(Path.of("a.txt"))
来源：http://qpd.yanxiufei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jtw.tarul.cn

Ruby: File.size("a.txt")
来源：http://vxa.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://dft.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://crt.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cmj.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://olt.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rib.xylfe.cn

TS:   path.extname("a.txt")
来源：http://bur.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pkk.shzxlz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nch.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://irz.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://suf.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://sdt.zhongyouzk.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jed.zhijiandao.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://izv.mhx1999.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tmr.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hmr.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uab.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lut.zhengqikj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vok.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yel.ppjwa.cn

[F12] CSV 读写
来源：http://scf.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ree.nwbrower.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vvy.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eyl.jlsjyb.cn

TS:   // 同上
来源：http://ufj.zhaomingkeji.xyz


<!-- 参考信息 -->