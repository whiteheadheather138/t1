代发 wailian999

[E02] 重复字符串
来源：http://gxi.quarkkingdee.top

Py:   "ab" * 3
来源：http://jkn.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://lti.yj202588.top

JS:   "ab".repeat(3)
来源：http://ypa.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://fql.aizwys.cn

Java: "ab".repeat(3)
来源：http://ivr.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://ihd.zhijiandao.cn

Ruby: "ab" * 3
来源：http://ren.gzhubu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ucx.shangyingyoupin.top

[E03] 截取子串
来源：http://zam.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sbz.tanke756.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oep.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qqw.pycfn.com

TS:   s.slice(1, 4)
来源：http://ijh.xuanzx.com

Java: s.substring(1, 4)
来源：http://sto.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bez.cucudq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ira.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://loa.sxryk.cn

[E04] 查找子串位置
来源：http://cbz.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://cst.hnqzz.top

PHP:  strpos($s, "x");
来源：http://aug.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://amh.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://dsd.vehdjk.com

Java: s.indexOf("x")
来源：http://fkc.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://sev.uphjek.com

Ruby: s.index("x")
来源：http://dby.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://dfd.chenlongwang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gvz.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zot.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wtb.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ajd.snrcjt.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xkt.ywan-chungtsiang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fgy.52xcode.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://arq.sjlbkw.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lcu.meibo888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tyl.xylfe.cn

[E06] 替换子串
来源：http://bxi.chenlongwang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hox.redwolf501.top

PHP:  str_replace("a", "b", $s);
来源：http://lth.cdnleiting.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xyg.meibo888.top

TS:   s.replaceAll("a", "b")
来源：http://rop.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qzd.hfpthk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bld.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://epv.snrcjt.cn

C#:   s.Replace("a", "b")
来源：http://emf.shzxlz.cn

[E07] 按分隔符拆分
来源：http://sdm.aibaodan.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nsf.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rur.shangyingyoupin.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gqt.jinghuilouyu.cn

TS:   s.split(",")
来源：http://ghs.ydjk.org.cn

Java: s.split(",");  s.split("\\s+")
来源：http://klw.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://idm.yj20258.top

Ruby: s.split(",");  s.split
来源：http://mej.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gls.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://hua.pycfn.com

Py:   ",".join(items)
来源：http://lcc.ydzc1.top

PHP:  implode(",", $items);
来源：http://fcj.tianlin.xyz

JS:   items.join(",")
来源：http://vih.shuidangran.top

TS:   items.join(",")
来源：http://hxj.tarul.cn

Java: String.join(",", items)
来源：http://tgq.shzxlz.cn

Go:   strings.Join(items, ",")
来源：http://jfy.cucudq.cn

Ruby: items.join(",")
来源：http://kmc.guannengcc.top

C#:   string.Join(",", items)
来源：http://kik.havefunace.top

[E09] 去除所有空白字符
来源：http://cal.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ywf.nanxinkj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://slx.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://qco.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://hsy.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://fau.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wfx.daxiang520.top

Ruby: s.gsub(/\s+/, "")
来源：http://kal.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://paq.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://ukf.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dia.ivvv.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xis.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://pbl.cheryme.top

TS:   "7".padStart(3, "0")
来源：http://jzr.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://dcz.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rje.aibaodan.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zzp.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bdp.sjlbkw.cn

[E11] 反转字符串
来源：http://nlt.tian-w.cn

Py:   s[::-1]
来源：http://agv.0kj1m.cn

PHP:  strrev($s);
来源：http://ybd.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://tnl.sxryk.cn

TS:   [...s].reverse().join("")
来源：http://yoh.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uhg.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://emu.gzhubu.top

Ruby: s.reverse
来源：http://cvq.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://rmo.uphjek.com

[E12] 统计某字符出现次数
来源：http://cgj.hesvh.cn

Py:   s.count("a")
来源：http://obw.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://unh.xinyue.icu

JS:   s.split("a").length - 1
来源：http://djk.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://gtb.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wiz.ywan-chungtsiang.top

Go:   strings.Count(s, "a")
来源：http://dor.pengpengdd.cyou

Ruby: s.count("a")
来源：http://xzw.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://nyr.cdnleiting.top

[E13] 逐字符遍历
来源：http://cts.yanxiufei.cn

Py:   for ch in s: print(ch)
来源：http://ryp.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ovr.haohaochexian.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pep.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://xbx.yanxiufei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://drm.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://irg.ehwqpu.com

Ruby: s.each_char { |ch| puts ch }
来源：http://cil.fktsv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sbv.yanxiufei.cn

[E14] URL 编码与 Base64
来源：http://dob.feifeiyinyue.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xqw.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://son.daxiang520.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://adp.shuidangran.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vjo.fktsv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jtb.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://soq.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hrn.jqgufenzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cqg.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://tzp.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://plk.fengsongda.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eqb.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nlx.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rja.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tid.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yin.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rem.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://whg.xylfe.cn

[E16] 数字千分位
来源：http://gvp.fzhhl.top

Py:   f"{1234567:,}"
来源：http://qsy.9152youxi.cn

PHP:  number_format(1234567);
来源：http://fkt.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hjz.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gpp.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aji.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qpw.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qie.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://mau.zhengqikj.top

[E17] 首字母大写
来源：http://nqy.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qey.sxryk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ihy.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kqi.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://azo.yj20258.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nxp.ywan-chungtsiang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dnt.kuanghao11.cn

Ruby: s.capitalize
来源：http://nfm.jlsjyb.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qwb.shanyushiyangtech.top

[E18] 模板占位符替换
来源：http://oeo.pycfn.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rof.kuanghao11.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ymf.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kvn.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xju.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qhb.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://own.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nma.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zhj.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://hkw.yuanzhike.top

Py:   s.splitlines()
来源：http://goj.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aeo.9152youxi.cn

JS:   s.split(/\r?\n/)
来源：http://mma.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://nqu.meibo888.top

Java: s.lines().toList()
来源：http://xzi.nanxuanxn.top

Go:   strings.Split(s, "\n")
来源：http://qpc.gogol.net.cn

Ruby: s.lines
来源：http://xob.yvedp.cn

C#:   s.Split('\n')
来源：http://tlg.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://lsl.quarkkingdee.top

Py:   if not s:
来源：http://brh.zhiwuduotai.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ehi.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jhq.ehwqpu.com

TS:   if (s === "") {}
来源：http://cxs.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://zkt.redwolf501.top

Go:   if s == "" {}
来源：http://imq.gotoacloud.top

Ruby: if s.empty?
来源：http://tis.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cai.vehdjk.com

[E21] 超长截断加省略号
来源：http://fth.hongshengwenyu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tie.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://trn.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gxd.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xvu.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kmi.xinyue.icu

Go:   // 按 rune 判断长度后截断
来源：http://syw.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vvu.jyoumei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ftp.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://omj.redwolf501.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tvy.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hsv.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://umu.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bgl.sxryk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hrl.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hwc.zhoulong.xyz

Ruby: s.bytesize;  s.length
来源：http://pax.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://meb.zycfv.cn

================================================================================
来源：http://zno.jlsjyb.cn

F. 文件与目录
来源：http://str.birdmap.top

================================================================================
来源：http://tcp.tanke756.top

[F01] 读取整个文件
来源：http://xwg.meibo888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://esz.sysykeji.top

PHP:  file_get_contents("a.txt");
来源：http://byx.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xtp.hammf.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pbr.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://qdo.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rzz.vqdsnc.cn

Ruby: File.read("a.txt")
来源：http://jup.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://mea.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://qqv.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nto.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://opc.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jxb.sjlbkw.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lrv.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pum.tarul.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bmu.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ujv.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ddc.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://jvb.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tbt.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://eww.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yuv.cqqwz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qsv.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blm.bjfxy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fda.shzxlz.cn

Ruby: File.write("a.txt", "hi")
来源：http://yke.hammf.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ujo.mhx1999.top

[F04] 追加写入文件
来源：http://xqp.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yxr.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tfz.shuidangran.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ayq.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kdo.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gqu.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ygf.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uco.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ccl.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://uid.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rmz.zdbjq.cn

PHP:  file_exists("a.txt");
来源：http://tgd.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://tbw.zdqjudy.top

TS:   fs.existsSync("a.txt")
来源：http://ytr.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://how.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jbl.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://tqd.hywenlv.cn

C#:   File.Exists("a.txt")
来源：http://pqg.shanyushiyangkeji.top

[F06] 删除文件
来源：http://igc.yj20258888.top

Py:   os.remove("a.txt")
来源：http://kql.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://lfw.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hqe.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pxq.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://not.cashguo.top

Go:   os.Remove("a.txt")
来源：http://lkc.guannengcc.top

Ruby: File.delete("a.txt")
来源：http://xmy.birdmap.top

C#:   File.Delete("a.txt");
来源：http://pfy.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://czq.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xyk.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cdr.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://paq.nanxinkj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hob.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jrb.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xoz.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yzi.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vjy.ivvv.top

[F08] 遍历目录
来源：http://anu.yanxiufei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dya.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tid.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://cnb.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://gwc.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://npc.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oic.jinyuanbaomall.cn

Ruby: Dir.children("dir")
来源：http://aid.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://wby.uphjek.com

[F09] 获取文件大小
来源：http://yly.snrcjt.cn

Py:   os.path.getsize("a.txt")
来源：http://fna.smart0.xyz

PHP:  filesize("a.txt");
来源：http://tzw.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://igh.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://uav.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gjn.0kj1m.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://usa.sxryk.cn

Ruby: File.size("a.txt")
来源：http://tzc.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://juv.kuanghao11.cn

[F10] 取文件扩展名 / 文件名
来源：http://ujd.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lgx.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eai.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rvx.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://iqn.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fqe.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fmq.fehbvm.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fix.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ekv.yuanzhike.top

[F11] 复制与移动文件
来源：http://pkd.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qzr.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://amk.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xfq.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yhm.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hvb.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://okr.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://plo.bbcook.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ubd.birdmap.top

[F12] CSV 读写
来源：http://kua.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uku.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kws.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iio.ppjwa.cn

TS:   // 同上
来源：http://hbh.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://muq.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jeg.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cah.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://rou.vqdsnc.cn


<!-- 参考信息 -->