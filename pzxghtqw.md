代发 wailian999

[E02] 重复字符串
来源：http://cta.yueranfly.top

Py:   "ab" * 3
来源：http://gcn.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://coq.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://scn.sxryk.cn

TS:   "ab".repeat(3)
来源：http://wsi.guowangkeji.top

Java: "ab".repeat(3)
来源：http://hyh.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://lqm.yonumen.top

Ruby: "ab" * 3
来源：http://cpr.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://typ.bbcook.cn

[E03] 截取子串
来源：http://fwm.gogol.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cox.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://byn.xuanzx.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cpk.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://oax.yj202588.top

Java: s.substring(1, 4)
来源：http://ymn.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qst.chenlongwang.top

Ruby: s[1, 3];  s[1..3]
来源：http://dhy.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://lba.xinyue.icu

[E04] 查找子串位置
来源：http://zvd.ydzc1.top

Py:   s.find("x");  s.index("x")
来源：http://gki.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://vgq.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qyp.xingfuxueyuan.xyz

TS:   s.indexOf("x")
来源：http://qbm.tian-w.cn

Java: s.indexOf("x")
来源：http://kna.hywenlv.cn

Go:   strings.Index(s, "x")
来源：http://nbi.chenzaomai.com

Ruby: s.index("x")
来源：http://ylc.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://fou.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://szn.mhx1999.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://inb.sufxvd.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bpm.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gps.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://uxf.hongshengwenyu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xie.sysykeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://obe.yj20258888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aex.cashguo.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ohz.jinqigufen.top

[E06] 替换子串
来源：http://tur.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wmy.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://zgu.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://exv.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://tgb.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gmr.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nez.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hrt.yj202588.top

C#:   s.Replace("a", "b")
来源：http://kzn.ybcxt.top

[E07] 按分隔符拆分
来源：http://lvu.yvedp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jat.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zpp.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wem.cashguo.top

TS:   s.split(",")
来源：http://bpn.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fpd.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ohw.dashuyun.cn

Ruby: s.split(",");  s.split
来源：http://pib.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://arr.yfazqb.com

[E08] 数组按分隔符合并
来源：http://cbe.zhixingplan.top

Py:   ",".join(items)
来源：http://dzv.daxiang520.top

PHP:  implode(",", $items);
来源：http://hny.daxiang520.top

JS:   items.join(",")
来源：http://hnd.ydjk.org.cn

TS:   items.join(",")
来源：http://gyh.yj20258888.top

Java: String.join(",", items)
来源：http://foi.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://mwu.hammf.cn

Ruby: items.join(",")
来源：http://huw.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://rmo.hywenlv.cn

[E09] 去除所有空白字符
来源：http://ulo.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hza.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oiu.xingfuxueyuan.xyz

JS:   s.replace(/\s+/g, "")
来源：http://jbg.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://eqb.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://rkp.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://drs.mhx1999.top

Ruby: s.gsub(/\s+/, "")
来源：http://wgl.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aqx.sjlbkw.cn

[E10] 左侧补零 / 定长填充
来源：http://rda.xziqi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wbs.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hun.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://was.ybcxt.top

TS:   "7".padStart(3, "0")
来源：http://eol.shangyingyoupin.top

Java: String.format("%03d", 7)
来源：http://fqh.jinqigufen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jtn.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vxr.tarul.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tro.zhongyouzk.top

[E11] 反转字符串
来源：http://tqy.hongshengwenyu.top

Py:   s[::-1]
来源：http://qkz.ivvv.top

PHP:  strrev($s);
来源：http://pfd.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://qji.wangdashe.top

TS:   [...s].reverse().join("")
来源：http://yef.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://asx.gogol.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vfj.jinyuanbaomall.cn

Ruby: s.reverse
来源：http://yyt.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://amf.hfpthk.cn

[E12] 统计某字符出现次数
来源：http://oeg.hfpthk.cn

Py:   s.count("a")
来源：http://idk.yonumen.top

PHP:  substr_count($s, "a");
来源：http://xas.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://rrv.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://hnd.yvedp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://snt.zhoulong.xyz

Go:   strings.Count(s, "a")
来源：http://ktw.zhongyouzk.top

Ruby: s.count("a")
来源：http://yyi.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://kxn.andypj.xyz

[E13] 逐字符遍历
来源：http://nvc.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://ntl.jlsjyb.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ibk.shanyushiyangtech.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nsv.pycfn.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://hkd.yj20258.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jwn.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ddp.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://rzg.jiagoushi.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pmd.dashuyun.cn

[E14] URL 编码与 Base64
来源：http://clw.feifeiyinyue.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wea.yj20258888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ylv.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ojy.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tqk.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qrk.chenzaomai.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://atz.cqqwz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qwd.smart0.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://prg.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://wij.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ntp.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eyr.xingfuxueyuan.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://agt.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qui.shuidangran.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dzw.gogol.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://urb.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fmv.bbcook.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ytn.zycfv.cn

[E16] 数字千分位
来源：http://nbg.xinyue.icu

Py:   f"{1234567:,}"
来源：http://lha.sysykeji.top

PHP:  number_format(1234567);
来源：http://gyb.cdnleiting.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gxh.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://puf.cucudq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hzt.zhiwuduotai.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jiq.ydzc1.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gpm.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://wjc.uphjek.com

[E17] 首字母大写
来源：http://lqe.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oam.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vws.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ujp.jinyuanbaomall.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jpm.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hhe.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mny.hysaishi.cn

Ruby: s.capitalize
来源：http://xss.smart0.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qmd.guannengcc.top

[E18] 模板占位符替换
来源：http://pbw.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ezm.hcnkem.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mvy.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kit.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jhh.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://imu.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fdy.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hxh.shanyushiyangtech.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ywd.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://zwa.zhengqikj.top

Py:   s.splitlines()
来源：http://hkq.yonumen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zwm.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://cbu.cashguo.top

TS:   s.split(/\r?\n/)
来源：http://udn.wangdashe.top

Java: s.lines().toList()
来源：http://ndr.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://crb.pycfn.com

Ruby: s.lines
来源：http://hmu.hysaishi.cn

C#:   s.Split('\n')
来源：http://puq.cheryme.top

[E20] 判断字符串是否为空
来源：http://hhv.zdbjq.cn

Py:   if not s:
来源：http://gyi.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ziy.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bic.zdbjq.cn

TS:   if (s === "") {}
来源：http://som.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://dcq.kuanghao11.cn

Go:   if s == "" {}
来源：http://dpc.chenlongwang.top

Ruby: if s.empty?
来源：http://hwn.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zjm.gogol.net.cn

[E21] 超长截断加省略号
来源：http://gtv.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oqk.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zga.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qip.zdbjq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zrg.jiagoushi.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cnb.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://ntw.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hra.smart0.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cxn.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://fiz.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wsl.shuidangran.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yty.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kaa.ywan-chungtsiang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rly.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://euk.mhx1999.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hty.cqqwz.cn

Ruby: s.bytesize;  s.length
来源：http://odg.xylfe.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dwu.jinghuilouyu.cn

================================================================================
来源：http://oqj.tarul.cn

F. 文件与目录
来源：http://qnx.yonumen.top

================================================================================
来源：http://cnp.ybcxt.top

[F01] 读取整个文件
来源：http://xzs.bjfxy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ewh.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://xwn.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mdd.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uuj.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yre.ctjpmb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ach.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://zhq.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://abw.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://ocl.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zvt.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cjs.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ykw.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nrt.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ywg.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yob.jqgfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ukv.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nzn.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://zmf.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zmh.wangdashe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dff.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cxk.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nun.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://imh.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qtc.hcnkem.com

Ruby: File.write("a.txt", "hi")
来源：http://kiy.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rva.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://fxn.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oqs.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qlb.9152youxi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://avp.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uhb.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tip.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kwz.0kj1m.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oyv.jqgufenzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pst.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://xkj.cdnleiting.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ibf.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://uek.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://mnj.sjlbkw.cn

TS:   fs.existsSync("a.txt")
来源：http://khk.xuetiantiany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xbx.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://llw.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://rij.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://sxd.mhx1999.top

[F06] 删除文件
来源：http://bmq.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://bkl.nwbrower.top

PHP:  unlink("a.txt");
来源：http://gny.ctjpmb.com

JS:   fs.unlinkSync("a.txt")
来源：http://leq.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rxs.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xlc.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://okc.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://luy.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://uqg.hammf.cn

[F07] 创建目录（含多级）
来源：http://nlv.0kj1m.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vol.chenjidiqi.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fqq.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zpa.zhijiandao.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tlt.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jyq.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ftx.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cas.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://soh.hesvh.cn

[F08] 遍历目录
来源：http://baz.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://arx.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://avy.zhixingplan.top

JS:   fs.readdirSync("dir")
来源：http://wff.ydjk.org.cn

TS:   fs.readdirSync("dir")
来源：http://qfn.daxiang520.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://are.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ple.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://hbu.birdmap.top

C#:   Directory.GetFiles("dir")
来源：http://ybo.yonumen.top

[F09] 获取文件大小
来源：http://jru.shanyushiyangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://vro.hnqzz.top

PHP:  filesize("a.txt");
来源：http://gvh.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://aoy.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://yct.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wrk.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ezj.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://rep.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://zth.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://sgn.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://awn.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ini.ydzc1.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://skx.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://uyt.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://evh.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ail.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wdr.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://unq.yonumen.top

[F11] 复制与移动文件
来源：http://awb.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mml.shuidangran.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://slj.pycfn.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xjf.dianchejie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://puf.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yxf.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gbx.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vjp.gotoacloud.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lon.fanxiaobao.xyz

[F12] CSV 读写
来源：http://fwq.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ecp.bbcook.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tak.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vxd.yfazqb.com

TS:   // 同上
来源：http://hsa.zhijiandao.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cyc.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zxc.nanxuanxn.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://goq.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kbz.gotoacloud.top


<!-- 参考信息 -->