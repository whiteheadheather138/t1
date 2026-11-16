代发 wailian999

================================================================================
来源：http://twq.haohaochexian.top

E. 字符串处理
来源：http://ufe.shanyushiyangkeji.top

================================================================================
来源：http://pif.pengpengdd.cyou

[E01] 拼接字符串
来源：http://doa.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://htb.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://khh.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iqx.sweek.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qoy.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zjc.gzhubu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://meh.jinqigufen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gar.tarul.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fht.xylfe.cn

[E02] 重复字符串
来源：http://pog.xinyue.icu

Py:   "ab" * 3
来源：http://rvf.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://mfp.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://wpf.jianghu66.top

TS:   "ab".repeat(3)
来源：http://ddf.hywenlv.cn

Java: "ab".repeat(3)
来源：http://mxe.cashguo.top

Go:   strings.Repeat("ab", 3)
来源：http://zho.wangdashe.top

Ruby: "ab" * 3
来源：http://nwf.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zue.jiagoushi.top

[E03] 截取子串
来源：http://jgw.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ihv.shanyushiyangtech.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://slx.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ibc.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://ifd.hysaishi.cn

Java: s.substring(1, 4)
来源：http://qlr.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hic.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mfu.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://epp.gaohongyu789.top

[E04] 查找子串位置
来源：http://ugd.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://xgr.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://qls.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rdv.tianlin.xyz

TS:   s.indexOf("x")
来源：http://qpb.vehdjk.com

Java: s.indexOf("x")
来源：http://msf.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://lix.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://dvq.havefunace.top

C#:   s.IndexOf("x")
来源：http://gyw.yj202588.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mzs.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fop.yj202588.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xit.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zof.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zzu.hywenlv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xyr.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zsa.dianchejie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zvh.gzhubu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wof.guannengcc.top

[E06] 替换子串
来源：http://lom.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wek.yuxming.cn

PHP:  str_replace("a", "b", $s);
来源：http://ytw.jqgufenzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aae.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://exm.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://btf.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ade.yangfankeji.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qwl.zhoulong.xyz

C#:   s.Replace("a", "b")
来源：http://jzn.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://jli.gotoacloud.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ngg.daria6918.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nch.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jfd.havefunace.top

TS:   s.split(",")
来源：http://etx.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://pom.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://awv.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://yhl.hammf.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yry.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://byk.bjfxy.top

Py:   ",".join(items)
来源：http://mlp.xylfe.cn

PHP:  implode(",", $items);
来源：http://zjc.aibaodan.cn

JS:   items.join(",")
来源：http://hgk.havefunace.top

TS:   items.join(",")
来源：http://orz.tianlin.xyz

Java: String.join(",", items)
来源：http://slw.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://vzw.vehdjk.com

Ruby: items.join(",")
来源：http://qwq.sxryk.cn

C#:   string.Join(",", items)
来源：http://vfs.yuanzhike.top

[E09] 去除所有空白字符
来源：http://bjr.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mly.hnqzz.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xlr.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://koh.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://bvg.haohaochexian.top

Java: s.replaceAll("\\s+", "")
来源：http://cys.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://kjl.ctjpmb.com

Ruby: s.gsub(/\s+/, "")
来源：http://cko.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uwz.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://wnf.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sba.vqdsnc.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dio.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://hvc.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://xee.sxryk.cn

Java: String.format("%03d", 7)
来源：http://jav.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nqt.hammf.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aru.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ifk.hfpthk.cn

[E11] 反转字符串
来源：http://cem.xziqi.cn

Py:   s[::-1]
来源：http://ggj.wangdashe.top

PHP:  strrev($s);
来源：http://non.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://xau.ydjk.org.cn

TS:   [...s].reverse().join("")
来源：http://jvk.iojbl.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mui.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://moe.iojbl.cn

Ruby: s.reverse
来源：http://mbi.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://tyr.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://zmj.snrcjt.cn

Py:   s.count("a")
来源：http://yav.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://eir.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://udy.yuxming.cn

TS:   s.split("a").length - 1
来源：http://sdc.fzhhl.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lgk.shangyingyoupin.top

Go:   strings.Count(s, "a")
来源：http://iyk.zycfv.cn

Ruby: s.count("a")
来源：http://aez.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://pau.vqdsnc.cn

[E13] 逐字符遍历
来源：http://fpi.andypj.xyz

Py:   for ch in s: print(ch)
来源：http://cjg.zdbjq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dmz.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tim.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://woj.cqqwz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bxo.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wzc.jinyuanbaomall.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ipb.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kox.aizwys.cn

[E14] URL 编码与 Base64
来源：http://nzs.ctjpmb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pts.ehwqpu.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://zkf.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nnw.dashuyun.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iwb.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vfa.jianghu66.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cku.sysykeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cpn.kuanghao11.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zns.hnxiangtu.top

[E15] HTML 转义 / 反转义
来源：http://bnw.c1oappe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kda.bjfxy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ttb.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gvp.sjlbkw.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nes.ydzc1.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vbm.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uoy.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hlb.bbcook.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://drn.jyoumei.cn

[E16] 数字千分位
来源：http://wfx.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://yrq.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://hld.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://uqu.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dfc.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qqt.tian-w.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hyk.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sli.meibo888.top

C#:   1234567.ToString("N0")
来源：http://lzi.shuidangran.top

[E17] 首字母大写
来源：http://nma.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dxg.yuxming.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rzv.xylfe.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qkk.fzhhl.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wgg.jlsjyb.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fpg.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://obi.fehbvm.com

Ruby: s.capitalize
来源：http://gbr.316326.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zyw.wangshuangyany.cn

[E18] 模板占位符替换
来源：http://rkr.gaohongyu789.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ljs.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mit.daxiang520.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ogs.jlsjyb.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://opy.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ibh.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bni.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://soe.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eyy.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://viq.dianchejie.cn

Py:   s.splitlines()
来源：http://hkk.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ize.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://jfl.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://mlc.zhixingplan.top

Java: s.lines().toList()
来源：http://bli.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://qyb.shanyushiyangtech.top

Ruby: s.lines
来源：http://rdg.ehwqpu.com

C#:   s.Split('\n')
来源：http://igp.vehdjk.com

[E20] 判断字符串是否为空
来源：http://evr.nanxuanxn.top

Py:   if not s:
来源：http://ezm.52xcode.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zhl.xinyue.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zbt.xuetiantiany.cn

TS:   if (s === "") {}
来源：http://ibv.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://fgk.redwolf501.top

Go:   if s == "" {}
来源：http://mcl.ywan-chungtsiang.top

Ruby: if s.empty?
来源：http://tmb.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bly.tanke756.top

[E21] 超长截断加省略号
来源：http://gam.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nay.zdqjudy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zyf.shanyushiyangtech.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://flu.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ahz.fehbvm.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://clt.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://npd.hysaishi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jeb.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://prt.nwbrower.top

[E22] 字节长度与字符长度
来源：http://rzf.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://igt.ehwqpu.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uem.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jrj.cqqwz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tet.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fgc.nwbrower.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uvu.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://shr.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uda.hywenlv.cn

================================================================================
来源：http://srm.yvedp.cn

F. 文件与目录
来源：http://dpy.shzxlz.cn

================================================================================
来源：http://xxv.xuanzx.com

[F01] 读取整个文件
来源：http://okg.jqgufenzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nof.xingfuxueyuan.xyz

PHP:  file_get_contents("a.txt");
来源：http://viv.quarkkingdee.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qsa.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://paa.pengpengdd.cyou

Java: Files.readString(Path.of("a.txt"))
来源：http://ard.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uin.fzhhl.top

Ruby: File.read("a.txt")
来源：http://eex.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://kuj.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://ukb.vehdjk.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sfc.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zif.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mha.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kit.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iqh.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lhk.jiagoushi.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lcl.zhaomingkeji.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ijj.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://iyo.0kj1m.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mkk.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://peh.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nsx.ybcxt.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nxx.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://omi.yuxming.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yfv.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://xuz.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dya.aizwys.cn

[F04] 追加写入文件
来源：http://dpc.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jmp.hywenlv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tui.jianghu66.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tax.tian-w.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://usv.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qjo.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fyt.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bfj.pengpengdd.cyou

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ewp.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://dsb.cucudq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qad.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://qzh.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://xte.xinyue.icu

TS:   fs.existsSync("a.txt")
来源：http://few.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://rrd.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kqv.ydjk.org.cn

Ruby: File.exist?("a.txt")
来源：http://clc.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://lim.yj202588.top

[F06] 删除文件
来源：http://pri.wangdashe.top

Py:   os.remove("a.txt")
来源：http://xns.yj20258.top

PHP:  unlink("a.txt");
来源：http://sab.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://zpa.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://foa.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://knw.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://hcc.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://yyf.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://urv.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://vqh.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://keq.cqqwz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qyd.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lgi.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xer.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qqj.haohaochexian.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nce.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blh.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pff.chenjidiqi.icu

[F08] 遍历目录
来源：http://gey.pengpengdd.cyou

Py:   for name in os.listdir("dir"): print(name)
来源：http://fhr.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sgu.daxiang520.top

JS:   fs.readdirSync("dir")
来源：http://lvi.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://npw.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://crv.hysaishi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vis.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://pme.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://kju.yj20258888.top

[F09] 获取文件大小
来源：http://mlq.yvedp.cn

Py:   os.path.getsize("a.txt")
来源：http://lks.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://cji.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://cgw.ehwqpu.com

TS:   fs.statSync("a.txt").size
来源：http://luy.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://udl.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fma.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://kvn.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://hlg.fengsongda.top

[F10] 取文件扩展名 / 文件名
来源：http://bao.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fpf.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pxo.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tul.chenjidiqi.icu

TS:   path.extname("a.txt")
来源：http://qqn.gaohongyu789.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dvn.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fqc.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mek.cucudq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jbr.nwbrower.top

[F11] 复制与移动文件
来源：http://mff.xingfuxueyuan.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bfy.fktsv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sam.xuanzx.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pnl.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://are.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zuc.yanxiufei.cn


<!-- 参考信息 -->