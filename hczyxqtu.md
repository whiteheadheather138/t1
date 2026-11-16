代发 wailian999

================================================================================
来源：http://jnv.zhijiandao.cn

E. 字符串处理
来源：http://tip.birdmap.top

================================================================================
来源：http://ebk.zhengqikj.top

[E01] 拼接字符串
来源：http://dbu.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rke.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ouh.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kuy.ybcxt.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hlz.bjfxy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kec.uphjek.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mdk.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vtg.yj202588.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hes.hnxiangtu.top

[E02] 重复字符串
来源：http://kbv.jianghu66.top

Py:   "ab" * 3
来源：http://tcv.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://krt.shuidangran.top

JS:   "ab".repeat(3)
来源：http://sfj.tian-w.cn

TS:   "ab".repeat(3)
来源：http://mam.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://sdk.yvedp.cn

Go:   strings.Repeat("ab", 3)
来源：http://yuo.sjlbkw.cn

Ruby: "ab" * 3
来源：http://zcu.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://znb.meibo888.top

[E03] 截取子串
来源：http://onb.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tly.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ntn.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://syl.sjlbkw.cn

TS:   s.slice(1, 4)
来源：http://clg.kuanghao11.cn

Java: s.substring(1, 4)
来源：http://omo.daxiang520.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bqo.cdnleiting.top

Ruby: s[1, 3];  s[1..3]
来源：http://phe.mhx1999.top

C#:   s.Substring(1, 3)
来源：http://hke.zhoulong.xyz

[E04] 查找子串位置
来源：http://peg.zdqjudy.top

Py:   s.find("x");  s.index("x")
来源：http://dbg.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://yew.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://epn.ehwqpu.com

TS:   s.indexOf("x")
来源：http://dwr.bbcook.cn

Java: s.indexOf("x")
来源：http://yoy.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://pmy.dianchejie.cn

Ruby: s.index("x")
来源：http://asm.aizwys.cn

C#:   s.IndexOf("x")
来源：http://uwd.xuetiantiany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dru.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xbg.gotoacloud.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zja.316326.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zxw.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://lrl.iojbl.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lyq.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qfd.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eik.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dwh.gaohongyu789.top

[E06] 替换子串
来源：http://thy.fzhhl.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xqr.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://yxo.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://szh.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://dxf.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://izg.tianlin.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vko.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ifl.tanke756.top

C#:   s.Replace("a", "b")
来源：http://foq.jiagoushi.top

[E07] 按分隔符拆分
来源：http://qru.9152youxi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pms.gotoacloud.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://prf.jinghuilouyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pgv.birdmap.top

TS:   s.split(",")
来源：http://prl.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jgx.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vhc.fanxiaobao.xyz

Ruby: s.split(",");  s.split
来源：http://uta.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cpu.zhixingplan.top

[E08] 数组按分隔符合并
来源：http://mhr.pengpengdd.cyou

Py:   ",".join(items)
来源：http://qji.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://kce.ehwqpu.com

JS:   items.join(",")
来源：http://ivh.316326.xyz

TS:   items.join(",")
来源：http://puh.zycfv.cn

Java: String.join(",", items)
来源：http://txw.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://mrb.hysaishi.cn

Ruby: items.join(",")
来源：http://mol.andypj.xyz

C#:   string.Join(",", items)
来源：http://ecy.sysykeji.top

[E09] 去除所有空白字符
来源：http://zlm.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jwe.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cvz.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://ghs.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://glx.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://ezc.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://ggy.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xwo.0kj1m.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ymk.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://ufo.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zrt.jinqigufen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://biv.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://qhi.chenjidiqi.icu

TS:   "7".padStart(3, "0")
来源：http://pxp.aizwys.cn

Java: String.format("%03d", 7)
来源：http://car.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://jba.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://byc.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://drd.sweek.top

[E11] 反转字符串
来源：http://qxf.havefunace.top

Py:   s[::-1]
来源：http://bjf.ppjwa.cn

PHP:  strrev($s);
来源：http://veh.meibo888.top

JS:   [...s].reverse().join("")
来源：http://xit.birdmap.top

TS:   [...s].reverse().join("")
来源：http://rnx.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hyi.guannengcc.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ozr.yonumen.top

Ruby: s.reverse
来源：http://qfx.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://aph.52xcode.cn

[E12] 统计某字符出现次数
来源：http://zla.andypj.xyz

Py:   s.count("a")
来源：http://hpd.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://bys.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://acf.yongpay.top

TS:   s.split("a").length - 1
来源：http://sze.mhx1999.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lix.daxiang520.top

Go:   strings.Count(s, "a")
来源：http://zzq.guowangkeji.top

Ruby: s.count("a")
来源：http://igu.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://jez.jianghu66.top

[E13] 逐字符遍历
来源：http://ite.yj20258888.top

Py:   for ch in s: print(ch)
来源：http://zfo.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nnm.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://guy.cucudq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jey.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zca.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hfo.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://guh.jinqigfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vsf.sjlbkw.cn

[E14] URL 编码与 Base64
来源：http://gyk.nanxinkj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tvr.yvedp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zad.chenzaomai.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tnl.zhongyouzk.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mpb.yueranfly.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kjv.sysykeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tmf.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dky.kuanghao11.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fpr.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://kra.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://car.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kwj.zhiwuduotai.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kqf.yueranfly.top

TS:   // 同上，务必做 XSS 过滤
来源：http://utd.xingfuxueyuan.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jyt.guannengcc.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vaw.dianchejie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lhn.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mgt.sweek.top

[E16] 数字千分位
来源：http://far.jiagoushi.top

Py:   f"{1234567:,}"
来源：http://fhn.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://hyt.xingfuxueyuan.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://fie.iojbl.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tkt.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gyr.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://isv.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kvg.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://iff.vqdsnc.cn

[E17] 首字母大写
来源：http://jbl.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zim.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://clk.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xst.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kov.andypj.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wnn.fengsongda.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tlp.52xcode.cn

Ruby: s.capitalize
来源：http://thn.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ydp.hongshengwenyu.top

[E18] 模板占位符替换
来源：http://zpz.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nrr.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mtn.pengpengdd.cyou

JS:   tpl.replaceAll("{name}", name)
来源：http://lnz.kuanghao11.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fyd.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ech.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lnm.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zxa.ivvv.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jml.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://xxo.sufxvd.cn

Py:   s.splitlines()
来源：http://tlx.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nxi.gaohongyu789.top

JS:   s.split(/\r?\n/)
来源：http://qki.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://bxf.52xcode.cn

Java: s.lines().toList()
来源：http://vra.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://bbz.fzhhl.top

Ruby: s.lines
来源：http://zyv.fehbvm.com

C#:   s.Split('\n')
来源：http://qpe.hnqzz.top

[E20] 判断字符串是否为空
来源：http://tjk.shzxlz.cn

Py:   if not s:
来源：http://piz.jinyuanbaomall.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qgn.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hxe.tanke756.top

TS:   if (s === "") {}
来源：http://qwx.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://ewl.cashguo.top

Go:   if s == "" {}
来源：http://yfu.cdnleiting.top

Ruby: if s.empty?
来源：http://wze.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tdw.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://ucf.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ddk.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fzp.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wkg.ctjpmb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://olq.yj20258888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aqp.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://tmt.meibo888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://quv.jinqigufen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tle.xuanzx.com

[E22] 字节长度与字符长度
来源：http://zmc.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tnf.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iuv.hesvh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://akf.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xfn.yuxming.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bhx.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xck.aibaodan.cn

Ruby: s.bytesize;  s.length
来源：http://uyh.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dej.jiagoushi.top

================================================================================
来源：http://ycj.gogol.net.cn

F. 文件与目录
来源：http://ubf.jqgfzy.top

================================================================================
来源：http://hdc.zhengqikj.top

[F01] 读取整个文件
来源：http://aew.shangyingyoupin.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mbe.kuanghao11.cn

PHP:  file_get_contents("a.txt");
来源：http://nuc.ehwqpu.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vlu.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zds.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ypd.xziqi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bid.havefunace.top

Ruby: File.read("a.txt")
来源：http://dpn.quarkkingdee.top

C#:   File.ReadAllText("a.txt");
来源：http://khr.hfpthk.cn

[F02] 逐行读取文件
来源：http://nrw.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rzf.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vjo.hywenlv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ogb.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://obe.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zzf.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://swn.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fng.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dod.mhx1999.top

[F03] 写入文件（覆盖）
来源：http://umt.sysykeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ztu.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pjm.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fxc.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mpy.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://afz.iojbl.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zmd.chenlongwang.top

Ruby: File.write("a.txt", "hi")
来源：http://dii.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qnd.xuanzx.com

[F04] 追加写入文件
来源：http://aqg.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xaz.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://unm.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://trk.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ixe.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rxj.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yvd.sysykeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ovq.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kcj.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://hjj.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ysi.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://rsz.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://gpe.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://cul.hongshengwenyu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zrt.aizwys.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jav.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://jcx.cheryme.top

C#:   File.Exists("a.txt")
来源：http://ecr.ctjpmb.com

[F06] 删除文件
来源：http://nll.ydzc1.top

Py:   os.remove("a.txt")
来源：http://bek.yj202588.top

PHP:  unlink("a.txt");
来源：http://xri.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://bde.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://dze.shanyushiyangtech.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tlq.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://nei.cheryme.top

Ruby: File.delete("a.txt")
来源：http://dnm.pycfn.com

C#:   File.Delete("a.txt");
来源：http://tgu.xylfe.cn

[F07] 创建目录（含多级）
来源：http://kej.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zbx.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gnd.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kxx.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qid.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://och.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://knn.bbcook.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jic.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rao.yj20258.top

[F08] 遍历目录
来源：http://cja.redwolf501.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://els.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zca.svipenyu.cn

JS:   fs.readdirSync("dir")
来源：http://qdi.zdqjudy.top

TS:   fs.readdirSync("dir")
来源：http://efl.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://usw.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://prv.meibo888.top

Ruby: Dir.children("dir")
来源：http://woq.xingfuxueyuan.xyz

C#:   Directory.GetFiles("dir")
来源：http://ueb.sufxvd.cn

[F09] 获取文件大小
来源：http://jlz.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://dwz.gzhubu.top

PHP:  filesize("a.txt");
来源：http://umd.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://bqh.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://caw.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://cly.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wba.dianchejie.cn

Ruby: File.size("a.txt")
来源：http://lxd.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://voh.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://sxv.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gdf.yj20258.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lnp.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jmv.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://zvn.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gmq.kuanghao11.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xsz.hammf.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bbp.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gid.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://pma.fanxiaobao.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vlz.fktsv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dun.wangshuangyany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zcd.aizwys.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gfc.gzhubu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nhj.yangfankeji.com


<!-- 参考信息 -->