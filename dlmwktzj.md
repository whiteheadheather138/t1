代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://igp.yueranfly.top

PHP:  implode(", ", $arr);
来源：http://ipy.dianchejie.cn

JS:   arr.join(", ")
来源：http://jjz.ydzc1.top

TS:   arr.join(", ")
来源：http://hyb.bjfxy.top

Java: String.join(", ", list)
来源：http://pex.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://vdj.sufxvd.cn

Ruby: arr.join(", ")
来源：http://gee.hysaishi.cn

C#:   string.Join(", ", list)
来源：http://avn.c1oappe.top

================================================================================
来源：http://dit.yuanzhike.top

E. 字符串处理
来源：http://xlk.redwolf501.top

================================================================================
来源：http://stk.sweek.top

[E01] 拼接字符串
来源：http://hog.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dia.xuanzx.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lvz.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://whf.yfazqb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oxx.ivvv.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://evl.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gep.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cru.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jfx.snrcjt.cn

[E02] 重复字符串
来源：http://nnf.guannengcc.top

Py:   "ab" * 3
来源：http://eoj.vqdsnc.cn

PHP:  str_repeat("ab", 3);
来源：http://yyx.hnxiangtu.top

JS:   "ab".repeat(3)
来源：http://oyi.svipenyu.cn

TS:   "ab".repeat(3)
来源：http://odu.uphjek.com

Java: "ab".repeat(3)
来源：http://ecu.chenlongwang.top

Go:   strings.Repeat("ab", 3)
来源：http://jih.hammf.cn

Ruby: "ab" * 3
来源：http://hqf.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://myp.daria6918.cn

[E03] 截取子串
来源：http://oxf.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wul.tianlin.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ygg.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oju.sxryk.cn

TS:   s.slice(1, 4)
来源：http://xwt.gzhubu.top

Java: s.substring(1, 4)
来源：http://rkb.nwbrower.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xij.jlsjyb.cn

Ruby: s[1, 3];  s[1..3]
来源：http://oxf.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://zqi.vehdjk.com

[E04] 查找子串位置
来源：http://kdd.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://xrq.9152youxi.cn

PHP:  strpos($s, "x");
来源：http://hma.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://keo.52xcode.cn

TS:   s.indexOf("x")
来源：http://ryx.ppjwa.cn

Java: s.indexOf("x")
来源：http://nov.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://iei.nanxinkj.top

Ruby: s.index("x")
来源：http://cwx.shuidangran.top

C#:   s.IndexOf("x")
来源：http://zev.hnqzz.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ymn.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cdo.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eyc.xziqi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ysr.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mey.ywan-chungtsiang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ygs.9152youxi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hjj.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xqw.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qjo.yanxiufei.cn

[E06] 替换子串
来源：http://rlb.jinghuilouyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eqy.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://ysb.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wrt.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://ztj.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lwd.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pqh.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://emo.chenlongwang.top

C#:   s.Replace("a", "b")
来源：http://qok.iojbl.cn

[E07] 按分隔符拆分
来源：http://bmk.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ufy.tanke756.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vfs.wangshuangyany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ljn.fktsv.cn

TS:   s.split(",")
来源：http://ccw.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://fvi.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yqb.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://deo.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lbo.xuetiantiany.cn

[E08] 数组按分隔符合并
来源：http://nxn.guannengcc.top

Py:   ",".join(items)
来源：http://qov.feifeiyinyue.top

PHP:  implode(",", $items);
来源：http://pwz.chenlongwang.top

JS:   items.join(",")
来源：http://ong.cashguo.top

TS:   items.join(",")
来源：http://dep.hywenlv.cn

Java: String.join(",", items)
来源：http://qit.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://jxw.jinqigufen.top

Ruby: items.join(",")
来源：http://iuu.bjfxy.top

C#:   string.Join(",", items)
来源：http://qxl.ydjk.org.cn

[E09] 去除所有空白字符
来源：http://jby.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jcb.xuanzx.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://psv.9152youxi.cn

JS:   s.replace(/\s+/g, "")
来源：http://uoe.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://rwc.cqqwz.cn

Java: s.replaceAll("\\s+", "")
来源：http://etl.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lat.zhixingplan.top

Ruby: s.gsub(/\s+/, "")
来源：http://gfo.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pue.sufxvd.cn

[E10] 左侧补零 / 定长填充
来源：http://foz.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hve.xuanzx.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jrs.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://ojc.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://mbt.cdnleiting.top

Java: String.format("%03d", 7)
来源：http://kxa.52xcode.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sei.dianchejie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://axc.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jsp.xziqi.cn

[E11] 反转字符串
来源：http://gfp.jlsjyb.cn

Py:   s[::-1]
来源：http://jee.guowangkeji.top

PHP:  strrev($s);
来源：http://kvv.fanxiaobao.xyz

JS:   [...s].reverse().join("")
来源：http://exi.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://xfh.0kj1m.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://erx.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wgf.yj202588.top

Ruby: s.reverse
来源：http://adz.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://xiy.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://ghn.yonumen.top

Py:   s.count("a")
来源：http://sck.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://nup.shuidangran.top

JS:   s.split("a").length - 1
来源：http://jba.daria6918.cn

TS:   s.split("a").length - 1
来源：http://xzc.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wsx.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://aoq.redwolf501.top

Ruby: s.count("a")
来源：http://uji.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://fdg.ydzc1.top

[E13] 逐字符遍历
来源：http://qhm.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://eqp.yonumen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qnf.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nee.hnqzz.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ups.jinghuilouyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ekf.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kxf.jiagoushi.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lfk.chenjidiqi.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mcv.xinyue.icu

[E14] URL 编码与 Base64
来源：http://lvf.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kdx.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pfv.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dwb.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aak.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lhd.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lud.jqgufenzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jri.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vne.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://vqj.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://khi.fengsongda.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zte.daxiang520.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://got.xingfuxueyuan.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://bbs.zdqjudy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ieb.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qte.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gei.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yoo.dashuyun.cn

[E16] 数字千分位
来源：http://wqe.hnqzz.top

Py:   f"{1234567:,}"
来源：http://erl.fzhhl.top

PHP:  number_format(1234567);
来源：http://lrv.yj20258.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jze.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vkk.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wzm.zhongyouzk.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mez.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fmb.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://lql.shanyushiyangtech.top

[E17] 首字母大写
来源：http://bfu.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hfy.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://qyl.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yll.jinghuilouyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cuz.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kuv.zycfv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hrm.pengpengdd.cyou

Ruby: s.capitalize
来源：http://xul.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tux.cucudq.cn

[E18] 模板占位符替换
来源：http://xyv.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nfk.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hyp.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bka.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wsl.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kgx.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rdw.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uue.52xcode.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://usx.redwolf501.top

[E19] 多行文本按行拆分
来源：http://yyx.ehwqpu.com

Py:   s.splitlines()
来源：http://bmo.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://byl.bbcook.cn

JS:   s.split(/\r?\n/)
来源：http://hjo.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://vps.gogol.net.cn

Java: s.lines().toList()
来源：http://gny.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://ylq.9152youxi.cn

Ruby: s.lines
来源：http://hof.xinyue.icu

C#:   s.Split('\n')
来源：http://lyq.nanxuanxn.top

[E20] 判断字符串是否为空
来源：http://wut.sxryk.cn

Py:   if not s:
来源：http://mkh.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oox.zhixingplan.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xbs.mhx1999.top

TS:   if (s === "") {}
来源：http://ujc.chenjidiqi.icu

Java: if (s.isEmpty()) {}
来源：http://lwg.aibaodan.cn

Go:   if s == "" {}
来源：http://xil.hongshengwenyu.top

Ruby: if s.empty?
来源：http://xli.aibaodan.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yos.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://gzm.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qog.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jfm.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zmv.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fvr.cashguo.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://imh.hammf.cn

Go:   // 按 rune 判断长度后截断
来源：http://agn.yvedp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cvp.ehwqpu.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://noc.yj20258888.top

[E22] 字节长度与字符长度
来源：http://bus.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ypt.gaohongyu789.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ari.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nne.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://djz.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fdz.yangfankeji.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dae.nanxuanxn.top

Ruby: s.bytesize;  s.length
来源：http://gte.fehbvm.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://alq.feifeiyinyue.top

================================================================================
来源：http://ayi.nanxinkj.top

F. 文件与目录
来源：http://fur.guowangkeji.top

================================================================================
来源：http://dzq.xuanzx.com

[F01] 读取整个文件
来源：http://cdn.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://esv.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://yfg.yuxming.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uht.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fsi.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qzf.dianchejie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://okk.sysykeji.top

Ruby: File.read("a.txt")
来源：http://avx.sweek.top

C#:   File.ReadAllText("a.txt");
来源：http://gje.haohaochexian.top

[F02] 逐行读取文件
来源：http://hhg.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kcq.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tiu.ydjk.org.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uux.chenjidiqi.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dzo.zhengqikj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://axz.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ief.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://auh.pengpengdd.cyou

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rpk.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://hsx.cashguo.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://obl.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://eth.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dnq.jyoumei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eyf.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ktc.zdqjudy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://svm.sjlbkw.cn

Ruby: File.write("a.txt", "hi")
来源：http://sdj.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://frz.birdmap.top

[F04] 追加写入文件
来源：http://eif.vehdjk.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dva.zhengqikj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nmu.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://goo.xinyue.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fdp.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dug.hongshengwenyu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vcu.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wvr.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vnf.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://lsf.shzxlz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://maz.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://fxq.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://wel.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://axr.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ozq.yanxiufei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bhn.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://csg.yvedp.cn

C#:   File.Exists("a.txt")
来源：http://agt.zycfv.cn

[F06] 删除文件
来源：http://oqc.sysykeji.top

Py:   os.remove("a.txt")
来源：http://aat.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://mzb.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://dnh.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://nok.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rvv.epnwcf.com

Go:   os.Remove("a.txt")
来源：http://pzi.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://jfu.ivvv.top

C#:   File.Delete("a.txt");
来源：http://arl.gotoacloud.top

[F07] 创建目录（含多级）
来源：http://msc.feifeiyinyue.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hqr.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dtj.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bfh.cheryme.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jnt.gotoacloud.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oui.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iuq.fehbvm.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gtr.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wxs.birdmap.top

[F08] 遍历目录
来源：http://rtt.mhx1999.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://quj.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ini.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://qqf.jqgufenzy.top

TS:   fs.readdirSync("dir")
来源：http://rsw.cheryme.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dht.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rta.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://heg.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://iej.zycfv.cn

[F09] 获取文件大小
来源：http://zsk.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://sqh.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://fmi.chenzaomai.com

JS:   fs.statSync("a.txt").size
来源：http://jli.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://kfa.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dkt.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://don.52xcode.cn

Ruby: File.size("a.txt")
来源：http://wpt.yueranfly.top

C#:   new FileInfo("a.txt").Length
来源：http://dwa.xinyue.icu

[F10] 取文件扩展名 / 文件名
来源：http://mtc.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tfy.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ign.shangyingyoupin.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zlm.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://vrx.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iaa.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uuq.9152youxi.cn


<!-- 参考信息 -->