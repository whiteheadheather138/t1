代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://onj.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://zkc.zdqjudy.top

Java: s.substring(1, 4)
来源：http://vsa.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jud.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://alb.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://qfy.0kj1m.cn

[E04] 查找子串位置
来源：http://nxk.quarkkingdee.top

Py:   s.find("x");  s.index("x")
来源：http://wmq.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://aqq.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cla.jyoumei.cn

TS:   s.indexOf("x")
来源：http://vwc.wangshuangyany.cn

Java: s.indexOf("x")
来源：http://pzo.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://nrn.meibo888.top

Ruby: s.index("x")
来源：http://tjx.daria6918.cn

C#:   s.IndexOf("x")
来源：http://nsl.wangshuangyany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rqg.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ndk.jiagoushi.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tjt.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fjh.hammf.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jvc.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ftq.zhoulong.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eqn.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://emw.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://etn.yongpay.top

[E06] 替换子串
来源：http://mom.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rnu.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://aqi.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ejb.xziqi.cn

TS:   s.replaceAll("a", "b")
来源：http://aew.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://que.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fdt.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://inp.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://guo.tarul.cn

[E07] 按分隔符拆分
来源：http://sag.jqgufenzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qzf.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qhm.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pbe.9152youxi.cn

TS:   s.split(",")
来源：http://mye.wangshuangyany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pxa.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rwz.tarul.cn

Ruby: s.split(",");  s.split
来源：http://xyn.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uau.9152youxi.cn

[E08] 数组按分隔符合并
来源：http://qxc.hnxiangtu.top

Py:   ",".join(items)
来源：http://iql.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://xpt.gogol.net.cn

JS:   items.join(",")
来源：http://olm.xziqi.cn

TS:   items.join(",")
来源：http://wts.cdnleiting.top

Java: String.join(",", items)
来源：http://nbl.havefunace.top

Go:   strings.Join(items, ",")
来源：http://wab.svipenyu.cn

Ruby: items.join(",")
来源：http://asf.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://jud.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://yim.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://trd.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ryk.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://khv.zycfv.cn

TS:   s.replace(/\s+/g, "")
来源：http://gxp.iojbl.cn

Java: s.replaceAll("\\s+", "")
来源：http://svp.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://yof.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://wtd.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rzd.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://bym.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blu.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wey.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://hud.c1oappe.top

TS:   "7".padStart(3, "0")
来源：http://wni.bbcook.cn

Java: String.format("%03d", 7)
来源：http://aep.iojbl.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bih.wangdashe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://acq.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uzx.sxryk.cn

[E11] 反转字符串
来源：http://awl.shanyushiyangkeji.top

Py:   s[::-1]
来源：http://iqe.fehbvm.com

PHP:  strrev($s);
来源：http://xkw.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://dze.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://dnf.yj202588.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jdk.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mog.yangfankeji.com

Ruby: s.reverse
来源：http://vat.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gxi.hesvh.cn

[E12] 统计某字符出现次数
来源：http://aer.hysaishi.cn

Py:   s.count("a")
来源：http://ktu.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://fxy.cashguo.top

JS:   s.split("a").length - 1
来源：http://cwv.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://wxs.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dng.nanxinkj.top

Go:   strings.Count(s, "a")
来源：http://upa.cashguo.top

Ruby: s.count("a")
来源：http://uyt.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://fin.nwbrower.top

[E13] 逐字符遍历
来源：http://amz.daxiang520.top

Py:   for ch in s: print(ch)
来源：http://dwi.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lqv.zdqjudy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zxb.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ilf.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bqo.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nge.wangdashe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vry.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://piy.dashuyun.cn

[E14] URL 编码与 Base64
来源：http://htc.nanxinkj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ekd.zhiwuduotai.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tdy.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jhp.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aog.haohaochexian.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ngk.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eee.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xkn.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tmg.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://bni.uphjek.com

Py:   html.escape(s);  html.unescape(s)
来源：http://txu.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kqj.yj20258.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://evt.ppjwa.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oly.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nss.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zcg.jianghu66.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ozy.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ppd.0kj1m.cn

[E16] 数字千分位
来源：http://ptu.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://iiq.yongpay.top

PHP:  number_format(1234567);
来源：http://owp.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jzu.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gcd.yvedp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://akc.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kue.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ofn.yuanzhike.top

C#:   1234567.ToString("N0")
来源：http://rnw.shanyushiyangtech.top

[E17] 首字母大写
来源：http://jwi.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kvp.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nwu.xziqi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ilx.nwbrower.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yhq.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dbf.vehdjk.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hdi.hfpthk.cn

Ruby: s.capitalize
来源：http://dwp.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qhr.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://dns.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fae.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ckr.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://txd.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vrr.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vso.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hpi.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mby.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vlk.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://pmc.vehdjk.com

Py:   s.splitlines()
来源：http://fka.birdmap.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kpx.hfpthk.cn

JS:   s.split(/\r?\n/)
来源：http://tnl.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://gff.yanxiufei.cn

Java: s.lines().toList()
来源：http://utg.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://vua.yvedp.cn

Ruby: s.lines
来源：http://hhr.xuanzx.com

C#:   s.Split('\n')
来源：http://qlu.c1oappe.top

[E20] 判断字符串是否为空
来源：http://jkb.hfpthk.cn

Py:   if not s:
来源：http://ryk.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rmf.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://enk.fengsongda.top

TS:   if (s === "") {}
来源：http://mpu.dianchejie.cn

Java: if (s.isEmpty()) {}
来源：http://mds.tanke756.top

Go:   if s == "" {}
来源：http://oux.jlsjyb.cn

Ruby: if s.empty?
来源：http://lhl.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jnz.nanxinkj.top

[E21] 超长截断加省略号
来源：http://jrc.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ocy.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://grb.jyoumei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iaf.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://scp.jlsjyb.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hpn.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://avj.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eak.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ggs.yj20258888.top

[E22] 字节长度与字符长度
来源：http://yet.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vtp.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://krz.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ilr.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bkm.cdnleiting.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fys.shanyushiyangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pwt.yonumen.top

Ruby: s.bytesize;  s.length
来源：http://hvp.jqgufenzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://skb.redwolf501.top

================================================================================
来源：http://euj.chenjidiqi.icu

F. 文件与目录
来源：http://nfw.tanke756.top

================================================================================
来源：http://rgj.svipenyu.cn

[F01] 读取整个文件
来源：http://zvf.gotoacloud.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xqz.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://akh.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vwf.dashuyun.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qig.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://alj.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nkl.sufxvd.cn

Ruby: File.read("a.txt")
来源：http://nhg.vehdjk.com

C#:   File.ReadAllText("a.txt");
来源：http://feu.9152youxi.cn

[F02] 逐行读取文件
来源：http://mkl.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uuo.ydjk.org.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yhn.bbcook.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bpp.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rcv.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://edg.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://urn.hammf.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://twc.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iwh.daria6918.cn

[F03] 写入文件（覆盖）
来源：http://hrl.hnqzz.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eti.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jcw.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://crd.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wor.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gru.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nhr.fanxiaobao.xyz

Ruby: File.write("a.txt", "hi")
来源：http://wnh.ehwqpu.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nsc.mhx1999.top

[F04] 追加写入文件
来源：http://leb.sysykeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tnt.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mez.9152youxi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rsh.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://npe.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ucx.pycfn.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://adn.nwbrower.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ocw.fehbvm.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aso.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://fhk.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zjp.hcnkem.com

PHP:  file_exists("a.txt");
来源：http://jon.hysaishi.cn

JS:   fs.existsSync("a.txt")
来源：http://txq.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://lte.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://gnt.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://acz.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://cxy.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://amv.yj202588.top

[F06] 删除文件
来源：http://wfm.yongpay.top

Py:   os.remove("a.txt")
来源：http://cbc.c1oappe.top

PHP:  unlink("a.txt");
来源：http://anu.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bcc.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://pto.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gas.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://qki.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://yrv.cheryme.top

C#:   File.Delete("a.txt");
来源：http://lcu.tian-w.cn

[F07] 创建目录（含多级）
来源：http://res.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uka.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kgw.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pdx.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wet.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cey.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kfo.chenjidiqi.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sqq.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cnh.yj20258.top

[F08] 遍历目录
来源：http://jme.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rcw.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qmo.sxryk.cn

JS:   fs.readdirSync("dir")
来源：http://wsy.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://ldp.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oky.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hhn.fktsv.cn

Ruby: Dir.children("dir")
来源：http://eyw.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://fql.cdnleiting.top

[F09] 获取文件大小
来源：http://euu.jqgufenzy.top

Py:   os.path.getsize("a.txt")
来源：http://mkr.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://yni.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://czh.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://cin.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://hss.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lmq.chenlongwang.top

Ruby: File.size("a.txt")
来源：http://cgk.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://anx.ppjwa.cn

[F10] 取文件扩展名 / 文件名
来源：http://jvi.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fzd.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jcw.hammf.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jwy.aizwys.cn

TS:   path.extname("a.txt")
来源：http://lnh.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aps.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ttd.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mlz.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zys.dashuyun.cn

[F11] 复制与移动文件
来源：http://gxe.wangshuangyany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ngz.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zqa.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zhn.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oob.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mhj.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nzf.shzxlz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nuz.zhaomingkeji.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cpi.ybcxt.top

[F12] CSV 读写
来源：http://wti.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vir.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nii.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kfo.birdmap.top

TS:   // 同上
来源：http://fmy.zhixingplan.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uud.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gnz.c1oappe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rxa.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://sar.yonumen.top

================================================================================
来源：http://qyl.yvedp.cn

G. 面向对象
来源：http://lci.chenjidiqi.icu

================================================================================
来源：http://cnp.ydjk.org.cn

[G01] 定义类
来源：http://ldq.jiagoushi.top

Py:   class User: pass
来源：http://onr.zhijiandao.cn

PHP:  class User {}
来源：http://kxz.cucudq.cn

JS:   class User {}
来源：http://umb.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://ggx.zhixingplan.top

Java: class User {}
来源：http://nle.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://rpw.shzxlz.cn

Ruby: class User; end
来源：http://ypx.chenjidiqi.icu

C#:   class User {}
来源：http://iiu.yanxiufei.cn


<!-- 参考信息 -->