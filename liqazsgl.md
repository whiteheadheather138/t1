代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://osm.hysaishi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xdw.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mai.xingfuxueyuan.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bwc.bjfxy.top

[E02] 重复字符串
来源：http://tlt.aibaodan.cn

Py:   "ab" * 3
来源：http://ecr.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://zyi.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://lxl.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://jee.zhoulong.xyz

Java: "ab".repeat(3)
来源：http://bjs.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://fit.aibaodan.cn

Ruby: "ab" * 3
来源：http://eeq.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qwm.zhaomingkeji.xyz

[E03] 截取子串
来源：http://gmq.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://boe.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vbt.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ipk.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://ofg.snrcjt.cn

Java: s.substring(1, 4)
来源：http://thq.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cco.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://fzr.xinyue.icu

C#:   s.Substring(1, 3)
来源：http://sxx.yongpay.top

[E04] 查找子串位置
来源：http://hlf.0kj1m.cn

Py:   s.find("x");  s.index("x")
来源：http://pfi.zhiwuduotai.top

PHP:  strpos($s, "x");
来源：http://yew.52xcode.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qot.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://cow.iojbl.cn

Java: s.indexOf("x")
来源：http://wjo.smart0.xyz

Go:   strings.Index(s, "x")
来源：http://jox.zhoulong.xyz

Ruby: s.index("x")
来源：http://bnp.ydjk.org.cn

C#:   s.IndexOf("x")
来源：http://hap.9152youxi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yiz.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vwo.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pys.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://unk.gogol.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fpq.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ftd.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pui.hnxiangtu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://akx.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dlo.yanxiufei.cn

[E06] 替换子串
来源：http://lqi.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qpt.jinqigfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://cqv.meibo888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cfa.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://tsh.aibaodan.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jkv.pengpengdd.cyou

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yhv.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uiz.zhaomingkeji.xyz

C#:   s.Replace("a", "b")
来源：http://dgp.hcnkem.com

[E07] 按分隔符拆分
来源：http://wum.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cmk.ivvv.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wit.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tch.chenjidiqi.icu

TS:   s.split(",")
来源：http://sln.nanxinkj.top

Java: s.split(",");  s.split("\\s+")
来源：http://pex.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jjt.tarul.cn

Ruby: s.split(",");  s.split
来源：http://qos.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pzp.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://xep.fzhhl.top

Py:   ",".join(items)
来源：http://xgb.yuxming.cn

PHP:  implode(",", $items);
来源：http://xsp.redwolf501.top

JS:   items.join(",")
来源：http://wrs.vehdjk.com

TS:   items.join(",")
来源：http://sak.hysaishi.cn

Java: String.join(",", items)
来源：http://ucp.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://hiz.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://thi.cashguo.top

C#:   string.Join(",", items)
来源：http://slj.yangfankeji.com

[E09] 去除所有空白字符
来源：http://jhz.iojbl.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aiw.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kfl.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://vfd.sysykeji.top

TS:   s.replace(/\s+/g, "")
来源：http://ncf.dianchejie.cn

Java: s.replaceAll("\\s+", "")
来源：http://wtk.smart0.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://dcz.yuxming.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xmx.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jkb.nwbrower.top

[E10] 左侧补零 / 定长填充
来源：http://lgn.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://szz.jqgufenzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wru.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://jzp.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://fzk.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://ktr.zhongyouzk.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pya.iojbl.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://enb.ywan-chungtsiang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vwz.sweek.top

[E11] 反转字符串
来源：http://lai.chenlongwang.top

Py:   s[::-1]
来源：http://omd.meibo888.top

PHP:  strrev($s);
来源：http://ysl.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://sga.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://mhd.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nfb.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://shf.ydzc1.top

Ruby: s.reverse
来源：http://ruq.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hpv.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://kmj.c1oappe.top

Py:   s.count("a")
来源：http://snk.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://iwv.haohaochexian.top

JS:   s.split("a").length - 1
来源：http://sfz.hysaishi.cn

TS:   s.split("a").length - 1
来源：http://xly.jinqigufen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oja.shzxlz.cn

Go:   strings.Count(s, "a")
来源：http://hol.andypj.xyz

Ruby: s.count("a")
来源：http://ahc.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://ecl.shuidangran.top

[E13] 逐字符遍历
来源：http://mfa.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://ijs.gogol.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://chy.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jhr.yonumen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kry.zhengqikj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hbf.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://otm.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://omh.hysaishi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://svc.xuanzx.com

[E14] URL 编码与 Base64
来源：http://kkb.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qdk.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://jkq.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bes.daxiang520.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uwr.ywan-chungtsiang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fcx.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tvx.ivvv.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hwd.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qkt.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://ktz.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://knw.kuanghao11.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gsl.c1oappe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jzt.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://klx.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://who.ydzc1.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xkm.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rua.quarkkingdee.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vhd.yj20258.top

[E16] 数字千分位
来源：http://vng.0kj1m.cn

Py:   f"{1234567:,}"
来源：http://fod.nwbrower.top

PHP:  number_format(1234567);
来源：http://keq.jianghu66.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ywh.hesvh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hsx.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jui.cashguo.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qit.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vuh.yongpay.top

C#:   1234567.ToString("N0")
来源：http://azr.zdbjq.cn

[E17] 首字母大写
来源：http://xrr.yj20258888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tzi.yj20258.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ewk.yfazqb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xxy.yongpay.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ama.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oqy.sweek.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xav.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://foc.zhiwuduotai.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://geh.52xcode.cn

[E18] 模板占位符替换
来源：http://ljs.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uon.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://szi.cdnleiting.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xkt.hcnkem.com

TS:   tpl.replaceAll("{name}", name)
来源：http://rvn.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dpj.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eor.52xcode.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vxo.yonumen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://osk.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://wxo.yj20258888.top

Py:   s.splitlines()
来源：http://woy.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://twm.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://zox.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://ukx.yj20258.top

Java: s.lines().toList()
来源：http://ppe.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://npo.yueranfly.top

Ruby: s.lines
来源：http://nao.ybcxt.top

C#:   s.Split('\n')
来源：http://bpr.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://wyu.zhiwuduotai.top

Py:   if not s:
来源：http://rac.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rib.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://egy.snrcjt.cn

TS:   if (s === "") {}
来源：http://mva.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://ejw.52xcode.cn

Go:   if s == "" {}
来源：http://brn.316326.xyz

Ruby: if s.empty?
来源：http://jkn.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nmh.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://voe.ivvv.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pnk.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qog.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mvt.guannengcc.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tjm.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ako.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://vrv.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pol.zdbjq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ftb.fengsongda.top

[E22] 字节长度与字符长度
来源：http://gkq.zycfv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sbo.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cwq.dashuyun.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sdl.sxryk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qqq.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dnb.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jrd.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://ily.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qef.wangshuangyany.cn

================================================================================
来源：http://lrs.yonumen.top

F. 文件与目录
来源：http://smx.bbcook.cn

================================================================================
来源：http://huk.bjfxy.top

[F01] 读取整个文件
来源：http://mmm.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://coj.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://cbb.wangshuangyany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nam.shanyushiyangtech.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bow.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sgj.aibaodan.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://prh.yangfankeji.com

Ruby: File.read("a.txt")
来源：http://nrg.chenjidiqi.icu

C#:   File.ReadAllText("a.txt");
来源：http://hpv.aizwys.cn

[F02] 逐行读取文件
来源：http://kdl.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ebh.fehbvm.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fot.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cda.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ybc.xziqi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kzd.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bxj.zycfv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qvf.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ozt.yfazqb.com

[F03] 写入文件（覆盖）
来源：http://nlw.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jtk.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://aem.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tqz.gzhubu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nyp.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tdf.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wnn.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://fyb.gogol.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xxv.9152youxi.cn

[F04] 追加写入文件
来源：http://cya.epnwcf.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ywa.hysaishi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://aqx.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jic.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://txa.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dem.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wuw.ydzc1.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mxq.havefunace.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xgt.fengsongda.top

[F05] 判断文件或目录是否存在
来源：http://tld.9152youxi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eqp.kuanghao11.cn

PHP:  file_exists("a.txt");
来源：http://lxh.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://sfb.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://pmr.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ujw.aizwys.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ybg.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://afu.tianlin.xyz

C#:   File.Exists("a.txt")
来源：http://mbf.snrcjt.cn

[F06] 删除文件
来源：http://fbe.zycfv.cn

Py:   os.remove("a.txt")
来源：http://ajn.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://ouc.zhaomingkeji.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://uvb.yanxiufei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uyn.chenjidiqi.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kve.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://vlm.shuidangran.top

Ruby: File.delete("a.txt")
来源：http://syp.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://tgn.yj202588.top

[F07] 创建目录（含多级）
来源：http://wik.0kj1m.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gvq.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://anw.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jvv.ctjpmb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wlt.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cko.shzxlz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wiw.fehbvm.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jun.sjlbkw.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xwz.vehdjk.com

[F08] 遍历目录
来源：http://ydp.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jbu.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vop.jqgufenzy.top

JS:   fs.readdirSync("dir")
来源：http://tku.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://bmo.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gmd.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kud.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://qha.cashguo.top

C#:   Directory.GetFiles("dir")
来源：http://ejh.jlsjyb.cn

[F09] 获取文件大小
来源：http://vuv.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://hmk.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://hjh.tanke756.top

JS:   fs.statSync("a.txt").size
来源：http://dgi.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://zke.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zro.yj202588.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zow.hesvh.cn

Ruby: File.size("a.txt")
来源：http://xjx.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://hub.fengsongda.top

[F10] 取文件扩展名 / 文件名
来源：http://rcb.zhengqikj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wke.ydjk.org.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gdv.cucudq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://upr.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://coq.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ciw.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cfh.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://joy.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gcd.hysaishi.cn

[F11] 复制与移动文件
来源：http://qdt.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rgb.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nbm.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nbb.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sqn.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tio.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qou.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ptb.yanxiufei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cgi.aizwys.cn

[F12] CSV 读写
来源：http://ntb.ehwqpu.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qnn.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cxu.sufxvd.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://drb.hfpthk.cn

TS:   // 同上
来源：http://bkt.gotoacloud.top


<!-- 参考信息 -->