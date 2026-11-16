代发 wailian999

Java: String.join(", ", list)
来源：http://tdy.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://kpv.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://agf.cdnleiting.top

C#:   string.Join(", ", list)
来源：http://kvj.vehdjk.com

================================================================================
来源：http://htq.yanxiufei.cn

E. 字符串处理
来源：http://vah.yongpay.top

================================================================================
来源：http://zpe.kuanghao11.cn

[E01] 拼接字符串
来源：http://apo.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nvj.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sya.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gah.zhaomingkeji.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mpn.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hsi.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hpm.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bce.guannengcc.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wfi.jinqigufen.top

[E02] 重复字符串
来源：http://ovx.0kj1m.cn

Py:   "ab" * 3
来源：http://ggl.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://kgq.cucudq.cn

JS:   "ab".repeat(3)
来源：http://wgj.yj202588.top

TS:   "ab".repeat(3)
来源：http://tgi.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://dtz.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://uac.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://ejn.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bdq.yangfankeji.com

[E03] 截取子串
来源：http://xgk.birdmap.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://npi.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bso.sysykeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://odh.daria6918.cn

TS:   s.slice(1, 4)
来源：http://wiz.guowangkeji.top

Java: s.substring(1, 4)
来源：http://wjo.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ken.yvedp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://frl.sxryk.cn

C#:   s.Substring(1, 3)
来源：http://mst.sysykeji.top

[E04] 查找子串位置
来源：http://xnh.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://eyx.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://wys.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qzf.ydjk.org.cn

TS:   s.indexOf("x")
来源：http://snk.ctjpmb.com

Java: s.indexOf("x")
来源：http://wca.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://voq.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://djc.hesvh.cn

C#:   s.IndexOf("x")
来源：http://nmf.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jia.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kry.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rkk.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xpt.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zfu.aizwys.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mfl.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ctx.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eee.yanxiufei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://znv.52xcode.cn

[E06] 替换子串
来源：http://kxp.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://puk.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://abo.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fql.hywenlv.cn

TS:   s.replaceAll("a", "b")
来源：http://ced.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vqu.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ace.andypj.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bvy.xuanzx.com

C#:   s.Replace("a", "b")
来源：http://fgt.zhixingplan.top

[E07] 按分隔符拆分
来源：http://yba.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dhc.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ybe.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gbo.daxiang520.top

TS:   s.split(",")
来源：http://eix.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://soa.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://noa.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://hbd.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yxs.tarul.cn

[E08] 数组按分隔符合并
来源：http://ycs.zdqjudy.top

Py:   ",".join(items)
来源：http://mtb.jyoumei.cn

PHP:  implode(",", $items);
来源：http://zeg.zycfv.cn

JS:   items.join(",")
来源：http://mqz.hysaishi.cn

TS:   items.join(",")
来源：http://eus.wangshuangyany.cn

Java: String.join(",", items)
来源：http://ddl.yuxming.cn

Go:   strings.Join(items, ",")
来源：http://tus.zhengqikj.top

Ruby: items.join(",")
来源：http://qyi.ehwqpu.com

C#:   string.Join(",", items)
来源：http://wcs.gotoacloud.top

[E09] 去除所有空白字符
来源：http://yza.jinyuanbaomall.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bov.xuanzx.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vjs.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://noj.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://cqj.jinqigfzy.top

Java: s.replaceAll("\\s+", "")
来源：http://ysr.chenzaomai.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://igu.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pec.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ula.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://sjr.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aew.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vnv.gogol.net.cn

JS:   "7".padStart(3, "0")
来源：http://anu.xuetiantiany.cn

TS:   "7".padStart(3, "0")
来源：http://nfe.hcnkem.com

Java: String.format("%03d", 7)
来源：http://sud.chenlongwang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hxs.ctjpmb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tdm.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kpl.fanxiaobao.xyz

[E11] 反转字符串
来源：http://itf.ybcxt.top

Py:   s[::-1]
来源：http://oxa.52xcode.cn

PHP:  strrev($s);
来源：http://hil.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://ddp.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://ddn.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qxx.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://gxb.cucudq.cn

Ruby: s.reverse
来源：http://cne.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://bwb.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://mrg.wangdashe.top

Py:   s.count("a")
来源：http://jvi.sxryk.cn

PHP:  substr_count($s, "a");
来源：http://toj.havefunace.top

JS:   s.split("a").length - 1
来源：http://wfu.yueranfly.top

TS:   s.split("a").length - 1
来源：http://rsc.jinqigufen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iay.yj20258.top

Go:   strings.Count(s, "a")
来源：http://tmy.jqgfzy.top

Ruby: s.count("a")
来源：http://pug.bbcook.cn

C#:   s.Count(c => c == 'a')
来源：http://slh.shzxlz.cn

[E13] 逐字符遍历
来源：http://juh.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://yjx.shangyingyoupin.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uzq.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rvz.hammf.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ash.fengsongda.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://guq.guowangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mdr.hywenlv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ojv.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jog.tarul.cn

[E14] URL 编码与 Base64
来源：http://kyi.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pin.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hxv.sysykeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qns.xuanzx.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tzk.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cjw.ivvv.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eap.bjfxy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xho.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vzx.jinyuanbaomall.cn

[E15] HTML 转义 / 反转义
来源：http://ltk.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dui.hammf.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rcg.gaohongyu789.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ypz.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pug.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rgl.quarkkingdee.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kib.hnqzz.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sxh.jlsjyb.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zdu.ydjk.org.cn

[E16] 数字千分位
来源：http://doa.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://gny.haohaochexian.top

PHP:  number_format(1234567);
来源：http://nlx.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://saw.zycfv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nhf.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mjv.jinghuilouyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uit.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kyf.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://qcd.hammf.cn

[E17] 首字母大写
来源：http://iof.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rli.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ilw.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pvb.0kj1m.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wlp.zhijiandao.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tgz.shanyushiyangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lrs.redwolf501.top

Ruby: s.capitalize
来源：http://mri.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gff.iojbl.cn

[E18] 模板占位符替换
来源：http://tzj.vehdjk.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wnc.iojbl.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xug.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ork.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vyz.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sqq.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xbn.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xqj.sxryk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lhh.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://lvx.chenlongwang.top

Py:   s.splitlines()
来源：http://dhr.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://spb.ydzc1.top

JS:   s.split(/\r?\n/)
来源：http://emn.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://ivp.sxryk.cn

Java: s.lines().toList()
来源：http://ico.dashuyun.cn

Go:   strings.Split(s, "\n")
来源：http://brm.ehwqpu.com

Ruby: s.lines
来源：http://ddq.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://quq.gotoacloud.top

[E20] 判断字符串是否为空
来源：http://aov.snrcjt.cn

Py:   if not s:
来源：http://bro.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nqv.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kol.jinqigufen.top

TS:   if (s === "") {}
来源：http://jeu.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://kam.zdqjudy.top

Go:   if s == "" {}
来源：http://syf.nanxinkj.top

Ruby: if s.empty?
来源：http://pmv.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lev.nwbrower.top

[E21] 超长截断加省略号
来源：http://coj.0kj1m.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://skl.smart0.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ixu.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ueu.zhaomingkeji.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://azs.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lnm.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://njp.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qig.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://suc.shzxlz.cn

[E22] 字节长度与字符长度
来源：http://niv.fktsv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tch.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oyk.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://asf.shuidangran.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cio.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://akj.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://phm.jinqigfzy.top

Ruby: s.bytesize;  s.length
来源：http://akl.yvedp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lkr.jiagoushi.top

================================================================================
来源：http://btp.yueranfly.top

F. 文件与目录
来源：http://qgl.jyoumei.cn

================================================================================
来源：http://qur.hfpthk.cn

[F01] 读取整个文件
来源：http://fah.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rzs.pycfn.com

PHP:  file_get_contents("a.txt");
来源：http://acs.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ueb.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tzm.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://als.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fjy.nanxinkj.top

Ruby: File.read("a.txt")
来源：http://emu.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://yca.guowangkeji.top

[F02] 逐行读取文件
来源：http://dwi.vehdjk.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cgx.jinghuilouyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fhf.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zcw.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zxs.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qli.yj20258.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://voh.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mst.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ocq.dianchejie.cn

[F03] 写入文件（覆盖）
来源：http://qlu.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ffy.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://tof.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zms.jianghu66.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rmr.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jfo.mhx1999.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lph.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://nus.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bkg.epnwcf.com

[F04] 追加写入文件
来源：http://lpw.zdqjudy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bgf.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qex.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ndq.c1oappe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ita.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nuj.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zcy.zdbjq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kge.daria6918.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rmp.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://igb.ivvv.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gwo.meibo888.top

PHP:  file_exists("a.txt");
来源：http://zxs.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://cmr.xinyue.icu

TS:   fs.existsSync("a.txt")
来源：http://kon.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://mge.tian-w.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jom.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://rei.yanxiufei.cn

C#:   File.Exists("a.txt")
来源：http://inz.yj20258.top

[F06] 删除文件
来源：http://tny.zycfv.cn

Py:   os.remove("a.txt")
来源：http://jba.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://yjx.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hke.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://eub.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://smx.shuidangran.top

Go:   os.Remove("a.txt")
来源：http://ped.jlsjyb.cn

Ruby: File.delete("a.txt")
来源：http://snw.c1oappe.top

C#:   File.Delete("a.txt");
来源：http://jwe.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://jow.havefunace.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xkq.yvedp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ujl.guowangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xyt.yfazqb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pha.quarkkingdee.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://osv.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tsa.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cbq.cqqwz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://teq.shuidangran.top

[F08] 遍历目录
来源：http://ylr.guowangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mvw.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pxo.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://jbi.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://tbu.zhijiandao.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zfe.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ieo.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://ycz.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://tbs.tian-w.cn

[F09] 获取文件大小
来源：http://kbx.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://cah.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://qyd.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://ljq.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://mkf.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://aii.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wby.nanxinkj.top

Ruby: File.size("a.txt")
来源：http://bhk.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://rvj.shanyushiyangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://zft.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xta.zhijiandao.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aps.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lnk.yj202588.top

TS:   path.extname("a.txt")
来源：http://upu.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tab.tian-w.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rwz.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jcq.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dpr.ivvv.top

[F11] 复制与移动文件
来源：http://cnn.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mdp.gotoacloud.top


<!-- 参考信息 -->