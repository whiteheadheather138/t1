代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iwr.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gkj.nwbrower.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://piu.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ryo.yanxiufei.cn

[E02] 重复字符串
来源：http://fgz.gogol.net.cn

Py:   "ab" * 3
来源：http://sja.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://wqn.cdnleiting.top

JS:   "ab".repeat(3)
来源：http://xyl.jinyuanbaomall.cn

TS:   "ab".repeat(3)
来源：http://kej.smart0.xyz

Java: "ab".repeat(3)
来源：http://wak.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://xxs.yj20258.top

Ruby: "ab" * 3
来源：http://sfi.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kam.jiagoushi.top

[E03] 截取子串
来源：http://okn.jinghuilouyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vex.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://imw.shanyushiyangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fwk.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://iwu.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://oew.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tmo.jinghuilouyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zsp.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://qny.vehdjk.com

[E04] 查找子串位置
来源：http://sju.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://gys.nwbrower.top

PHP:  strpos($s, "x");
来源：http://ixn.zhixingplan.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vqg.ivvv.top

TS:   s.indexOf("x")
来源：http://cjo.vqdsnc.cn

Java: s.indexOf("x")
来源：http://lhl.mhx1999.top

Go:   strings.Index(s, "x")
来源：http://fdz.hammf.cn

Ruby: s.index("x")
来源：http://wpn.uphjek.com

C#:   s.IndexOf("x")
来源：http://wkz.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gvr.fanxiaobao.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zua.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fsk.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hhh.sysykeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://oon.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rbh.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bsd.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xpu.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mgq.zhengqikj.top

[E06] 替换子串
来源：http://riw.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qvl.yj20258.top

PHP:  str_replace("a", "b", $s);
来源：http://jgn.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ytv.birdmap.top

TS:   s.replaceAll("a", "b")
来源：http://pfu.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yov.cheryme.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://was.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xhp.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://lgq.cucudq.cn

[E07] 按分隔符拆分
来源：http://jud.birdmap.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wxd.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ywd.pycfn.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ujn.epnwcf.com

TS:   s.split(",")
来源：http://hoo.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://szp.zycfv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xug.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://qxo.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vtw.yfazqb.com

[E08] 数组按分隔符合并
来源：http://nhv.0kj1m.cn

Py:   ",".join(items)
来源：http://rjk.fehbvm.com

PHP:  implode(",", $items);
来源：http://lbn.zycfv.cn

JS:   items.join(",")
来源：http://ygj.daxiang520.top

TS:   items.join(",")
来源：http://jeh.sxryk.cn

Java: String.join(",", items)
来源：http://tio.sxryk.cn

Go:   strings.Join(items, ",")
来源：http://ebi.vqdsnc.cn

Ruby: items.join(",")
来源：http://biv.sufxvd.cn

C#:   string.Join(",", items)
来源：http://vsd.aibaodan.cn

[E09] 去除所有空白字符
来源：http://khh.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zgw.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iyx.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://aal.cucudq.cn

TS:   s.replace(/\s+/g, "")
来源：http://bqd.guannengcc.top

Java: s.replaceAll("\\s+", "")
来源：http://jvo.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://inb.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://ngz.snrcjt.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kwl.yongpay.top

[E10] 左侧补零 / 定长填充
来源：http://iwo.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xks.quarkkingdee.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ngo.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://jqn.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://atw.yuxming.cn

Java: String.format("%03d", 7)
来源：http://orf.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://jua.yueranfly.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yeo.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mej.ppjwa.cn

[E11] 反转字符串
来源：http://ycp.yuanzhike.top

Py:   s[::-1]
来源：http://cct.tian-w.cn

PHP:  strrev($s);
来源：http://xoy.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://xuo.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://chh.tian-w.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cwe.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://iiy.hnqzz.top

Ruby: s.reverse
来源：http://hia.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://crc.fzhhl.top

[E12] 统计某字符出现次数
来源：http://aef.vehdjk.com

Py:   s.count("a")
来源：http://orv.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://mpd.sweek.top

JS:   s.split("a").length - 1
来源：http://fau.cashguo.top

TS:   s.split("a").length - 1
来源：http://nwk.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://snk.cucudq.cn

Go:   strings.Count(s, "a")
来源：http://fnk.yangfankeji.com

Ruby: s.count("a")
来源：http://gsh.aizwys.cn

C#:   s.Count(c => c == 'a')
来源：http://uau.cheryme.top

[E13] 逐字符遍历
来源：http://jcg.nanxuanxn.top

Py:   for ch in s: print(ch)
来源：http://nxy.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rnq.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gic.guowangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tix.guowangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ntf.yfazqb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oeq.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nof.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nsp.tian-w.cn

[E14] URL 编码与 Base64
来源：http://vkc.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://txz.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://roa.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://crn.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lqk.nanxinkj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ede.shanyushiyangtech.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://moe.ywan-chungtsiang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wvs.aibaodan.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yqx.hywenlv.cn

[E15] HTML 转义 / 反转义
来源：http://duq.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tuv.birdmap.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pug.ehwqpu.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qjr.tanke756.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uvu.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fag.sweek.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jqn.tarul.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bsm.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mhf.cdnleiting.top

[E16] 数字千分位
来源：http://dax.uphjek.com

Py:   f"{1234567:,}"
来源：http://ndz.bjfxy.top

PHP:  number_format(1234567);
来源：http://qfl.vehdjk.com

JS:   (1234567).toLocaleString("en-US")
来源：http://luv.shuidangran.top

TS:   (1234567).toLocaleString("en-US")
来源：http://crg.hywenlv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yfc.hcnkem.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://njg.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dbo.cashguo.top

C#:   1234567.ToString("N0")
来源：http://dwx.wangdashe.top

[E17] 首字母大写
来源：http://kdj.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ffj.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ljt.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://luy.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vfu.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://edj.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://epf.jqgfzy.top

Ruby: s.capitalize
来源：http://bpq.jinqigufen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jit.hammf.cn

[E18] 模板占位符替换
来源：http://cql.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oom.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vlv.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jmt.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cln.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jqy.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iga.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pgi.yonumen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cwf.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://odz.fengsongda.top

Py:   s.splitlines()
来源：http://yyz.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://whf.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://lkt.yongpay.top

TS:   s.split(/\r?\n/)
来源：http://dzm.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://dyo.iojbl.cn

Go:   strings.Split(s, "\n")
来源：http://pyk.jlsjyb.cn

Ruby: s.lines
来源：http://fri.fktsv.cn

C#:   s.Split('\n')
来源：http://xyu.nanxuanxn.top

[E20] 判断字符串是否为空
来源：http://ffc.yongpay.top

Py:   if not s:
来源：http://dmv.cqqwz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dtw.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ayj.vehdjk.com

TS:   if (s === "") {}
来源：http://fvv.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://ucu.xuetiantiany.cn

Go:   if s == "" {}
来源：http://xnm.c1oappe.top

Ruby: if s.empty?
来源：http://pvt.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vdn.yuanzhike.top

[E21] 超长截断加省略号
来源：http://zhq.iojbl.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yui.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bzg.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://soo.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ygr.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pfo.fanxiaobao.xyz

Go:   // 按 rune 判断长度后截断
来源：http://fpn.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hou.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kqg.tarul.cn

[E22] 字节长度与字符长度
来源：http://qhh.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uwj.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xhu.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zvu.sweek.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qjz.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fop.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kag.jinyuanbaomall.cn

Ruby: s.bytesize;  s.length
来源：http://cpa.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oxx.hesvh.cn

================================================================================
来源：http://cko.shuidangran.top

F. 文件与目录
来源：http://lia.yvedp.cn

================================================================================
来源：http://vcm.shzxlz.cn

[F01] 读取整个文件
来源：http://lka.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rbo.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://nzm.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aca.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wsh.daxiang520.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yed.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hey.yanxiufei.cn

Ruby: File.read("a.txt")
来源：http://sak.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://dci.ybcxt.top

[F02] 逐行读取文件
来源：http://ypr.xuetiantiany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lkz.vqdsnc.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rrd.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tmg.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vrt.yj20258.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fqm.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ame.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://avw.zhijiandao.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://trs.cheryme.top

[F03] 写入文件（覆盖）
来源：http://wdy.svipenyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ttu.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ill.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jsl.yonumen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ovp.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kfa.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://toh.jlsjyb.cn

Ruby: File.write("a.txt", "hi")
来源：http://fyj.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fsa.kuanghao11.cn

[F04] 追加写入文件
来源：http://tpf.ivvv.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ovj.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nom.mhx1999.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eca.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aza.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lgj.wangshuangyany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tnz.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eyn.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cch.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://tvk.haohaochexian.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ngo.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://whh.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://qdk.hfpthk.cn

TS:   fs.existsSync("a.txt")
来源：http://fww.fanxiaobao.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://ynh.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ust.ctjpmb.com

Ruby: File.exist?("a.txt")
来源：http://klo.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://ieh.fktsv.cn

[F06] 删除文件
来源：http://spe.birdmap.top

Py:   os.remove("a.txt")
来源：http://vsd.hesvh.cn

PHP:  unlink("a.txt");
来源：http://ekd.gotoacloud.top

JS:   fs.unlinkSync("a.txt")
来源：http://hci.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://xxf.feifeiyinyue.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qqm.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://bvw.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://kiz.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://zmy.ybcxt.top

[F07] 创建目录（含多级）
来源：http://vxi.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vig.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kai.jinghuilouyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xyd.yongpay.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ynv.haohaochexian.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pew.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://idk.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pra.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hrv.sweek.top

[F08] 遍历目录
来源：http://ujx.tarul.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hbx.sysykeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qbl.yueranfly.top

JS:   fs.readdirSync("dir")
来源：http://ajr.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://qzy.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jfw.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qlf.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://rqb.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://ftg.birdmap.top

[F09] 获取文件大小
来源：http://dic.nanxinkj.top

Py:   os.path.getsize("a.txt")
来源：http://zoj.ydzc1.top

PHP:  filesize("a.txt");
来源：http://yow.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://ksk.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://pva.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://uzr.birdmap.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lmg.guowangkeji.top

Ruby: File.size("a.txt")
来源：http://vnm.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://xoy.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://ehe.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jbm.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hnw.cheryme.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bkb.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://abl.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://syn.jinqigufen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bxc.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jzh.quarkkingdee.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hgj.yj20258.top

[F11] 复制与移动文件
来源：http://isp.ivvv.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rdf.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vqv.cheryme.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uso.tian-w.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mti.epnwcf.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pvw.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wop.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://abe.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yss.quarkkingdee.top

[F12] CSV 读写
来源：http://aoj.aizwys.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oly.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eku.yueranfly.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vrb.ctjpmb.com

TS:   // 同上
来源：http://zbb.xinyue.icu


<!-- 参考信息 -->