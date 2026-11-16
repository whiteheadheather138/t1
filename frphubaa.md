代发 wailian999

Java: String.join(", ", list)
来源：http://bsa.zhengqikj.top

Go:   strings.Join(strs, ", ")
来源：http://vcz.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://fug.guannengcc.top

C#:   string.Join(", ", list)
来源：http://zxb.jqgufenzy.top

================================================================================
来源：http://lyq.yj20258.top

E. 字符串处理
来源：http://hwv.zhixingplan.top

================================================================================
来源：http://gso.fengsongda.top

[E01] 拼接字符串
来源：http://rjh.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vxv.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xaa.hesvh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://omw.snrcjt.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iad.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vxl.zhixingplan.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://azc.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tvl.pycfn.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jpw.ydzc1.top

[E02] 重复字符串
来源：http://xiq.cqqwz.cn

Py:   "ab" * 3
来源：http://ncl.svipenyu.cn

PHP:  str_repeat("ab", 3);
来源：http://rfh.iojbl.cn

JS:   "ab".repeat(3)
来源：http://ofe.kuanghao11.cn

TS:   "ab".repeat(3)
来源：http://gay.xylfe.cn

Java: "ab".repeat(3)
来源：http://ain.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://cod.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://kqw.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ztb.yuanzhike.top

[E03] 截取子串
来源：http://tqj.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eim.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pbw.yonumen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ruu.xuanzx.com

TS:   s.slice(1, 4)
来源：http://rsf.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://feu.sysykeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pgz.fehbvm.com

Ruby: s[1, 3];  s[1..3]
来源：http://vwr.sweek.top

C#:   s.Substring(1, 3)
来源：http://ggw.jlsjyb.cn

[E04] 查找子串位置
来源：http://zqr.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://pti.yj20258888.top

PHP:  strpos($s, "x");
来源：http://cpy.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xlo.dianchejie.cn

TS:   s.indexOf("x")
来源：http://wpq.zhiwuduotai.top

Java: s.indexOf("x")
来源：http://fwz.cheryme.top

Go:   strings.Index(s, "x")
来源：http://bsq.chenjidiqi.icu

Ruby: s.index("x")
来源：http://xtn.hnxiangtu.top

C#:   s.IndexOf("x")
来源：http://ecr.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tho.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://isp.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bnu.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jrp.zhengqikj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jpc.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uzv.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fli.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dxy.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rkp.wangdashe.top

[E06] 替换子串
来源：http://dbj.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xai.chenjidiqi.icu

PHP:  str_replace("a", "b", $s);
来源：http://vbf.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mjk.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://rwn.fktsv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rbv.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mcw.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wfp.iojbl.cn

C#:   s.Replace("a", "b")
来源：http://mur.ydzc1.top

[E07] 按分隔符拆分
来源：http://bcf.aibaodan.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://odo.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fmn.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ebh.jinqigufen.top

TS:   s.split(",")
来源：http://mdk.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://epd.sweek.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rhj.shanyushiyangtech.top

Ruby: s.split(",");  s.split
来源：http://uly.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vpn.9152youxi.cn

[E08] 数组按分隔符合并
来源：http://gga.smart0.xyz

Py:   ",".join(items)
来源：http://bgo.yongpay.top

PHP:  implode(",", $items);
来源：http://avd.wangshuangyany.cn

JS:   items.join(",")
来源：http://igs.yvedp.cn

TS:   items.join(",")
来源：http://jmi.yangfankeji.com

Java: String.join(",", items)
来源：http://kxx.bjfxy.top

Go:   strings.Join(items, ",")
来源：http://jtc.ctjpmb.com

Ruby: items.join(",")
来源：http://lcv.jiagoushi.top

C#:   string.Join(",", items)
来源：http://jye.cqqwz.cn

[E09] 去除所有空白字符
来源：http://jud.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tvh.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zwx.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://lft.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://spy.fktsv.cn

Java: s.replaceAll("\\s+", "")
来源：http://akj.dashuyun.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qhv.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://qif.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ngw.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://fgt.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zle.cucudq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://meu.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://qdy.guowangkeji.top

TS:   "7".padStart(3, "0")
来源：http://wuj.iojbl.cn

Java: String.format("%03d", 7)
来源：http://xqc.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://rac.wangshuangyany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://icl.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ejk.chenjidiqi.icu

[E11] 反转字符串
来源：http://kri.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://kpv.nanxuanxn.top

PHP:  strrev($s);
来源：http://xwd.cashguo.top

JS:   [...s].reverse().join("")
来源：http://omq.yongpay.top

TS:   [...s].reverse().join("")
来源：http://row.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ngo.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://jvo.0kj1m.cn

Ruby: s.reverse
来源：http://lhh.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wkk.cheryme.top

[E12] 统计某字符出现次数
来源：http://jib.nanxinkj.top

Py:   s.count("a")
来源：http://xhy.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://xsj.jinghuilouyu.cn

JS:   s.split("a").length - 1
来源：http://sxr.gzhubu.top

TS:   s.split("a").length - 1
来源：http://iao.yvedp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rlz.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://tcs.hcnkem.com

Ruby: s.count("a")
来源：http://qxg.hfpthk.cn

C#:   s.Count(c => c == 'a')
来源：http://fvd.jyoumei.cn

[E13] 逐字符遍历
来源：http://atb.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://wmg.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hsh.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jwp.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://zqi.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kpd.ivvv.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://puj.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://rsv.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://klr.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://hii.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yua.dianchejie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qub.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ftq.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jrm.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://prs.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jvu.jqgufenzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vjw.sjlbkw.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tgs.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://zmo.havefunace.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ldm.cucudq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ymc.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qrj.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xkd.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mvp.jinghuilouyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://puj.zhijiandao.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://scv.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://svn.hnqzz.top

[E16] 数字千分位
来源：http://vgj.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://qbj.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://qjf.xuetiantiany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yjk.fanxiaobao.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://pyn.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rct.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yan.aizwys.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ekp.shzxlz.cn

C#:   1234567.ToString("N0")
来源：http://yfz.52xcode.cn

[E17] 首字母大写
来源：http://edk.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://muq.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://evi.gzhubu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zry.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://waz.hnqzz.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fqd.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aip.tianlin.xyz

Ruby: s.capitalize
来源：http://jwv.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fdj.sjlbkw.cn

[E18] 模板占位符替换
来源：http://nrb.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jmk.epnwcf.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ivw.tian-w.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nim.ywan-chungtsiang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dtm.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ykc.fanxiaobao.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yfl.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yon.ydjk.org.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ulx.ydjk.org.cn

[E19] 多行文本按行拆分
来源：http://ttl.tanke756.top

Py:   s.splitlines()
来源：http://tha.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iez.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://bqj.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://hfv.vqdsnc.cn

Java: s.lines().toList()
来源：http://cbz.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://rzf.gogol.net.cn

Ruby: s.lines
来源：http://sjm.jiagoushi.top

C#:   s.Split('\n')
来源：http://tck.fktsv.cn

[E20] 判断字符串是否为空
来源：http://xtc.yuanzhike.top

Py:   if not s:
来源：http://mpo.hnqzz.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vtd.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zdv.hesvh.cn

TS:   if (s === "") {}
来源：http://cxp.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://rae.haohaochexian.top

Go:   if s == "" {}
来源：http://sqq.iojbl.cn

Ruby: if s.empty?
来源：http://qyk.tian-w.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ymu.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://iyt.yj202588.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tge.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wxi.uphjek.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ilw.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ujf.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zys.meibo888.top

Go:   // 按 rune 判断长度后截断
来源：http://mks.hysaishi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ejc.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://api.zycfv.cn

[E22] 字节长度与字符长度
来源：http://qgt.epnwcf.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gzm.xuanzx.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dwp.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qry.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dmz.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://obl.ywan-chungtsiang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://imr.yj20258888.top

Ruby: s.bytesize;  s.length
来源：http://fjv.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fnq.0kj1m.cn

================================================================================
来源：http://uyy.jlsjyb.cn

F. 文件与目录
来源：http://ubd.kuanghao11.cn

================================================================================
来源：http://bhx.nwbrower.top

[F01] 读取整个文件
来源：http://ult.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ioh.svipenyu.cn

PHP:  file_get_contents("a.txt");
来源：http://lxv.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hat.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fqx.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://xwg.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hyo.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://tpi.hongshengwenyu.top

C#:   File.ReadAllText("a.txt");
来源：http://dcf.xylfe.cn

[F02] 逐行读取文件
来源：http://kkw.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lel.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ign.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lmg.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://arp.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jwt.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yoc.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kez.yj20258888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qtn.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://kgx.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zcl.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://myw.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zcd.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kni.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://boq.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bbu.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://xbi.chenlongwang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iwp.yanxiufei.cn

[F04] 追加写入文件
来源：http://ple.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pig.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lzo.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://imo.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dxd.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ikv.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ipb.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vfc.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zmv.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://hqw.yangfankeji.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gyl.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://pbx.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://kgc.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://vbz.shanyushiyangtech.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lpr.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dnx.xingfuxueyuan.xyz

Ruby: File.exist?("a.txt")
来源：http://qfy.daxiang520.top

C#:   File.Exists("a.txt")
来源：http://ibn.yj20258888.top

[F06] 删除文件
来源：http://xiy.kuanghao11.cn

Py:   os.remove("a.txt")
来源：http://iak.wangdashe.top

PHP:  unlink("a.txt");
来源：http://xdw.xuetiantiany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hbf.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://swt.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bcs.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://cnk.xuanzx.com

Ruby: File.delete("a.txt")
来源：http://lwm.hnqzz.top

C#:   File.Delete("a.txt");
来源：http://nll.tanke756.top

[F07] 创建目录（含多级）
来源：http://ypg.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zfc.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gtx.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vdj.zhixingplan.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nax.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ktx.yuxming.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://moo.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tsq.0kj1m.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://msf.jiagoushi.top

[F08] 遍历目录
来源：http://mku.ctjpmb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://vth.sxryk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aaz.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://cvu.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://boo.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vuw.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nsl.hammf.cn

Ruby: Dir.children("dir")
来源：http://fzi.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://rea.nanxinkj.top

[F09] 获取文件大小
来源：http://yav.fktsv.cn

Py:   os.path.getsize("a.txt")
来源：http://mvp.tarul.cn

PHP:  filesize("a.txt");
来源：http://gzm.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://bqa.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://cle.jinghuilouyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://luq.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lta.cashguo.top

Ruby: File.size("a.txt")
来源：http://wiw.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://htj.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://ueq.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ttn.jianghu66.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pwn.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rmo.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://mpg.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kjm.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cxw.tian-w.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://srg.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rqf.yonumen.top

[F11] 复制与移动文件
来源：http://wxl.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qpa.xinyue.icu


<!-- 参考信息 -->