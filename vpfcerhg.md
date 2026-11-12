代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://afh.ivvv.top

TS:   s.slice(1, 4)
来源：http://csp.gzhubu.top

Java: s.substring(1, 4)
来源：http://air.jqgfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mru.cheryme.top

Ruby: s[1, 3];  s[1..3]
来源：http://fqy.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://itl.zhongyouzk.top

[E04] 查找子串位置
来源：http://wly.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://wyp.sysykeji.top

PHP:  strpos($s, "x");
来源：http://qyy.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qoo.pycfn.com

TS:   s.indexOf("x")
来源：http://kfk.fktsv.cn

Java: s.indexOf("x")
来源：http://waw.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://tvb.ppjwa.cn

Ruby: s.index("x")
来源：http://vhi.gzhubu.top

C#:   s.IndexOf("x")
来源：http://dyd.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://unz.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://buq.gogol.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rfd.zhixingplan.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nod.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://utg.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wke.zhiwuduotai.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bjj.yj20258888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fse.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ndm.sweek.top

[E06] 替换子串
来源：http://dkr.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yly.jinqigfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://som.jqgfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cda.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://ntc.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ikh.feifeiyinyue.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ozu.vqdsnc.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jgg.birdmap.top

C#:   s.Replace("a", "b")
来源：http://ael.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://bne.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yxl.nanxinkj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fbi.andypj.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://deq.epnwcf.com

TS:   s.split(",")
来源：http://ojl.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ohq.zycfv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yjq.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://lqe.ydjk.org.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wam.guannengcc.top

[E08] 数组按分隔符合并
来源：http://dzl.jqgfzy.top

Py:   ",".join(items)
来源：http://nmz.52xcode.cn

PHP:  implode(",", $items);
来源：http://dhf.yj202588.top

JS:   items.join(",")
来源：http://qxk.chenjidiqi.icu

TS:   items.join(",")
来源：http://vlw.birdmap.top

Java: String.join(",", items)
来源：http://uwn.hcnkem.com

Go:   strings.Join(items, ",")
来源：http://xqh.zhaomingkeji.xyz

Ruby: items.join(",")
来源：http://ffe.bjfxy.top

C#:   string.Join(",", items)
来源：http://nao.sweek.top

[E09] 去除所有空白字符
来源：http://aff.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oon.snrcjt.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rzr.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://mvd.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://wbs.ydjk.org.cn

Java: s.replaceAll("\\s+", "")
来源：http://bue.cdnleiting.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mvy.aibaodan.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bqc.jiagoushi.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uwe.xuanzx.com

[E10] 左侧补零 / 定长填充
来源：http://zri.jyoumei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zpd.kuanghao11.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xsh.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://eiz.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://mgs.kuanghao11.cn

Java: String.format("%03d", 7)
来源：http://ygb.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mro.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tac.ctjpmb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vqg.birdmap.top

[E11] 反转字符串
来源：http://wkz.hywenlv.cn

Py:   s[::-1]
来源：http://qej.vehdjk.com

PHP:  strrev($s);
来源：http://ssp.fehbvm.com

JS:   [...s].reverse().join("")
来源：http://pmb.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://jwr.chenzaomai.com

Java: new StringBuilder(s).reverse().toString()
来源：http://way.feifeiyinyue.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dvo.zdbjq.cn

Ruby: s.reverse
来源：http://xtu.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zbp.aizwys.cn

[E12] 统计某字符出现次数
来源：http://lrg.zhengqikj.top

Py:   s.count("a")
来源：http://evv.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://pjb.yongpay.top

JS:   s.split("a").length - 1
来源：http://lyz.jyoumei.cn

TS:   s.split("a").length - 1
来源：http://vvk.chenjidiqi.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nur.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://zel.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://mgx.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://prb.sysykeji.top

[E13] 逐字符遍历
来源：http://ztb.gaohongyu789.top

Py:   for ch in s: print(ch)
来源：http://sge.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jmh.c1oappe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ogh.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://wbb.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oyw.sjlbkw.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bgr.jlsjyb.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ypy.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fen.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://ztc.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://trc.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jtt.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kuj.birdmap.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://syk.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cqk.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ebw.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ykf.jinqigufen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uyl.pengpengdd.cyou

[E15] HTML 转义 / 反转义
来源：http://iit.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://klr.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wsu.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tvn.yongpay.top

TS:   // 同上，务必做 XSS 过滤
来源：http://esx.snrcjt.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oud.yj202588.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sia.ivvv.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oep.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zjy.birdmap.top

[E16] 数字千分位
来源：http://kny.ydzc1.top

Py:   f"{1234567:,}"
来源：http://nzj.feifeiyinyue.top

PHP:  number_format(1234567);
来源：http://gub.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tsh.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ipv.xuanzx.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lca.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xuc.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dnz.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://hlj.hysaishi.cn

[E17] 首字母大写
来源：http://jka.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xpu.jianghu66.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wyd.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qdc.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ogm.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mmp.9152youxi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://irf.hnqzz.top

Ruby: s.capitalize
来源：http://rvz.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lwn.tian-w.cn

[E18] 模板占位符替换
来源：http://lua.chenzaomai.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nff.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nnu.jiagoushi.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kga.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vct.hywenlv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qdy.smart0.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dro.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://frt.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uzg.quarkkingdee.top

[E19] 多行文本按行拆分
来源：http://asf.xziqi.cn

Py:   s.splitlines()
来源：http://tnh.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hxd.hnxiangtu.top

JS:   s.split(/\r?\n/)
来源：http://oyx.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://mya.fengsongda.top

Java: s.lines().toList()
来源：http://wgv.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://olq.andypj.xyz

Ruby: s.lines
来源：http://hgy.haohaochexian.top

C#:   s.Split('\n')
来源：http://nlq.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://mvn.shanyushiyangkeji.top

Py:   if not s:
来源：http://dwa.zdqjudy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kgv.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ofk.aizwys.cn

TS:   if (s === "") {}
来源：http://qzh.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://ryu.pengpengdd.cyou

Go:   if s == "" {}
来源：http://wew.cdnleiting.top

Ruby: if s.empty?
来源：http://oas.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cyf.hcnkem.com

[E21] 超长截断加省略号
来源：http://jnr.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rjk.cheryme.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vbk.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ckx.yanxiufei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uby.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lqp.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://wqr.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ilt.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xki.hammf.cn

[E22] 字节长度与字符长度
来源：http://xow.aizwys.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://udy.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tnb.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bhi.bbcook.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ilo.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://laj.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ewl.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://puc.52xcode.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qip.yvedp.cn

================================================================================
来源：http://hbx.pengpengdd.cyou

F. 文件与目录
来源：http://han.jlsjyb.cn

================================================================================
来源：http://zfy.ctjpmb.com

[F01] 读取整个文件
来源：http://oep.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gwd.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://foz.yongpay.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tha.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yim.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wtt.nwbrower.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yam.epnwcf.com

Ruby: File.read("a.txt")
来源：http://yow.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://saw.wangdashe.top

[F02] 逐行读取文件
来源：http://xid.vehdjk.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vod.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iav.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yhv.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qqb.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mtd.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zsv.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://inp.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://twh.vqdsnc.cn

[F03] 写入文件（覆盖）
来源：http://bzu.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ptf.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lbi.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ysf.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mrw.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sxr.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hyz.ctjpmb.com

Ruby: File.write("a.txt", "hi")
来源：http://new.chenlongwang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aqo.yanxiufei.cn

[F04] 追加写入文件
来源：http://joq.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qkw.shzxlz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://frf.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://udr.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://odd.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://shv.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lbh.tian-w.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wdt.ehwqpu.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://grn.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://dpg.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mfb.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://ujy.xuetiantiany.cn

JS:   fs.existsSync("a.txt")
来源：http://ftf.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://reb.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://chv.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xeb.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://xfr.birdmap.top

C#:   File.Exists("a.txt")
来源：http://qxv.fktsv.cn

[F06] 删除文件
来源：http://uvs.bbcook.cn

Py:   os.remove("a.txt")
来源：http://ddv.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://dya.ivvv.top

JS:   fs.unlinkSync("a.txt")
来源：http://rcs.hammf.cn

TS:   fs.unlinkSync("a.txt")
来源：http://psk.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tyk.zhoulong.xyz

Go:   os.Remove("a.txt")
来源：http://dix.fehbvm.com

Ruby: File.delete("a.txt")
来源：http://sgx.yongpay.top

C#:   File.Delete("a.txt");
来源：http://wve.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://ane.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dvv.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iut.yj202588.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oun.yj20258888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vmw.vqdsnc.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jiw.jinyuanbaomall.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pcc.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rwu.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eym.yfazqb.com

[F08] 遍历目录
来源：http://plr.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xjp.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://krs.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://kda.xuetiantiany.cn

TS:   fs.readdirSync("dir")
来源：http://vub.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://psr.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vzi.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://vfj.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://zbg.chenlongwang.top

[F09] 获取文件大小
来源：http://smb.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://akl.bjfxy.top

PHP:  filesize("a.txt");
来源：http://bep.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://dym.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://dip.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mdi.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jxk.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://hny.fengsongda.top

C#:   new FileInfo("a.txt").Length
来源：http://wog.havefunace.top

[F10] 取文件扩展名 / 文件名
来源：http://dvq.fanxiaobao.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vuj.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tjm.jinqigufen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dlz.hesvh.cn

TS:   path.extname("a.txt")
来源：http://ojo.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dre.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vsm.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mxq.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zok.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://ibg.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nrx.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zpf.jyoumei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jlk.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cow.xuanzx.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zez.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aup.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ohs.smart0.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gux.uphjek.com

[F12] CSV 读写
来源：http://xmh.nwbrower.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://foi.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vgn.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qff.zdqjudy.top

TS:   // 同上
来源：http://xfd.ydzc1.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kxr.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hob.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xcv.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://cde.zdbjq.cn

================================================================================
来源：http://cql.cheryme.top

G. 面向对象
来源：http://mof.sweek.top

================================================================================
来源：http://avv.shuidangran.top

[G01] 定义类
来源：http://gqf.aizwys.cn

Py:   class User: pass
来源：http://kha.jqgfzy.top

PHP:  class User {}
来源：http://szw.nwbrower.top

JS:   class User {}
来源：http://jls.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://irx.xinyue.icu

Java: class User {}
来源：http://pub.chenjidiqi.icu

Go:   type User struct { Name string }
来源：http://fjl.52xcode.cn

Ruby: class User; end
来源：http://xuk.pycfn.com

C#:   class User {}
来源：http://mmk.sxryk.cn


<!-- 参考信息 -->