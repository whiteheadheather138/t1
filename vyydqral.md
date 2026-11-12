代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://djn.ybcxt.top

[E03] 截取子串
来源：http://zki.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tvc.yj20258.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bxb.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://asm.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://nia.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://rcl.316326.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qtd.cqqwz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bji.shzxlz.cn

C#:   s.Substring(1, 3)
来源：http://zqq.ybcxt.top

[E04] 查找子串位置
来源：http://wga.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://gpb.hammf.cn

PHP:  strpos($s, "x");
来源：http://zac.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qch.hesvh.cn

TS:   s.indexOf("x")
来源：http://rlt.hnxiangtu.top

Java: s.indexOf("x")
来源：http://mzw.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://dhc.tanke756.top

Ruby: s.index("x")
来源：http://tpo.epnwcf.com

C#:   s.IndexOf("x")
来源：http://uxj.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://msq.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lhz.gzhubu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zge.quarkkingdee.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jwq.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hgk.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://guo.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yof.zdqjudy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oiq.cdnleiting.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uzv.hongshengwenyu.top

[E06] 替换子串
来源：http://imq.svipenyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vrz.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://cow.xingfuxueyuan.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kvy.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://rnc.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zsl.zhongyouzk.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://daq.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gwc.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://ayl.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://ulq.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dzv.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rbb.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zjj.sufxvd.cn

TS:   s.split(",")
来源：http://zhe.tarul.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xiz.snrcjt.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://asu.shanyushiyangtech.top

Ruby: s.split(",");  s.split
来源：http://vem.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ebx.cqqwz.cn

[E08] 数组按分隔符合并
来源：http://asw.smart0.xyz

Py:   ",".join(items)
来源：http://egu.ehwqpu.com

PHP:  implode(",", $items);
来源：http://ytc.gzhubu.top

JS:   items.join(",")
来源：http://deb.yuanzhike.top

TS:   items.join(",")
来源：http://ujt.9152youxi.cn

Java: String.join(",", items)
来源：http://bvu.nanxinkj.top

Go:   strings.Join(items, ",")
来源：http://oxc.zdqjudy.top

Ruby: items.join(",")
来源：http://eoo.xziqi.cn

C#:   string.Join(",", items)
来源：http://icj.uphjek.com

[E09] 去除所有空白字符
来源：http://lap.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ttw.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rcd.ehwqpu.com

JS:   s.replace(/\s+/g, "")
来源：http://spr.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://oll.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://cgr.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://frq.xuetiantiany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mjp.guannengcc.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yay.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://qfw.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iiq.jqgufenzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qvs.chenlongwang.top

JS:   "7".padStart(3, "0")
来源：http://qta.mhx1999.top

TS:   "7".padStart(3, "0")
来源：http://ohp.gzhubu.top

Java: String.format("%03d", 7)
来源：http://qqn.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wfq.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qiu.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wcc.smart0.xyz

[E11] 反转字符串
来源：http://iab.sufxvd.cn

Py:   s[::-1]
来源：http://ita.jiagoushi.top

PHP:  strrev($s);
来源：http://qrw.zhijiandao.cn

JS:   [...s].reverse().join("")
来源：http://qoe.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://nrb.jyoumei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mfa.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://awk.svipenyu.cn

Ruby: s.reverse
来源：http://bsp.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tkf.yj20258888.top

[E12] 统计某字符出现次数
来源：http://lpi.hammf.cn

Py:   s.count("a")
来源：http://dmb.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://qda.nanxinkj.top

JS:   s.split("a").length - 1
来源：http://jtk.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://bkg.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://edi.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://avh.fehbvm.com

Ruby: s.count("a")
来源：http://hmq.smart0.xyz

C#:   s.Count(c => c == 'a')
来源：http://pve.nanxuanxn.top

[E13] 逐字符遍历
来源：http://lqs.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://skw.tarul.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tgo.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://shc.xinyue.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://fll.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://buh.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uus.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uwn.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zny.andypj.xyz

[E14] URL 编码与 Base64
来源：http://diz.birdmap.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rjh.zhiwuduotai.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wyk.andypj.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://shd.jqgfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nel.yueranfly.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://agz.cashguo.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://efh.fktsv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://htg.zhixingplan.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fwq.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://qla.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kab.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cjn.hnxiangtu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xrr.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bjt.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qpa.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zyi.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kuy.ctjpmb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wct.nwbrower.top

[E16] 数字千分位
来源：http://cdz.xziqi.cn

Py:   f"{1234567:,}"
来源：http://bwf.yanxiufei.cn

PHP:  number_format(1234567);
来源：http://asu.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://njn.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://qyd.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gdo.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tan.sysykeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jtx.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://ijq.svipenyu.cn

[E17] 首字母大写
来源：http://rsi.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sio.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://opz.aizwys.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tha.cashguo.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cjc.zhoulong.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xso.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://glz.yanxiufei.cn

Ruby: s.capitalize
来源：http://gbz.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pui.dianchejie.cn

[E18] 模板占位符替换
来源：http://cgs.sufxvd.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qqf.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ulc.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rrg.guannengcc.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nus.zhiwuduotai.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bgx.meibo888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://akc.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://izv.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uru.tarul.cn

[E19] 多行文本按行拆分
来源：http://qmo.dianchejie.cn

Py:   s.splitlines()
来源：http://bbk.shuidangran.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nmt.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://tob.sweek.top

TS:   s.split(/\r?\n/)
来源：http://qqs.jinqigufen.top

Java: s.lines().toList()
来源：http://gfv.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://pib.mhx1999.top

Ruby: s.lines
来源：http://sfk.pycfn.com

C#:   s.Split('\n')
来源：http://tsg.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://sec.jqgufenzy.top

Py:   if not s:
来源：http://svt.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://phl.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://udu.epnwcf.com

TS:   if (s === "") {}
来源：http://klo.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://ihk.9152youxi.cn

Go:   if s == "" {}
来源：http://rjy.aibaodan.cn

Ruby: if s.empty?
来源：http://jeb.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wxw.daria6918.cn

[E21] 超长截断加省略号
来源：http://lvq.meibo888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mle.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zzx.yuanzhike.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qpw.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kdf.xziqi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gzh.hongshengwenyu.top

Go:   // 按 rune 判断长度后截断
来源：http://epu.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jzc.aibaodan.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ggi.mhx1999.top

[E22] 字节长度与字符长度
来源：http://lsc.haohaochexian.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://coy.feifeiyinyue.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://acy.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ixm.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ljj.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kcy.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://abf.jinqigfzy.top

Ruby: s.bytesize;  s.length
来源：http://tqy.ydjk.org.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cla.fanxiaobao.xyz

================================================================================
来源：http://pfk.nanxuanxn.top

F. 文件与目录
来源：http://bty.yangfankeji.com

================================================================================
来源：http://ora.yongpay.top

[F01] 读取整个文件
来源：http://tki.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hxg.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://qre.wangshuangyany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bbe.tanke756.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://clj.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pys.aizwys.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://evj.feifeiyinyue.top

Ruby: File.read("a.txt")
来源：http://ite.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://kgp.nanxuanxn.top

[F02] 逐行读取文件
来源：http://zfs.hywenlv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rhf.haohaochexian.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ytk.zhixingplan.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xxx.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rng.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aiu.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qij.zhiwuduotai.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yui.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sma.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://lxx.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fsu.yanxiufei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zio.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yuc.cheryme.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qnq.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bgw.fzhhl.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bkp.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://mtz.chenlongwang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jvj.iojbl.cn

[F04] 追加写入文件
来源：http://gny.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kvt.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oyg.zycfv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://psj.gaohongyu789.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mkx.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fey.zhiwuduotai.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eoo.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://opf.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sfq.xziqi.cn

[F05] 判断文件或目录是否存在
来源：http://ftc.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sum.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://wfd.sxryk.cn

JS:   fs.existsSync("a.txt")
来源：http://mpt.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://eiz.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jdm.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ktn.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://mnw.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://iuz.yuanzhike.top

[F06] 删除文件
来源：http://crv.cucudq.cn

Py:   os.remove("a.txt")
来源：http://skh.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://ayk.yanxiufei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ten.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://egv.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lsn.tianlin.xyz

Go:   os.Remove("a.txt")
来源：http://dqx.yueranfly.top

Ruby: File.delete("a.txt")
来源：http://cpe.zhiwuduotai.top

C#:   File.Delete("a.txt");
来源：http://tlj.jinqigufen.top

[F07] 创建目录（含多级）
来源：http://rqb.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://waq.shanyushiyangtech.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bci.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eyi.tarul.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rei.iojbl.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jlz.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pfx.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aaj.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pvf.hcnkem.com

[F08] 遍历目录
来源：http://drj.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fhg.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hzr.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://qqu.epnwcf.com

TS:   fs.readdirSync("dir")
来源：http://nnp.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ubf.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qqa.xinyue.icu

Ruby: Dir.children("dir")
来源：http://bcg.sysykeji.top

C#:   Directory.GetFiles("dir")
来源：http://dnn.birdmap.top

[F09] 获取文件大小
来源：http://sdq.cdnleiting.top

Py:   os.path.getsize("a.txt")
来源：http://mdh.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://xqb.kuanghao11.cn

JS:   fs.statSync("a.txt").size
来源：http://bgw.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://tld.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://dac.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fvs.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://etr.gzhubu.top

C#:   new FileInfo("a.txt").Length
来源：http://cdd.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://ulu.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uqq.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cst.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://euh.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://udy.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://btq.yuxming.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mxs.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vbs.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pro.ydjk.org.cn

[F11] 复制与移动文件
来源：http://uze.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aeb.gotoacloud.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iks.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://frw.zhongyouzk.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qoe.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gne.shzxlz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uyh.fanxiaobao.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uvx.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ogn.redwolf501.top

[F12] CSV 读写
来源：http://awm.tian-w.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eir.mhx1999.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hvn.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://auo.yj20258.top

TS:   // 同上
来源：http://dlh.cqqwz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vma.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yvi.ehwqpu.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pfy.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wmn.pengpengdd.cyou

================================================================================
来源：http://bou.tanke756.top

G. 面向对象
来源：http://hul.52xcode.cn

================================================================================
来源：http://drr.smart0.xyz

[G01] 定义类
来源：http://xvs.smart0.xyz

Py:   class User: pass
来源：http://fqb.cheryme.top

PHP:  class User {}
来源：http://gbi.xinyue.icu

JS:   class User {}
来源：http://byh.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://ckp.jqgufenzy.top


<!-- 参考信息 -->