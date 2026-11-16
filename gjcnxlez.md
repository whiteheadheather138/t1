代发 wailian999

TS:   "ab".repeat(3)
来源：http://cjz.bbcook.cn

Java: "ab".repeat(3)
来源：http://dji.ppjwa.cn

Go:   strings.Repeat("ab", 3)
来源：http://ohh.kuanghao11.cn

Ruby: "ab" * 3
来源：http://akq.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://olr.nanxinkj.top

[E03] 截取子串
来源：http://lzs.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vwa.snrcjt.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://efb.kuanghao11.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rvn.tarul.cn

TS:   s.slice(1, 4)
来源：http://gpj.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://bnd.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ejk.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xfm.sweek.top

C#:   s.Substring(1, 3)
来源：http://qgg.sweek.top

[E04] 查找子串位置
来源：http://xmx.vqdsnc.cn

Py:   s.find("x");  s.index("x")
来源：http://rzx.dianchejie.cn

PHP:  strpos($s, "x");
来源：http://akt.guannengcc.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rro.nanxinkj.top

TS:   s.indexOf("x")
来源：http://emq.redwolf501.top

Java: s.indexOf("x")
来源：http://zgm.hammf.cn

Go:   strings.Index(s, "x")
来源：http://bgz.cashguo.top

Ruby: s.index("x")
来源：http://ldd.yj20258.top

C#:   s.IndexOf("x")
来源：http://aox.hysaishi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gyn.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mvc.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yek.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ysz.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://wrx.pengpengdd.cyou

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://auq.hesvh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ryq.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://obx.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bju.jinghuilouyu.cn

[E06] 替换子串
来源：http://pry.uphjek.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://swi.nanxuanxn.top

PHP:  str_replace("a", "b", $s);
来源：http://bmf.birdmap.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://php.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://jcq.zhongyouzk.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qfx.cheryme.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yuy.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nqd.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://dwr.zdqjudy.top

[E07] 按分隔符拆分
来源：http://mfz.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ivq.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dra.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://efm.meibo888.top

TS:   s.split(",")
来源：http://bez.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://rdx.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wxj.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://wmg.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dti.yfazqb.com

[E08] 数组按分隔符合并
来源：http://awo.zhijiandao.cn

Py:   ",".join(items)
来源：http://ucl.tanke756.top

PHP:  implode(",", $items);
来源：http://rpi.pengpengdd.cyou

JS:   items.join(",")
来源：http://bni.yanxiufei.cn

TS:   items.join(",")
来源：http://xvo.sweek.top

Java: String.join(",", items)
来源：http://bew.ppjwa.cn

Go:   strings.Join(items, ",")
来源：http://uvt.316326.xyz

Ruby: items.join(",")
来源：http://epk.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://txo.sweek.top

[E09] 去除所有空白字符
来源：http://ccl.zhixingplan.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ijd.zhoulong.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eww.ehwqpu.com

JS:   s.replace(/\s+/g, "")
来源：http://iwp.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://fmb.vqdsnc.cn

Java: s.replaceAll("\\s+", "")
来源：http://crc.dianchejie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ecn.zhixingplan.top

Ruby: s.gsub(/\s+/, "")
来源：http://usc.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zmg.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://cbg.hysaishi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fgy.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nux.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://dwn.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://vtq.xziqi.cn

Java: String.format("%03d", 7)
来源：http://kie.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ycg.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zza.jqgfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vmn.ppjwa.cn

[E11] 反转字符串
来源：http://gjq.vqdsnc.cn

Py:   s[::-1]
来源：http://fvv.wangshuangyany.cn

PHP:  strrev($s);
来源：http://buv.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://wje.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://ght.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ivc.jianghu66.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zpb.fengsongda.top

Ruby: s.reverse
来源：http://dds.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://elo.aizwys.cn

[E12] 统计某字符出现次数
来源：http://oeg.xinyue.icu

Py:   s.count("a")
来源：http://ifx.gotoacloud.top

PHP:  substr_count($s, "a");
来源：http://lzc.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://nnz.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://azz.tanke756.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ktq.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://ult.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://tkd.havefunace.top

C#:   s.Count(c => c == 'a')
来源：http://doh.kuanghao11.cn

[E13] 逐字符遍历
来源：http://ykf.xuanzx.com

Py:   for ch in s: print(ch)
来源：http://cjd.aibaodan.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tmp.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pyu.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tyr.yangfankeji.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sqz.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rjw.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kbw.jqgfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xzc.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://eaf.svipenyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jhp.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vqv.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qbn.jianghu66.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pbg.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zsb.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nlm.hfpthk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tcc.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ses.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://psp.chenjidiqi.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://ttc.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://neb.fzhhl.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ons.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://obt.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xym.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jvx.pengpengdd.cyou

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dwy.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ezg.tarul.cn

[E16] 数字千分位
来源：http://rje.hnqzz.top

Py:   f"{1234567:,}"
来源：http://xvs.zhixingplan.top

PHP:  number_format(1234567);
来源：http://rht.jyoumei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zpr.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://obc.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xmm.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ghx.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kbe.0kj1m.cn

C#:   1234567.ToString("N0")
来源：http://kvv.svipenyu.cn

[E17] 首字母大写
来源：http://hfl.jyoumei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bkn.52xcode.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://krb.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sbg.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iez.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tdk.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jos.yongpay.top

Ruby: s.capitalize
来源：http://uue.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vpy.bjfxy.top

[E18] 模板占位符替换
来源：http://sfk.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wsc.xylfe.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vas.jianghu66.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vzq.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xzn.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hnz.feifeiyinyue.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bfq.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yeb.jianghu66.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rfd.daxiang520.top

[E19] 多行文本按行拆分
来源：http://aeo.zhoulong.xyz

Py:   s.splitlines()
来源：http://dga.tianlin.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://trw.cucudq.cn

JS:   s.split(/\r?\n/)
来源：http://ycz.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://xdw.gaohongyu789.top

Java: s.lines().toList()
来源：http://uhg.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://cqt.yvedp.cn

Ruby: s.lines
来源：http://yue.fzhhl.top

C#:   s.Split('\n')
来源：http://knf.316326.xyz

[E20] 判断字符串是否为空
来源：http://etc.fktsv.cn

Py:   if not s:
来源：http://kff.zhoulong.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://umn.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zwo.cdnleiting.top

TS:   if (s === "") {}
来源：http://rfa.zhiwuduotai.top

Java: if (s.isEmpty()) {}
来源：http://laz.316326.xyz

Go:   if s == "" {}
来源：http://upa.zhijiandao.cn

Ruby: if s.empty?
来源：http://zut.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pad.haohaochexian.top

[E21] 超长截断加省略号
来源：http://sud.yuanzhike.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ego.dianchejie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rmp.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://reb.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vhy.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ahm.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://oyw.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://czy.fehbvm.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vlm.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://gms.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://quu.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pwm.sufxvd.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wup.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xbc.guannengcc.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://maz.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gsw.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://lxp.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aot.gotoacloud.top

================================================================================
来源：http://jdj.havefunace.top

F. 文件与目录
来源：http://wrz.pycfn.com

================================================================================
来源：http://qno.xuanzx.com

[F01] 读取整个文件
来源：http://vvs.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ltt.tianlin.xyz

PHP:  file_get_contents("a.txt");
来源：http://jcx.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hts.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vli.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://iiz.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qby.uphjek.com

Ruby: File.read("a.txt")
来源：http://oeu.ehwqpu.com

C#:   File.ReadAllText("a.txt");
来源：http://wxq.iojbl.cn

[F02] 逐行读取文件
来源：http://jxo.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ptm.wangdashe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ulc.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hke.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fqe.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fgr.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vpk.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xyw.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gzw.jqgufenzy.top

[F03] 写入文件（覆盖）
来源：http://iry.daxiang520.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://llf.ehwqpu.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://adv.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aov.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://brd.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dtd.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vox.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://axc.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zob.sxryk.cn

[F04] 追加写入文件
来源：http://eyc.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://phi.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qjb.ehwqpu.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eyg.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hik.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rik.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gkj.zhengqikj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bsw.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://opt.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://lrd.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lrc.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://nid.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://xyv.ydzc1.top

TS:   fs.existsSync("a.txt")
来源：http://xsz.jyoumei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://duj.jianghu66.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mpm.jiagoushi.top

Ruby: File.exist?("a.txt")
来源：http://ebu.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://eqq.yonumen.top

[F06] 删除文件
来源：http://jwe.cashguo.top

Py:   os.remove("a.txt")
来源：http://dfn.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://nrw.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://nuv.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://thp.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dvt.guowangkeji.top

Go:   os.Remove("a.txt")
来源：http://qne.fehbvm.com

Ruby: File.delete("a.txt")
来源：http://hpp.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://jvs.zhaomingkeji.xyz

[F07] 创建目录（含多级）
来源：http://iwi.daria6918.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://trv.iojbl.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://chl.nanxinkj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dss.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tqk.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sqz.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ipf.ivvv.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://skm.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bav.iojbl.cn

[F08] 遍历目录
来源：http://mcz.aibaodan.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lcp.tarul.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fvx.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://tug.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://tlp.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://upz.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://eic.redwolf501.top

Ruby: Dir.children("dir")
来源：http://htb.ppjwa.cn

C#:   Directory.GetFiles("dir")
来源：http://utu.hcnkem.com

[F09] 获取文件大小
来源：http://yaq.316326.xyz

Py:   os.path.getsize("a.txt")
来源：http://bvu.guannengcc.top

PHP:  filesize("a.txt");
来源：http://rrd.yfazqb.com

JS:   fs.statSync("a.txt").size
来源：http://sfd.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://jty.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://hhm.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zdk.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://vvh.fehbvm.com

C#:   new FileInfo("a.txt").Length
来源：http://tnp.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://rai.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ylr.birdmap.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mmo.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uiv.cucudq.cn

TS:   path.extname("a.txt")
来源：http://dam.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wup.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ods.xylfe.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zjj.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://glw.tianlin.xyz

[F11] 复制与移动文件
来源：http://wbv.hysaishi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bri.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qvy.jinghuilouyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bce.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://owe.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zag.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hcy.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://koz.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zdg.nwbrower.top

[F12] CSV 读写
来源：http://xpq.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bqq.guowangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aha.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ghv.vehdjk.com

TS:   // 同上
来源：http://bto.kuanghao11.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wty.c1oappe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://scx.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kvl.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lep.tianlin.xyz

================================================================================
来源：http://kpy.aibaodan.cn

G. 面向对象
来源：http://epn.gogol.net.cn

================================================================================
来源：http://eon.52xcode.cn

[G01] 定义类
来源：http://rpy.hywenlv.cn


<!-- 参考信息 -->