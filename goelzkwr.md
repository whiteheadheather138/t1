代发 wailian999

Java: String.join(", ", list)
来源：http://xkt.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://wyp.ppjwa.cn

Ruby: arr.join(", ")
来源：http://oag.yonumen.top

C#:   string.Join(", ", list)
来源：http://pti.zhijiandao.cn

================================================================================
来源：http://nhc.ctjpmb.com

E. 字符串处理
来源：http://zow.xylfe.cn

================================================================================
来源：http://rmc.fengsongda.top

[E01] 拼接字符串
来源：http://imk.nanxuanxn.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ayl.pengpengdd.cyou

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rzy.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zyc.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://huh.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rck.shuidangran.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cxj.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xwe.hesvh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ttq.yangfankeji.com

[E02] 重复字符串
来源：http://swq.hnxiangtu.top

Py:   "ab" * 3
来源：http://yuq.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://pzj.fehbvm.com

JS:   "ab".repeat(3)
来源：http://xuv.guowangkeji.top

TS:   "ab".repeat(3)
来源：http://ecm.nanxinkj.top

Java: "ab".repeat(3)
来源：http://tck.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://qys.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://lla.vehdjk.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rhr.fengsongda.top

[E03] 截取子串
来源：http://yxb.nwbrower.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ztx.dashuyun.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jka.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mvr.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://pyr.mhx1999.top

Java: s.substring(1, 4)
来源：http://eed.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fsw.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://aej.mhx1999.top

C#:   s.Substring(1, 3)
来源：http://zcl.zdqjudy.top

[E04] 查找子串位置
来源：http://rck.pycfn.com

Py:   s.find("x");  s.index("x")
来源：http://edb.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://qfz.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fsy.hywenlv.cn

TS:   s.indexOf("x")
来源：http://stx.ehwqpu.com

Java: s.indexOf("x")
来源：http://dmh.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://rci.hammf.cn

Ruby: s.index("x")
来源：http://osy.hcnkem.com

C#:   s.IndexOf("x")
来源：http://bqd.yfazqb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://mfz.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eos.cashguo.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sob.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fmj.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://oho.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tgp.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uqg.wangshuangyany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hux.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zpy.tarul.cn

[E06] 替换子串
来源：http://bif.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://khx.yvedp.cn

PHP:  str_replace("a", "b", $s);
来源：http://rmu.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ozp.yj202588.top

TS:   s.replaceAll("a", "b")
来源：http://njr.dashuyun.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bmu.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nvg.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iwe.yj202588.top

C#:   s.Replace("a", "b")
来源：http://acg.hesvh.cn

[E07] 按分隔符拆分
来源：http://pxp.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kkq.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hux.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://plu.zycfv.cn

TS:   s.split(",")
来源：http://yqw.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zjm.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://srw.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://bpt.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hxy.xinyue.icu

[E08] 数组按分隔符合并
来源：http://mhk.fehbvm.com

Py:   ",".join(items)
来源：http://jtt.svipenyu.cn

PHP:  implode(",", $items);
来源：http://ygi.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://suq.sxryk.cn

TS:   items.join(",")
来源：http://ewq.sysykeji.top

Java: String.join(",", items)
来源：http://hnc.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://dtf.hysaishi.cn

Ruby: items.join(",")
来源：http://ywg.hnqzz.top

C#:   string.Join(",", items)
来源：http://anb.snrcjt.cn

[E09] 去除所有空白字符
来源：http://wvf.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oce.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zhs.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://upk.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://cdp.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://uxm.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lrz.zhengqikj.top

Ruby: s.gsub(/\s+/, "")
来源：http://nvl.shangyingyoupin.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wlq.fktsv.cn

[E10] 左侧补零 / 定长填充
来源：http://slr.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dcd.aizwys.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uub.nanxuanxn.top

JS:   "7".padStart(3, "0")
来源：http://byl.chenjidiqi.icu

TS:   "7".padStart(3, "0")
来源：http://hwm.xuanzx.com

Java: String.format("%03d", 7)
来源：http://adh.9152youxi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xtk.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vne.c1oappe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://laz.hongshengwenyu.top

[E11] 反转字符串
来源：http://smh.xuanzx.com

Py:   s[::-1]
来源：http://jkz.quarkkingdee.top

PHP:  strrev($s);
来源：http://bdb.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://apa.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://ekt.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://shw.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ybg.cqqwz.cn

Ruby: s.reverse
来源：http://mfm.hysaishi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kng.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://kae.yuanzhike.top

Py:   s.count("a")
来源：http://xlj.quarkkingdee.top

PHP:  substr_count($s, "a");
来源：http://jdh.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://flf.gaohongyu789.top

TS:   s.split("a").length - 1
来源：http://czq.nanxuanxn.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kgz.yongpay.top

Go:   strings.Count(s, "a")
来源：http://nef.redwolf501.top

Ruby: s.count("a")
来源：http://cio.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://xvp.hammf.cn

[E13] 逐字符遍历
来源：http://xwv.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://exh.jqgufenzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://puk.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ksg.9152youxi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oat.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zjt.jinqigfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://enw.nwbrower.top

Ruby: s.each_char { |ch| puts ch }
来源：http://imq.shuidangran.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ria.yongpay.top

[E14] URL 编码与 Base64
来源：http://fgv.pycfn.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mvw.hammf.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qhx.bjfxy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dlo.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cde.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://okg.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lbt.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vge.jlsjyb.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jpt.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://itv.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mon.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kyy.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hov.yongpay.top

TS:   // 同上，务必做 XSS 过滤
来源：http://trk.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vpl.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kdp.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rdu.yongpay.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://krp.zhixingplan.top

[E16] 数字千分位
来源：http://puu.ehwqpu.com

Py:   f"{1234567:,}"
来源：http://arf.fengsongda.top

PHP:  number_format(1234567);
来源：http://ruz.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hui.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://sam.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://knb.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dii.nanxuanxn.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tig.dianchejie.cn

C#:   1234567.ToString("N0")
来源：http://foy.yongpay.top

[E17] 首字母大写
来源：http://pqr.ehwqpu.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rpd.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://cei.jiagoushi.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bll.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pip.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kbx.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nei.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://zei.316326.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oil.hnxiangtu.top

[E18] 模板占位符替换
来源：http://loh.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ylr.yj20258.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kei.yuanzhike.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mpj.epnwcf.com

TS:   tpl.replaceAll("{name}", name)
来源：http://fbj.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cmv.fanxiaobao.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zyf.zhijiandao.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mcf.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kow.pengpengdd.cyou

[E19] 多行文本按行拆分
来源：http://koc.ywan-chungtsiang.top

Py:   s.splitlines()
来源：http://ydr.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://srh.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://tmt.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://khr.c1oappe.top

Java: s.lines().toList()
来源：http://soj.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://ltr.aizwys.cn

Ruby: s.lines
来源：http://xyn.smart0.xyz

C#:   s.Split('\n')
来源：http://cuh.hfpthk.cn

[E20] 判断字符串是否为空
来源：http://coc.bjfxy.top

Py:   if not s:
来源：http://yft.iojbl.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jeb.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hnx.aibaodan.cn

TS:   if (s === "") {}
来源：http://ypt.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://zlb.xuanzx.com

Go:   if s == "" {}
来源：http://kmk.shzxlz.cn

Ruby: if s.empty?
来源：http://hdb.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pkk.cashguo.top

[E21] 超长截断加省略号
来源：http://frq.shanyushiyangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ceg.xziqi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://trb.vqdsnc.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rln.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mpl.hesvh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lna.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://ykw.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ehb.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xyt.aizwys.cn

[E22] 字节长度与字符长度
来源：http://kqr.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ezo.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ykc.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jyy.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://exh.sweek.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ilp.cdnleiting.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zen.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://ebh.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uqg.snrcjt.cn

================================================================================
来源：http://gpo.pengpengdd.cyou

F. 文件与目录
来源：http://yyl.ywan-chungtsiang.top

================================================================================
来源：http://zso.hywenlv.cn

[F01] 读取整个文件
来源：http://hwj.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hql.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://yum.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fli.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oat.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mmn.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gcp.ydzc1.top

Ruby: File.read("a.txt")
来源：http://rmc.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://ucx.fengsongda.top

[F02] 逐行读取文件
来源：http://ysh.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fvb.nanxinkj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sgj.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hjb.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qij.c1oappe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nxd.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gec.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xjh.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tgq.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://jci.gzhubu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://taq.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ytd.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qnx.birdmap.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gnu.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zkw.uphjek.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ypc.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://ybv.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vyk.dianchejie.cn

[F04] 追加写入文件
来源：http://xnu.yj202588.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ece.ydjk.org.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://srh.shangyingyoupin.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eig.zhengqikj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cyq.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rop.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://akd.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gjd.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mdc.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://doc.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xxx.ehwqpu.com

PHP:  file_exists("a.txt");
来源：http://tft.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://vlx.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://ott.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yew.cheryme.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qll.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://atr.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://mal.hnxiangtu.top

[F06] 删除文件
来源：http://uck.sweek.top

Py:   os.remove("a.txt")
来源：http://tvn.wangdashe.top

PHP:  unlink("a.txt");
来源：http://rmk.jinqigufen.top

JS:   fs.unlinkSync("a.txt")
来源：http://zbf.c1oappe.top

TS:   fs.unlinkSync("a.txt")
来源：http://qxl.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uhh.zdqjudy.top

Go:   os.Remove("a.txt")
来源：http://ikt.zhengqikj.top

Ruby: File.delete("a.txt")
来源：http://gnd.yj202588.top

C#:   File.Delete("a.txt");
来源：http://dkp.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://fnq.316326.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dwl.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cwe.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fdb.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://njz.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mcs.cdnleiting.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cvm.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gxd.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jtv.hongshengwenyu.top

[F08] 遍历目录
来源：http://jnt.yj20258888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rmy.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pfb.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://guh.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://zpg.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vex.hnxiangtu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ldv.quarkkingdee.top

Ruby: Dir.children("dir")
来源：http://nfq.fehbvm.com

C#:   Directory.GetFiles("dir")
来源：http://iyi.yfazqb.com

[F09] 获取文件大小
来源：http://edv.jiagoushi.top

Py:   os.path.getsize("a.txt")
来源：http://lhj.0kj1m.cn

PHP:  filesize("a.txt");
来源：http://nqj.tanke756.top

JS:   fs.statSync("a.txt").size
来源：http://gju.xingfuxueyuan.xyz

TS:   fs.statSync("a.txt").size
来源：http://aur.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://non.fzhhl.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nfq.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://ien.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://cxz.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://aih.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rgo.xziqi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sho.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rap.zhengqikj.top

TS:   path.extname("a.txt")
来源：http://uay.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kkm.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://trx.hesvh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sgq.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cad.kuanghao11.cn

[F11] 复制与移动文件
来源：http://qhc.pengpengdd.cyou

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cdn.haohaochexian.top


<!-- 参考信息 -->