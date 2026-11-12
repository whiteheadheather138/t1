代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jjz.xuetiantiany.cn

[E03] 截取子串
来源：http://ojs.yj202588.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cwo.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xgq.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ahk.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://nyb.hesvh.cn

Java: s.substring(1, 4)
来源：http://tqw.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gqf.shanyushiyangtech.top

Ruby: s[1, 3];  s[1..3]
来源：http://dnz.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://zwn.guowangkeji.top

[E04] 查找子串位置
来源：http://grm.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://bkn.bjfxy.top

PHP:  strpos($s, "x");
来源：http://rqs.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vja.tarul.cn

TS:   s.indexOf("x")
来源：http://rtx.xylfe.cn

Java: s.indexOf("x")
来源：http://ndr.jinyuanbaomall.cn

Go:   strings.Index(s, "x")
来源：http://kuf.sysykeji.top

Ruby: s.index("x")
来源：http://vrt.iojbl.cn

C#:   s.IndexOf("x")
来源：http://jaa.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nvy.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ufw.ydzc1.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://itp.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vlv.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://avy.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lin.52xcode.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ame.snrcjt.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bzo.meibo888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zrm.gaohongyu789.top

[E06] 替换子串
来源：http://wli.svipenyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uyj.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://vjo.chenzaomai.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yxl.jqgufenzy.top

TS:   s.replaceAll("a", "b")
来源：http://oxy.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mta.fzhhl.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fpv.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://btj.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://lic.bbcook.cn

[E07] 按分隔符拆分
来源：http://dgk.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wvb.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uzy.snrcjt.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dgi.birdmap.top

TS:   s.split(",")
来源：http://mbl.wangshuangyany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lum.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vxk.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://ehc.xinyue.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://isg.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://dey.sweek.top

Py:   ",".join(items)
来源：http://jsc.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://sle.tianlin.xyz

JS:   items.join(",")
来源：http://sug.shzxlz.cn

TS:   items.join(",")
来源：http://ibx.chenzaomai.com

Java: String.join(",", items)
来源：http://ieg.fzhhl.top

Go:   strings.Join(items, ",")
来源：http://ova.zhiwuduotai.top

Ruby: items.join(",")
来源：http://jpt.zhengqikj.top

C#:   string.Join(",", items)
来源：http://hxb.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://ubu.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uux.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dpa.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://urw.zhijiandao.cn

TS:   s.replace(/\s+/g, "")
来源：http://lsu.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://rin.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jtv.zhiwuduotai.top

Ruby: s.gsub(/\s+/, "")
来源：http://azf.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kow.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://qls.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oix.daria6918.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ocd.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://wpa.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://onh.nwbrower.top

Java: String.format("%03d", 7)
来源：http://zep.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jvq.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lfl.tanke756.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://twx.cqqwz.cn

[E11] 反转字符串
来源：http://jjc.cheryme.top

Py:   s[::-1]
来源：http://qxr.zycfv.cn

PHP:  strrev($s);
来源：http://irs.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://zhl.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://pog.jinghuilouyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pjl.nwbrower.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pnj.fzhhl.top

Ruby: s.reverse
来源：http://tyh.nanxuanxn.top

C#:   new string(s.Reverse().ToArray())
来源：http://obw.hnxiangtu.top

[E12] 统计某字符出现次数
来源：http://trv.wangshuangyany.cn

Py:   s.count("a")
来源：http://kfp.hesvh.cn

PHP:  substr_count($s, "a");
来源：http://tgq.ybcxt.top

JS:   s.split("a").length - 1
来源：http://pgz.jqgfzy.top

TS:   s.split("a").length - 1
来源：http://tgk.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zlw.hesvh.cn

Go:   strings.Count(s, "a")
来源：http://htm.vehdjk.com

Ruby: s.count("a")
来源：http://kcv.xziqi.cn

C#:   s.Count(c => c == 'a')
来源：http://cez.ppjwa.cn

[E13] 逐字符遍历
来源：http://ebj.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://nxs.shanyushiyangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mbk.shanyushiyangtech.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uiq.0kj1m.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wvv.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bhg.fanxiaobao.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oxn.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ayg.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://psv.jianghu66.top

[E14] URL 编码与 Base64
来源：http://nzk.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qkc.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://sko.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ckf.shzxlz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tok.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vrs.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://knf.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cyj.shzxlz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bcm.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://dwk.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lzv.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dym.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://efu.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gjb.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wyy.meibo888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://loh.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rbt.xuetiantiany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jda.aizwys.cn

[E16] 数字千分位
来源：http://awn.wangdashe.top

Py:   f"{1234567:,}"
来源：http://gha.chenjidiqi.icu

PHP:  number_format(1234567);
来源：http://tex.quarkkingdee.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ndl.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://shj.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tkb.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kob.jinghuilouyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xcf.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://gmv.nanxuanxn.top

[E17] 首字母大写
来源：http://mzi.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jly.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ycr.jinyuanbaomall.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xfp.xinyue.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wsu.yj202588.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rlr.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jtz.tarul.cn

Ruby: s.capitalize
来源：http://tow.jlsjyb.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xgh.pycfn.com

[E18] 模板占位符替换
来源：http://ekz.yj20258.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://org.uphjek.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rou.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nai.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yws.jlsjyb.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fng.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bbu.redwolf501.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ule.fanxiaobao.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://whc.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://heb.hcnkem.com

Py:   s.splitlines()
来源：http://ifv.hywenlv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hja.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://rif.yongpay.top

TS:   s.split(/\r?\n/)
来源：http://ikw.daxiang520.top

Java: s.lines().toList()
来源：http://wqs.bbcook.cn

Go:   strings.Split(s, "\n")
来源：http://kdf.yvedp.cn

Ruby: s.lines
来源：http://ivq.daxiang520.top

C#:   s.Split('\n')
来源：http://bof.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://jsj.andypj.xyz

Py:   if not s:
来源：http://vka.zhoulong.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fts.nanxinkj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vdz.jyoumei.cn

TS:   if (s === "") {}
来源：http://pjd.jqgfzy.top

Java: if (s.isEmpty()) {}
来源：http://wdn.aizwys.cn

Go:   if s == "" {}
来源：http://uxa.aibaodan.cn

Ruby: if s.empty?
来源：http://gbl.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qsa.birdmap.top

[E21] 超长截断加省略号
来源：http://ren.zhongyouzk.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nbr.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hwz.ywan-chungtsiang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cpp.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://apo.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jwz.yj202588.top

Go:   // 按 rune 判断长度后截断
来源：http://dwl.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cgg.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pbo.pycfn.com

[E22] 字节长度与字符长度
来源：http://nxb.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://msb.xingfuxueyuan.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://idn.wangshuangyany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://slr.guannengcc.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vhf.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kuw.shangyingyoupin.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zex.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://tjv.ydjk.org.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lyg.pycfn.com

================================================================================
来源：http://sau.snrcjt.cn

F. 文件与目录
来源：http://trc.gogol.net.cn

================================================================================
来源：http://nma.sxryk.cn

[F01] 读取整个文件
来源：http://qsr.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aar.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://wto.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://egt.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bbc.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://cza.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tut.fengsongda.top

Ruby: File.read("a.txt")
来源：http://ubz.fktsv.cn

C#:   File.ReadAllText("a.txt");
来源：http://rrd.havefunace.top

[F02] 逐行读取文件
来源：http://rox.sufxvd.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ypr.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kml.yvedp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mam.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lfj.wangshuangyany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zem.zhongyouzk.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gqd.xingfuxueyuan.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tbe.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jmh.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://svm.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xwk.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://alu.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vwn.ehwqpu.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tpo.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pxe.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ptc.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://cak.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mcy.zdbjq.cn

[F04] 追加写入文件
来源：http://hcy.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pnb.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hty.tian-w.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uwv.c1oappe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tye.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xdg.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rua.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wzg.quarkkingdee.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fbd.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://nye.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sgn.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://luk.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://uex.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://ywd.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ezw.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bqt.dianchejie.cn

Ruby: File.exist?("a.txt")
来源：http://uyb.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://fix.xuanzx.com

[F06] 删除文件
来源：http://yhf.vehdjk.com

Py:   os.remove("a.txt")
来源：http://jzt.snrcjt.cn

PHP:  unlink("a.txt");
来源：http://blf.gaohongyu789.top

JS:   fs.unlinkSync("a.txt")
来源：http://aeg.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://trt.sxryk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gpq.ivvv.top

Go:   os.Remove("a.txt")
来源：http://xak.chenjidiqi.icu

Ruby: File.delete("a.txt")
来源：http://xmg.ydzc1.top

C#:   File.Delete("a.txt");
来源：http://crp.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://jtl.316326.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gvt.tianlin.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ajp.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uyd.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vam.ctjpmb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hmr.guowangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zse.0kj1m.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qvq.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cqf.jlsjyb.cn

[F08] 遍历目录
来源：http://tqf.snrcjt.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yqs.0kj1m.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yoi.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://gai.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://vqa.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nbv.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ros.quarkkingdee.top

Ruby: Dir.children("dir")
来源：http://ddz.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://fng.nanxuanxn.top

[F09] 获取文件大小
来源：http://kgh.birdmap.top

Py:   os.path.getsize("a.txt")
来源：http://sue.fanxiaobao.xyz

PHP:  filesize("a.txt");
来源：http://qyx.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://hvv.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://nkn.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://lhk.bjfxy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://psx.hnxiangtu.top

Ruby: File.size("a.txt")
来源：http://icz.epnwcf.com

C#:   new FileInfo("a.txt").Length
来源：http://wcr.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://tvr.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zzt.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pnf.sjlbkw.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ogw.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://bhb.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zod.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mvy.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lyl.nanxinkj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oqj.svipenyu.cn

[F11] 复制与移动文件
来源：http://jjl.yueranfly.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lmg.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kgw.xinyue.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://niy.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rny.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fkm.jyoumei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ajh.hammf.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xfk.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ihb.uphjek.com

[F12] CSV 读写
来源：http://nwo.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pns.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hxh.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lmx.shuidangran.top

TS:   // 同上
来源：http://eoe.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tru.fengsongda.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yhu.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://esu.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ziu.chenjidiqi.icu

================================================================================
来源：http://sce.jianghu66.top

G. 面向对象
来源：http://wus.tian-w.cn

================================================================================
来源：http://jdw.uphjek.com

[G01] 定义类
来源：http://gam.jinghuilouyu.cn

Py:   class User: pass
来源：http://tkf.ivvv.top

PHP:  class User {}
来源：http://qao.svipenyu.cn

JS:   class User {}
来源：http://yxq.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://fvi.dianchejie.cn


<!-- 参考信息 -->