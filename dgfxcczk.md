代发 wailian999

================================================================================
来源：http://mof.yj20258888.top

E. 字符串处理
来源：http://bel.mhx1999.top

================================================================================
来源：http://hzg.zycfv.cn

[E01] 拼接字符串
来源：http://lwl.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uzr.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gkt.pengpengdd.cyou

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://txm.zhijiandao.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eav.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nie.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fmw.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lsq.yongpay.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qbz.zhongyouzk.top

[E02] 重复字符串
来源：http://whk.smart0.xyz

Py:   "ab" * 3
来源：http://jdd.gaohongyu789.top

PHP:  str_repeat("ab", 3);
来源：http://eyq.yj20258.top

JS:   "ab".repeat(3)
来源：http://zdd.hcnkem.com

TS:   "ab".repeat(3)
来源：http://dlu.cqqwz.cn

Java: "ab".repeat(3)
来源：http://ylz.yongpay.top

Go:   strings.Repeat("ab", 3)
来源：http://ejz.xuanzx.com

Ruby: "ab" * 3
来源：http://dko.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lpp.mhx1999.top

[E03] 截取子串
来源：http://gxr.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cmm.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sui.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fpk.52xcode.cn

TS:   s.slice(1, 4)
来源：http://bkl.cqqwz.cn

Java: s.substring(1, 4)
来源：http://zlt.nwbrower.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://frv.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://bsd.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://niv.zhijiandao.cn

[E04] 查找子串位置
来源：http://ohe.pycfn.com

Py:   s.find("x");  s.index("x")
来源：http://jhr.daxiang520.top

PHP:  strpos($s, "x");
来源：http://tnu.hysaishi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fpy.nanxuanxn.top

TS:   s.indexOf("x")
来源：http://fbn.redwolf501.top

Java: s.indexOf("x")
来源：http://qhx.yj202588.top

Go:   strings.Index(s, "x")
来源：http://anr.316326.xyz

Ruby: s.index("x")
来源：http://xay.hysaishi.cn

C#:   s.IndexOf("x")
来源：http://epu.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://zws.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uay.yfazqb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wpi.xylfe.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vsq.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zir.yanxiufei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://asx.zdbjq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wjp.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ubv.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://drd.cucudq.cn

[E06] 替换子串
来源：http://qbp.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yoc.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://hcz.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ylt.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://tsz.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tbl.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://svg.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qdu.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://opa.jinqigufen.top

[E07] 按分隔符拆分
来源：http://aho.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://smf.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pgr.svipenyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hpy.ydjk.org.cn

TS:   s.split(",")
来源：http://qyv.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hjz.zhijiandao.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dij.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://trx.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://grd.ybcxt.top

[E08] 数组按分隔符合并
来源：http://wjp.hammf.cn

Py:   ",".join(items)
来源：http://cbs.haohaochexian.top

PHP:  implode(",", $items);
来源：http://eqz.jinyuanbaomall.cn

JS:   items.join(",")
来源：http://kdf.iojbl.cn

TS:   items.join(",")
来源：http://bpv.yueranfly.top

Java: String.join(",", items)
来源：http://tof.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://xot.fengsongda.top

Ruby: items.join(",")
来源：http://izf.sufxvd.cn

C#:   string.Join(",", items)
来源：http://wjz.aizwys.cn

[E09] 去除所有空白字符
来源：http://kqm.haohaochexian.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://prl.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zgr.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://cnv.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://nwf.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://cte.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://mxe.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cfc.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bab.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://zpd.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qpr.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qmi.tarul.cn

JS:   "7".padStart(3, "0")
来源：http://fpe.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://gcw.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://ody.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://opq.cashguo.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qms.yvedp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rfq.tianlin.xyz

[E11] 反转字符串
来源：http://tgu.sweek.top

Py:   s[::-1]
来源：http://afo.xylfe.cn

PHP:  strrev($s);
来源：http://idz.shanyushiyangtech.top

JS:   [...s].reverse().join("")
来源：http://bce.uphjek.com

TS:   [...s].reverse().join("")
来源：http://myv.zhiwuduotai.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wgp.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://znz.chenjidiqi.icu

Ruby: s.reverse
来源：http://dmd.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://amc.bjfxy.top

[E12] 统计某字符出现次数
来源：http://dkf.fengsongda.top

Py:   s.count("a")
来源：http://vwz.yonumen.top

PHP:  substr_count($s, "a");
来源：http://bfq.aizwys.cn

JS:   s.split("a").length - 1
来源：http://hhi.xinyue.icu

TS:   s.split("a").length - 1
来源：http://cka.ydzc1.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xzt.ivvv.top

Go:   strings.Count(s, "a")
来源：http://rus.yfazqb.com

Ruby: s.count("a")
来源：http://sux.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://xzn.wangshuangyany.cn

[E13] 逐字符遍历
来源：http://anj.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://hqb.hnqzz.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ovj.jqgufenzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qez.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xlv.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ffl.xuetiantiany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jae.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qqo.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ujy.hcnkem.com

[E14] URL 编码与 Base64
来源：http://uuv.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xxp.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://adp.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gnw.svipenyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aae.jiagoushi.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rfc.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mtr.svipenyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://htc.aizwys.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gjz.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://nuf.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pbu.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yth.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rvl.ydjk.org.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kpc.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sjp.hnqzz.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wwf.chenjidiqi.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kzi.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rkn.yvedp.cn

[E16] 数字千分位
来源：http://rda.xylfe.cn

Py:   f"{1234567:,}"
来源：http://cml.xingfuxueyuan.xyz

PHP:  number_format(1234567);
来源：http://lxl.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://amx.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bme.birdmap.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qii.zhoulong.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ude.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ioh.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://nsb.pycfn.com

[E17] 首字母大写
来源：http://ufl.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lck.jiagoushi.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qzn.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tvz.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hht.hywenlv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yzu.svipenyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vpm.chenzaomai.com

Ruby: s.capitalize
来源：http://kvx.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jlr.gaohongyu789.top

[E18] 模板占位符替换
来源：http://shq.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://brg.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://por.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://naq.hnxiangtu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://grr.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hdm.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ylf.redwolf501.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bee.cheryme.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nte.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://tbq.daxiang520.top

Py:   s.splitlines()
来源：http://ykt.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mpx.zhijiandao.cn

JS:   s.split(/\r?\n/)
来源：http://yhh.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://pfa.hnxiangtu.top

Java: s.lines().toList()
来源：http://dva.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://lno.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://krz.zhijiandao.cn

C#:   s.Split('\n')
来源：http://rgm.zhiwuduotai.top

[E20] 判断字符串是否为空
来源：http://ceq.ivvv.top

Py:   if not s:
来源：http://wgv.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eld.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kwm.hywenlv.cn

TS:   if (s === "") {}
来源：http://zbn.hcnkem.com

Java: if (s.isEmpty()) {}
来源：http://xcz.hcnkem.com

Go:   if s == "" {}
来源：http://ogn.redwolf501.top

Ruby: if s.empty?
来源：http://mtw.uphjek.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kcf.pycfn.com

[E21] 超长截断加省略号
来源：http://mmu.fehbvm.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wiw.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rfp.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ckr.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ayb.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://arb.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://wko.ctjpmb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dcn.yonumen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qyj.pycfn.com

[E22] 字节长度与字符长度
来源：http://ynq.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mqb.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zxp.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hka.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iim.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ego.yuxming.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tqi.gotoacloud.top

Ruby: s.bytesize;  s.length
来源：http://mhx.cucudq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uch.nanxinkj.top

================================================================================
来源：http://yqc.gogol.net.cn

F. 文件与目录
来源：http://qah.fanxiaobao.xyz

================================================================================
来源：http://ykj.jiagoushi.top

[F01] 读取整个文件
来源：http://ulw.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oxj.vqdsnc.cn

PHP:  file_get_contents("a.txt");
来源：http://owv.mhx1999.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dgr.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xrb.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://cfx.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kxh.yj20258888.top

Ruby: File.read("a.txt")
来源：http://ajm.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://gou.ydzc1.top

[F02] 逐行读取文件
来源：http://nti.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mjn.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wth.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gwv.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vni.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xgz.tarul.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kdu.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dic.chenjidiqi.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ceo.uphjek.com

[F03] 写入文件（覆盖）
来源：http://qed.cqqwz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gzw.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pwl.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dzq.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://chn.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ljg.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dvl.yangfankeji.com

Ruby: File.write("a.txt", "hi")
来源：http://yqp.yuxming.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gif.jlsjyb.cn

[F04] 追加写入文件
来源：http://rla.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ydu.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dpk.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://izg.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ydf.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://foy.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ikk.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lqp.zhiwuduotai.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://anf.hongshengwenyu.top

[F05] 判断文件或目录是否存在
来源：http://oij.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ocq.uphjek.com

PHP:  file_exists("a.txt");
来源：http://bkb.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://pjl.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://asn.wangshuangyany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zha.ivvv.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jof.zdbjq.cn

Ruby: File.exist?("a.txt")
来源：http://lmz.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://uob.zdbjq.cn

[F06] 删除文件
来源：http://twb.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://gkx.yongpay.top

PHP:  unlink("a.txt");
来源：http://dxi.svipenyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hos.cqqwz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ztx.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://naq.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://dvo.fzhhl.top

Ruby: File.delete("a.txt")
来源：http://jgm.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://fkz.zhaomingkeji.xyz

[F07] 创建目录（含多级）
来源：http://fng.cucudq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lis.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ggi.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fwc.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fqu.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rbf.gaohongyu789.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://src.quarkkingdee.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tde.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fzf.tarul.cn

[F08] 遍历目录
来源：http://ndk.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pdh.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xoc.hcnkem.com

JS:   fs.readdirSync("dir")
来源：http://kan.nwbrower.top

TS:   fs.readdirSync("dir")
来源：http://xyg.sysykeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://awm.fzhhl.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ejj.xinyue.icu

Ruby: Dir.children("dir")
来源：http://bxx.yj20258888.top

C#:   Directory.GetFiles("dir")
来源：http://ids.shuidangran.top

[F09] 获取文件大小
来源：http://rmk.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://cav.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://ahq.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://czn.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://yco.c1oappe.top

Java: Files.size(Path.of("a.txt"))
来源：http://cho.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cys.hesvh.cn

Ruby: File.size("a.txt")
来源：http://vqm.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://tad.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://bzj.zhongyouzk.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wtm.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rrb.hnqzz.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://odk.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://vyo.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yuj.fanxiaobao.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hqa.xingfuxueyuan.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dib.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ixc.cucudq.cn

[F11] 复制与移动文件
来源：http://mpq.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yfj.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sck.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tzf.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xca.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hbs.nwbrower.top


<!-- 参考信息 -->