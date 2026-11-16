代发 wailian999

Java: String.join(", ", list)
来源：http://nif.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://ztl.birdmap.top

Ruby: arr.join(", ")
来源：http://pex.fzhhl.top

C#:   string.Join(", ", list)
来源：http://xgl.xuanzx.com

================================================================================
来源：http://izv.yanxiufei.cn

E. 字符串处理
来源：http://vpw.tian-w.cn

================================================================================
来源：http://jnr.wangshuangyany.cn

[E01] 拼接字符串
来源：http://igw.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wsw.316326.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gqc.nanxuanxn.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dfn.hywenlv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sdb.cqqwz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qtw.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hlw.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zrz.zhaomingkeji.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wje.zdqjudy.top

[E02] 重复字符串
来源：http://jlg.chenjidiqi.icu

Py:   "ab" * 3
来源：http://cib.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://ocp.ppjwa.cn

JS:   "ab".repeat(3)
来源：http://scm.xuanzx.com

TS:   "ab".repeat(3)
来源：http://tyb.yj202588.top

Java: "ab".repeat(3)
来源：http://hxt.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://tab.snrcjt.cn

Ruby: "ab" * 3
来源：http://hyi.c1oappe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cdx.redwolf501.top

[E03] 截取子串
来源：http://mgi.c1oappe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mti.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zpx.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xtj.cashguo.top

TS:   s.slice(1, 4)
来源：http://mgi.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://vkg.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qra.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://gwx.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://jbz.fktsv.cn

[E04] 查找子串位置
来源：http://tds.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://lry.tanke756.top

PHP:  strpos($s, "x");
来源：http://wwr.yj20258888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://muv.hesvh.cn

TS:   s.indexOf("x")
来源：http://pzb.feifeiyinyue.top

Java: s.indexOf("x")
来源：http://ttd.meibo888.top

Go:   strings.Index(s, "x")
来源：http://apf.fzhhl.top

Ruby: s.index("x")
来源：http://edo.ybcxt.top

C#:   s.IndexOf("x")
来源：http://dbj.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wtx.jqgufenzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lqq.yanxiufei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xza.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yse.gzhubu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rkt.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mre.yj20258.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://csu.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yty.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tuc.quarkkingdee.top

[E06] 替换子串
来源：http://wnj.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cby.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://tlk.vqdsnc.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qjn.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://epd.zdbjq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fpy.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lcw.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://luz.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://glr.hammf.cn

[E07] 按分隔符拆分
来源：http://cwl.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ylb.redwolf501.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gpq.cucudq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dnb.vehdjk.com

TS:   s.split(",")
来源：http://ljg.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://blc.ehwqpu.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oal.guowangkeji.top

Ruby: s.split(",");  s.split
来源：http://xmt.xziqi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eam.guannengcc.top

[E08] 数组按分隔符合并
来源：http://dwy.yj202588.top

Py:   ",".join(items)
来源：http://awh.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://dyf.dashuyun.cn

JS:   items.join(",")
来源：http://gzj.hywenlv.cn

TS:   items.join(",")
来源：http://fva.xziqi.cn

Java: String.join(",", items)
来源：http://jtc.fengsongda.top

Go:   strings.Join(items, ",")
来源：http://vog.andypj.xyz

Ruby: items.join(",")
来源：http://gos.hesvh.cn

C#:   string.Join(",", items)
来源：http://jdc.tarul.cn

[E09] 去除所有空白字符
来源：http://ywx.zycfv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://loh.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mob.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://dqh.feifeiyinyue.top

TS:   s.replace(/\s+/g, "")
来源：http://yer.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://eru.xinyue.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://lgk.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zmv.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ucu.shanyushiyangtech.top

[E10] 左侧补零 / 定长填充
来源：http://mln.jyoumei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lxa.xuetiantiany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eru.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://izj.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://toj.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://umr.tian-w.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://aab.sjlbkw.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ejv.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ikq.cqqwz.cn

[E11] 反转字符串
来源：http://hsu.tarul.cn

Py:   s[::-1]
来源：http://imf.nwbrower.top

PHP:  strrev($s);
来源：http://hpf.shangyingyoupin.top

JS:   [...s].reverse().join("")
来源：http://sty.yvedp.cn

TS:   [...s].reverse().join("")
来源：http://bmj.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://szr.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pav.hywenlv.cn

Ruby: s.reverse
来源：http://fxl.redwolf501.top

C#:   new string(s.Reverse().ToArray())
来源：http://zji.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://hzh.gaohongyu789.top

Py:   s.count("a")
来源：http://yni.yueranfly.top

PHP:  substr_count($s, "a");
来源：http://pbx.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://nls.sxryk.cn

TS:   s.split("a").length - 1
来源：http://dux.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vig.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://irr.yj20258888.top

Ruby: s.count("a")
来源：http://mqz.zhaomingkeji.xyz

C#:   s.Count(c => c == 'a')
来源：http://czf.bbcook.cn

[E13] 逐字符遍历
来源：http://gua.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://krd.zdbjq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yzk.jinyuanbaomall.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eoo.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://muz.jinghuilouyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fkj.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gxj.cashguo.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qvs.fehbvm.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://riy.yvedp.cn

[E14] URL 编码与 Base64
来源：http://lxk.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fcq.jinyuanbaomall.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tkk.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zcj.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uif.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gqc.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nus.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eoe.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xql.nanxinkj.top

[E15] HTML 转义 / 反转义
来源：http://tml.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bxp.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://abh.ybcxt.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fhp.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tdt.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kvi.shuidangran.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mls.pycfn.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hqp.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pyg.zhixingplan.top

[E16] 数字千分位
来源：http://wtm.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://vdz.sxryk.cn

PHP:  number_format(1234567);
来源：http://bac.fzhhl.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lns.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zkp.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mfl.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yip.0kj1m.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://knv.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://xeb.yfazqb.com

[E17] 首字母大写
来源：http://mic.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ors.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ktc.feifeiyinyue.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kye.dianchejie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cfg.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jqv.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wtk.iojbl.cn

Ruby: s.capitalize
来源：http://grt.daria6918.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://spy.bbcook.cn

[E18] 模板占位符替换
来源：http://npp.gzhubu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mvt.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jfe.tianlin.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://oon.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gdz.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gxy.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xkr.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oov.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tys.zdbjq.cn

[E19] 多行文本按行拆分
来源：http://mto.yfazqb.com

Py:   s.splitlines()
来源：http://nkz.ivvv.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vxo.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://mln.jlsjyb.cn

TS:   s.split(/\r?\n/)
来源：http://nqj.hnxiangtu.top

Java: s.lines().toList()
来源：http://vkh.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://pev.sjlbkw.cn

Ruby: s.lines
来源：http://hun.cashguo.top

C#:   s.Split('\n')
来源：http://fhu.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://abh.svipenyu.cn

Py:   if not s:
来源：http://ehf.ywan-chungtsiang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wag.shuidangran.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gyd.sjlbkw.cn

TS:   if (s === "") {}
来源：http://kbm.chenjidiqi.icu

Java: if (s.isEmpty()) {}
来源：http://uil.chenjidiqi.icu

Go:   if s == "" {}
来源：http://qho.sxryk.cn

Ruby: if s.empty?
来源：http://uch.uphjek.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vfv.hywenlv.cn

[E21] 超长截断加省略号
来源：http://hnr.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qmx.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hbi.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hqk.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cnc.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://grz.zhijiandao.cn

Go:   // 按 rune 判断长度后截断
来源：http://lry.xuanzx.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sif.cashguo.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uxc.hammf.cn

[E22] 字节长度与字符长度
来源：http://wao.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kgn.yuxming.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nrt.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lfb.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pdu.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cvv.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://biq.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://jzg.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://may.snrcjt.cn

================================================================================
来源：http://lwp.ybcxt.top

F. 文件与目录
来源：http://uqr.wangshuangyany.cn

================================================================================
来源：http://rjt.uphjek.com

[F01] 读取整个文件
来源：http://cvy.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ufq.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://xvr.chenzaomai.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lnd.zhiwuduotai.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vcs.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://erv.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yzs.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://dwd.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://qke.c1oappe.top

[F02] 逐行读取文件
来源：http://muw.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xiu.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://led.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ldd.aizwys.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eui.ydzc1.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aoo.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ils.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nwm.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qll.pycfn.com

[F03] 写入文件（覆盖）
来源：http://xtk.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yjl.hnqzz.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yru.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pvd.meibo888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rdi.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zao.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://waw.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://wbu.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xsx.zhijiandao.cn

[F04] 追加写入文件
来源：http://zwy.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://glk.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fte.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uwd.yj202588.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qqi.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ftd.yj202588.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jaq.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tcj.hywenlv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mwx.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://pzo.cdnleiting.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ofc.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://fwm.sufxvd.cn

JS:   fs.existsSync("a.txt")
来源：http://xlf.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://pgn.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://env.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pae.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://dpz.zhengqikj.top

C#:   File.Exists("a.txt")
来源：http://xmy.c1oappe.top

[F06] 删除文件
来源：http://pim.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://cmv.cheryme.top

PHP:  unlink("a.txt");
来源：http://cte.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://jjx.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://uak.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://usr.jqgfzy.top

Go:   os.Remove("a.txt")
来源：http://vsw.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://dpf.yj20258888.top

C#:   File.Delete("a.txt");
来源：http://nhw.yongpay.top

[F07] 创建目录（含多级）
来源：http://rpf.jinqigfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kkt.kuanghao11.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wiq.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lxy.shuidangran.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dwo.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bar.hcnkem.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nnw.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wgl.svipenyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ayo.tian-w.cn

[F08] 遍历目录
来源：http://nuu.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xpg.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://udj.hongshengwenyu.top

JS:   fs.readdirSync("dir")
来源：http://hjs.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://fgw.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tlw.redwolf501.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cwy.gzhubu.top

Ruby: Dir.children("dir")
来源：http://nnd.redwolf501.top

C#:   Directory.GetFiles("dir")
来源：http://qmv.tarul.cn

[F09] 获取文件大小
来源：http://yql.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://jqg.fzhhl.top

PHP:  filesize("a.txt");
来源：http://yux.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://ggu.shangyingyoupin.top

TS:   fs.statSync("a.txt").size
来源：http://jen.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://ddj.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pmj.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://jlc.guowangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://rkd.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://nye.aibaodan.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://czz.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pwq.zhiwuduotai.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fwz.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://ibq.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fqa.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kkg.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fbg.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cjc.zhengqikj.top

[F11] 复制与移动文件
来源：http://the.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rvq.zhengqikj.top


<!-- 参考信息 -->