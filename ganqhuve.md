代发 wailian999

================================================================================
来源：http://odn.jqgfzy.top

E. 字符串处理
来源：http://mgv.ydzc1.top

================================================================================
来源：http://wlr.snrcjt.cn

[E01] 拼接字符串
来源：http://vuu.meibo888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zro.andypj.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lbk.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bez.ywan-chungtsiang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vag.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ybf.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oba.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bou.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uod.zdqjudy.top

[E02] 重复字符串
来源：http://yqo.xingfuxueyuan.xyz

Py:   "ab" * 3
来源：http://sni.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://hcb.uphjek.com

JS:   "ab".repeat(3)
来源：http://wwz.ctjpmb.com

TS:   "ab".repeat(3)
来源：http://wps.shzxlz.cn

Java: "ab".repeat(3)
来源：http://vis.hongshengwenyu.top

Go:   strings.Repeat("ab", 3)
来源：http://obp.yj20258888.top

Ruby: "ab" * 3
来源：http://sdd.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bcu.zycfv.cn

[E03] 截取子串
来源：http://ftz.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bbd.xziqi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lev.sysykeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://brh.ivvv.top

TS:   s.slice(1, 4)
来源：http://xyw.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://wxg.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wsh.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://ssr.sweek.top

C#:   s.Substring(1, 3)
来源：http://vvm.cucudq.cn

[E04] 查找子串位置
来源：http://wgv.epnwcf.com

Py:   s.find("x");  s.index("x")
来源：http://bih.cqqwz.cn

PHP:  strpos($s, "x");
来源：http://ymw.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oyu.jinqigufen.top

TS:   s.indexOf("x")
来源：http://lrv.gaohongyu789.top

Java: s.indexOf("x")
来源：http://dwp.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://lpb.sxryk.cn

Ruby: s.index("x")
来源：http://rsk.0kj1m.cn

C#:   s.IndexOf("x")
来源：http://hyt.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zhc.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vwm.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ske.chenlongwang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wha.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://zyj.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aaj.quarkkingdee.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bna.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yeh.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://otv.hesvh.cn

[E06] 替换子串
来源：http://hbr.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ozb.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://hwc.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fvd.xingfuxueyuan.xyz

TS:   s.replaceAll("a", "b")
来源：http://xrr.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iat.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://imw.hfpthk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qlt.cheryme.top

C#:   s.Replace("a", "b")
来源：http://unx.nanxinkj.top

[E07] 按分隔符拆分
来源：http://lfe.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yyp.chenjidiqi.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iqe.zhixingplan.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ako.nwbrower.top

TS:   s.split(",")
来源：http://nae.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://wng.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kpz.tanke756.top

Ruby: s.split(",");  s.split
来源：http://lel.xuetiantiany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xjp.shuidangran.top

[E08] 数组按分隔符合并
来源：http://zkh.316326.xyz

Py:   ",".join(items)
来源：http://leo.bjfxy.top

PHP:  implode(",", $items);
来源：http://tre.yvedp.cn

JS:   items.join(",")
来源：http://nza.gzhubu.top

TS:   items.join(",")
来源：http://vji.ivvv.top

Java: String.join(",", items)
来源：http://tct.yj202588.top

Go:   strings.Join(items, ",")
来源：http://yxk.bjfxy.top

Ruby: items.join(",")
来源：http://qdz.52xcode.cn

C#:   string.Join(",", items)
来源：http://ojm.svipenyu.cn

[E09] 去除所有空白字符
来源：http://hni.yfazqb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rwo.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://glc.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://jic.hongshengwenyu.top

TS:   s.replace(/\s+/g, "")
来源：http://fno.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://xau.zycfv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ckf.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://dje.hongshengwenyu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qgl.wangdashe.top

[E10] 左侧补零 / 定长填充
来源：http://zum.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://abm.nwbrower.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zhc.0kj1m.cn

JS:   "7".padStart(3, "0")
来源：http://wjh.ydzc1.top

TS:   "7".padStart(3, "0")
来源：http://vun.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://fif.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oxy.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wsf.ivvv.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bva.xinyue.icu

[E11] 反转字符串
来源：http://baj.havefunace.top

Py:   s[::-1]
来源：http://hzt.zhengqikj.top

PHP:  strrev($s);
来源：http://rpq.yvedp.cn

JS:   [...s].reverse().join("")
来源：http://iyo.ydjk.org.cn

TS:   [...s].reverse().join("")
来源：http://pop.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://oiz.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vxr.ybcxt.top

Ruby: s.reverse
来源：http://oiu.hnxiangtu.top

C#:   new string(s.Reverse().ToArray())
来源：http://fgu.uphjek.com

[E12] 统计某字符出现次数
来源：http://qow.yj202588.top

Py:   s.count("a")
来源：http://yif.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://gqf.andypj.xyz

JS:   s.split("a").length - 1
来源：http://xkq.tarul.cn

TS:   s.split("a").length - 1
来源：http://hth.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ezg.tianlin.xyz

Go:   strings.Count(s, "a")
来源：http://shw.ybcxt.top

Ruby: s.count("a")
来源：http://vtx.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://qvu.9152youxi.cn

[E13] 逐字符遍历
来源：http://thd.tarul.cn

Py:   for ch in s: print(ch)
来源：http://ixs.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fek.yj20258888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tnv.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dtq.cqqwz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://siy.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gwy.jinyuanbaomall.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vsh.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kxl.cashguo.top

[E14] URL 编码与 Base64
来源：http://okh.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mmp.ehwqpu.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://fzf.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sim.redwolf501.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kyv.cashguo.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rdy.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hmr.xylfe.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jdf.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://khl.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://liu.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://obl.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gao.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ezn.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lnv.316326.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://emb.hammf.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://obg.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mzi.yuanzhike.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zxz.guannengcc.top

[E16] 数字千分位
来源：http://pth.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://lsy.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://nbz.zhongyouzk.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vpy.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qbq.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eyx.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wjy.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ugp.jiagoushi.top

C#:   1234567.ToString("N0")
来源：http://gdo.hnqzz.top

[E17] 首字母大写
来源：http://ons.fktsv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vkh.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://osx.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kxe.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vrj.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vxd.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mdo.dianchejie.cn

Ruby: s.capitalize
来源：http://kuq.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://brz.xylfe.cn

[E18] 模板占位符替换
来源：http://xdb.nanxinkj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nqr.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zfx.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jrj.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://nhe.jqgufenzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rtw.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jnp.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ocv.ybcxt.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pnm.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://bjj.jinqigfzy.top

Py:   s.splitlines()
来源：http://scb.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yvn.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://yzc.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://hjv.tarul.cn

Java: s.lines().toList()
来源：http://jcs.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://prn.pengpengdd.cyou

Ruby: s.lines
来源：http://zyv.fengsongda.top

C#:   s.Split('\n')
来源：http://wqp.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://yob.nwbrower.top

Py:   if not s:
来源：http://vmd.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bcn.sxryk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://adu.cashguo.top

TS:   if (s === "") {}
来源：http://ytk.cashguo.top

Java: if (s.isEmpty()) {}
来源：http://yui.bjfxy.top

Go:   if s == "" {}
来源：http://oyx.andypj.xyz

Ruby: if s.empty?
来源：http://uqh.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ebc.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://kun.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aga.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mfp.jinqigfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://swe.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lvt.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mam.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://tsw.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://huz.zhiwuduotai.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://goj.cqqwz.cn

[E22] 字节长度与字符长度
来源：http://mkg.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mlr.zhaomingkeji.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xyf.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vtt.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://awe.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://czn.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ovx.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://jne.cdnleiting.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pdz.xziqi.cn

================================================================================
来源：http://ovo.jyoumei.cn

F. 文件与目录
来源：http://dhg.shangyingyoupin.top

================================================================================
来源：http://siv.haohaochexian.top

[F01] 读取整个文件
来源：http://hos.jinyuanbaomall.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fqx.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://ipf.zycfv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xtf.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zdq.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mqg.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qfp.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://wtr.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://xox.316326.xyz

[F02] 逐行读取文件
来源：http://gmn.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ixi.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dht.jlsjyb.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vcc.zhaomingkeji.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bfo.xingfuxueyuan.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uuo.iojbl.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xuv.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lhv.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mze.dianchejie.cn

[F03] 写入文件（覆盖）
来源：http://tfh.cheryme.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mzd.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jtx.chenzaomai.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ajm.yonumen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tyv.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tci.zhengqikj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://daq.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://ymm.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wfc.tian-w.cn

[F04] 追加写入文件
来源：http://zyw.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kpm.sysykeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://shw.316326.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://svh.yj20258888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pka.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ggy.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qhe.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uvx.yuxming.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ckt.daxiang520.top

[F05] 判断文件或目录是否存在
来源：http://xmz.vehdjk.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://otj.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://sif.svipenyu.cn

JS:   fs.existsSync("a.txt")
来源：http://wlc.quarkkingdee.top

TS:   fs.existsSync("a.txt")
来源：http://qop.meibo888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vxu.yanxiufei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pba.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://rkh.yvedp.cn

C#:   File.Exists("a.txt")
来源：http://jtd.yvedp.cn

[F06] 删除文件
来源：http://rkk.cheryme.top

Py:   os.remove("a.txt")
来源：http://cge.cheryme.top

PHP:  unlink("a.txt");
来源：http://eyb.zhixingplan.top

JS:   fs.unlinkSync("a.txt")
来源：http://mqt.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://hoh.jiagoushi.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mwq.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://dmo.c1oappe.top

Ruby: File.delete("a.txt")
来源：http://zpk.pycfn.com

C#:   File.Delete("a.txt");
来源：http://xni.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://mgs.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kdm.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yik.hesvh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dhl.sufxvd.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dct.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mku.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pfz.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://osp.hesvh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xci.fehbvm.com

[F08] 遍历目录
来源：http://ayv.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ohy.zhengqikj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mxe.quarkkingdee.top

JS:   fs.readdirSync("dir")
来源：http://pan.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://vzl.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qmb.fzhhl.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nea.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://bws.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://mcp.ybcxt.top

[F09] 获取文件大小
来源：http://vib.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://dxr.hammf.cn

PHP:  filesize("a.txt");
来源：http://afc.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://vww.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://dvn.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://typ.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zsr.zycfv.cn

Ruby: File.size("a.txt")
来源：http://rao.jlsjyb.cn

C#:   new FileInfo("a.txt").Length
来源：http://kpm.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://wha.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vny.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mps.tian-w.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://svy.redwolf501.top

TS:   path.extname("a.txt")
来源：http://bkj.hongshengwenyu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vgz.ydjk.org.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nno.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nqj.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ivr.aibaodan.cn

[F11] 复制与移动文件
来源：http://oxt.dashuyun.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mpg.smart0.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sna.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ctf.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://niu.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jsu.hysaishi.cn


<!-- 参考信息 -->