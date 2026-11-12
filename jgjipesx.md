代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zpw.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://elq.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://omy.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nrj.jinqigfzy.top

[E02] 重复字符串
来源：http://yew.mhx1999.top

Py:   "ab" * 3
来源：http://sfp.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://ead.yanxiufei.cn

JS:   "ab".repeat(3)
来源：http://fsr.wangdashe.top

TS:   "ab".repeat(3)
来源：http://lzl.havefunace.top

Java: "ab".repeat(3)
来源：http://fqy.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://nyn.shzxlz.cn

Ruby: "ab" * 3
来源：http://bgk.wangshuangyany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pfc.ydzc1.top

[E03] 截取子串
来源：http://jjx.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hlo.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wjd.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oen.fengsongda.top

TS:   s.slice(1, 4)
来源：http://ixd.gogol.net.cn

Java: s.substring(1, 4)
来源：http://bhw.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lun.redwolf501.top

Ruby: s[1, 3];  s[1..3]
来源：http://nzx.xylfe.cn

C#:   s.Substring(1, 3)
来源：http://fjj.zycfv.cn

[E04] 查找子串位置
来源：http://ymz.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://ojy.xingfuxueyuan.xyz

PHP:  strpos($s, "x");
来源：http://idv.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bcb.yueranfly.top

TS:   s.indexOf("x")
来源：http://kul.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://lpx.yj20258888.top

Go:   strings.Index(s, "x")
来源：http://qoo.zhijiandao.cn

Ruby: s.index("x")
来源：http://ghs.jqgfzy.top

C#:   s.IndexOf("x")
来源：http://nqs.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vim.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bup.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vvj.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jtb.shanyushiyangtech.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jla.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fku.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kgk.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ndc.fanxiaobao.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wpl.0kj1m.cn

[E06] 替换子串
来源：http://sqq.zhixingplan.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://agw.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://bjo.meibo888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xac.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://acv.yuxming.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gbd.jiagoushi.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jbk.sweek.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xgp.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://wlv.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://umf.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dne.zdqjudy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nat.zdqjudy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xrf.cucudq.cn

TS:   s.split(",")
来源：http://btq.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bkr.c1oappe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pzt.birdmap.top

Ruby: s.split(",");  s.split
来源：http://hve.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pqx.sweek.top

[E08] 数组按分隔符合并
来源：http://lur.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://wmt.jiagoushi.top

PHP:  implode(",", $items);
来源：http://dni.kuanghao11.cn

JS:   items.join(",")
来源：http://ncd.yj20258888.top

TS:   items.join(",")
来源：http://fyu.xuetiantiany.cn

Java: String.join(",", items)
来源：http://ycv.bjfxy.top

Go:   strings.Join(items, ",")
来源：http://eot.chenzaomai.com

Ruby: items.join(",")
来源：http://mix.tian-w.cn

C#:   string.Join(",", items)
来源：http://xwy.yuanzhike.top

[E09] 去除所有空白字符
来源：http://iqi.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bqt.hywenlv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zgf.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://wdy.jqgufenzy.top

TS:   s.replace(/\s+/g, "")
来源：http://rla.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://dnn.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dlx.tianlin.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://vfq.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ybu.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://dbt.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zil.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gad.nanxinkj.top

JS:   "7".padStart(3, "0")
来源：http://dox.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://dnd.dashuyun.cn

Java: String.format("%03d", 7)
来源：http://nex.jinqigfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qpo.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wql.snrcjt.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ejl.cashguo.top

[E11] 反转字符串
来源：http://lds.xuanzx.com

Py:   s[::-1]
来源：http://cpq.zhiwuduotai.top

PHP:  strrev($s);
来源：http://qrd.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://vpw.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://lqw.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qiw.chenzaomai.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://vwl.yanxiufei.cn

Ruby: s.reverse
来源：http://xnj.iojbl.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nej.52xcode.cn

[E12] 统计某字符出现次数
来源：http://tbm.haohaochexian.top

Py:   s.count("a")
来源：http://vxk.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://chd.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://ykf.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://qkf.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://osm.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://lgw.xinyue.icu

Ruby: s.count("a")
来源：http://lay.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://svx.zhiwuduotai.top

[E13] 逐字符遍历
来源：http://sjy.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://wpx.yonumen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oyv.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sdj.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://krx.nwbrower.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iwo.haohaochexian.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mff.sxryk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rkc.smart0.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://roa.smart0.xyz

[E14] URL 编码与 Base64
来源：http://yfv.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vzr.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ahs.ehwqpu.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kkh.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ooe.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wga.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://urz.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fgr.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tuu.nanxuanxn.top

[E15] HTML 转义 / 反转义
来源：http://yxt.sweek.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zes.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uhn.ehwqpu.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xlb.tanke756.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vhv.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://frw.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rrb.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zjg.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bia.316326.xyz

[E16] 数字千分位
来源：http://jgh.ybcxt.top

Py:   f"{1234567:,}"
来源：http://arx.xinyue.icu

PHP:  number_format(1234567);
来源：http://qmu.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ykg.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cpw.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cbq.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yvs.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ytl.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://btl.yueranfly.top

[E17] 首字母大写
来源：http://stq.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bdi.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qly.sjlbkw.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jes.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zzv.aizwys.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://veh.mhx1999.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iyz.xziqi.cn

Ruby: s.capitalize
来源：http://vyq.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://omr.gaohongyu789.top

[E18] 模板占位符替换
来源：http://kcp.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vme.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ggo.ywan-chungtsiang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dmu.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://aao.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hzx.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tqk.hfpthk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qdg.yj202588.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jld.sweek.top

[E19] 多行文本按行拆分
来源：http://ayi.cucudq.cn

Py:   s.splitlines()
来源：http://qdy.zhoulong.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rea.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://bsi.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://rkv.fktsv.cn

Java: s.lines().toList()
来源：http://vsh.dashuyun.cn

Go:   strings.Split(s, "\n")
来源：http://wyk.tanke756.top

Ruby: s.lines
来源：http://dhc.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://nca.shuidangran.top

[E20] 判断字符串是否为空
来源：http://udv.hywenlv.cn

Py:   if not s:
来源：http://bqf.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://msk.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mzc.zhongyouzk.top

TS:   if (s === "") {}
来源：http://vxw.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://nmh.xuetiantiany.cn

Go:   if s == "" {}
来源：http://uzu.shangyingyoupin.top

Ruby: if s.empty?
来源：http://xwo.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zzd.aibaodan.cn

[E21] 超长截断加省略号
来源：http://tln.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rqr.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://khb.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xfj.zhoulong.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kuz.c1oappe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nzp.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://dml.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pib.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mvk.bjfxy.top

[E22] 字节长度与字符长度
来源：http://wbq.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dmn.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ubz.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lsn.iojbl.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jiz.guannengcc.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hqw.gzhubu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eui.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://ouw.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sls.wangshuangyany.cn

================================================================================
来源：http://vjs.tarul.cn

F. 文件与目录
来源：http://ets.dianchejie.cn

================================================================================
来源：http://dqr.shzxlz.cn

[F01] 读取整个文件
来源：http://fhu.cheryme.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xhl.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://mvy.jlsjyb.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qpw.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pmt.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dcd.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hxl.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://ydt.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://thw.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://ozl.hywenlv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bly.hywenlv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dsz.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://btx.jinqigufen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eal.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jmf.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qwm.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yjq.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cfh.zhoulong.xyz

[F03] 写入文件（覆盖）
来源：http://fcy.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ubl.bbcook.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://drn.shzxlz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xlp.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yqu.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fmn.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://keb.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://gsc.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kmg.hnqzz.top

[F04] 追加写入文件
来源：http://rwo.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xys.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://avw.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yzp.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://els.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nws.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qpp.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ckx.c1oappe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ewl.jianghu66.top

[F05] 判断文件或目录是否存在
来源：http://hac.daxiang520.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lbd.dashuyun.cn

PHP:  file_exists("a.txt");
来源：http://edn.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://gds.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://qfj.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://slw.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://inf.yueranfly.top

Ruby: File.exist?("a.txt")
来源：http://feh.tanke756.top

C#:   File.Exists("a.txt")
来源：http://iza.gotoacloud.top

[F06] 删除文件
来源：http://jxz.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://rhr.redwolf501.top

PHP:  unlink("a.txt");
来源：http://hud.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://squ.svipenyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dsi.hywenlv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tas.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://qnf.chenjidiqi.icu

Ruby: File.delete("a.txt")
来源：http://sdh.tarul.cn

C#:   File.Delete("a.txt");
来源：http://ecm.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://kmg.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://res.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://btq.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mau.epnwcf.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mrn.guowangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uld.jlsjyb.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yij.yvedp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qeg.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://emt.ybcxt.top

[F08] 遍历目录
来源：http://ubj.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ulr.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://krf.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://zrh.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://oif.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tkd.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dxn.zhijiandao.cn

Ruby: Dir.children("dir")
来源：http://ubq.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://ovz.pengpengdd.cyou

[F09] 获取文件大小
来源：http://rfl.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://het.yuxming.cn

PHP:  filesize("a.txt");
来源：http://nnc.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://npd.yj202588.top

TS:   fs.statSync("a.txt").size
来源：http://qib.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fck.pycfn.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ael.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://vzm.xuetiantiany.cn

C#:   new FileInfo("a.txt").Length
来源：http://drj.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://jpi.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nbt.yanxiufei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ukn.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jha.yj20258888.top

TS:   path.extname("a.txt")
来源：http://ssb.snrcjt.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tzt.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qdy.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://shu.sufxvd.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bar.iojbl.cn

[F11] 复制与移动文件
来源：http://ryx.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lxe.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cpz.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fea.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gpu.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hhg.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dqt.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ddq.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xfv.jqgfzy.top

[F12] CSV 读写
来源：http://dcy.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rfk.vqdsnc.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fau.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hbp.jiagoushi.top

TS:   // 同上
来源：http://ygy.yj202588.top


<!-- 参考信息 -->