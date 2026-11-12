代发 wailian999

[E02] 重复字符串
来源：http://scy.jianghu66.top

Py:   "ab" * 3
来源：http://xkk.nanxuanxn.top

PHP:  str_repeat("ab", 3);
来源：http://mvi.yj20258.top

JS:   "ab".repeat(3)
来源：http://ftn.fengsongda.top

TS:   "ab".repeat(3)
来源：http://bfd.vehdjk.com

Java: "ab".repeat(3)
来源：http://zic.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://cus.cqqwz.cn

Ruby: "ab" * 3
来源：http://jlo.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://prb.yj202588.top

[E03] 截取子串
来源：http://cwd.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nnl.shanyushiyangtech.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nss.jinqigufen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ykc.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://zhc.yj202588.top

Java: s.substring(1, 4)
来源：http://qbn.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hzh.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://xjv.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://pxh.daxiang520.top

[E04] 查找子串位置
来源：http://cyg.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://nyh.hnxiangtu.top

PHP:  strpos($s, "x");
来源：http://gyn.52xcode.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vkb.cqqwz.cn

TS:   s.indexOf("x")
来源：http://isw.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://pfe.epnwcf.com

Go:   strings.Index(s, "x")
来源：http://fme.hongshengwenyu.top

Ruby: s.index("x")
来源：http://jnu.wangdashe.top

C#:   s.IndexOf("x")
来源：http://qlj.yuanzhike.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tpm.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pwc.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uwb.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jig.mhx1999.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://thx.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uxo.316326.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://osj.svipenyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kiq.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nwt.yueranfly.top

[E06] 替换子串
来源：http://umw.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qsn.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://cxh.vqdsnc.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rxm.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://fsy.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ctd.cqqwz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kdf.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ooi.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://ach.uphjek.com

[E07] 按分隔符拆分
来源：http://hsf.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oau.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sll.hesvh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xqx.sjlbkw.cn

TS:   s.split(",")
来源：http://pag.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://vou.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ham.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://xsj.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oes.andypj.xyz

[E08] 数组按分隔符合并
来源：http://jnk.havefunace.top

Py:   ",".join(items)
来源：http://sco.hywenlv.cn

PHP:  implode(",", $items);
来源：http://mih.gzhubu.top

JS:   items.join(",")
来源：http://cwe.svipenyu.cn

TS:   items.join(",")
来源：http://hkg.chenzaomai.com

Java: String.join(",", items)
来源：http://xwz.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://dee.meibo888.top

Ruby: items.join(",")
来源：http://oqr.hysaishi.cn

C#:   string.Join(",", items)
来源：http://cto.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://voh.xuanzx.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sos.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pet.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://ulz.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://bxl.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://vfy.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gzt.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pjl.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wcy.zycfv.cn

[E10] 左侧补零 / 定长填充
来源：http://wlp.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://idm.iojbl.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ugu.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://prm.yueranfly.top

TS:   "7".padStart(3, "0")
来源：http://sck.sysykeji.top

Java: String.format("%03d", 7)
来源：http://nxt.aibaodan.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ifj.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nzr.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wyf.shanyushiyangkeji.top

[E11] 反转字符串
来源：http://ypr.yonumen.top

Py:   s[::-1]
来源：http://fyx.zdqjudy.top

PHP:  strrev($s);
来源：http://jbh.jinyuanbaomall.cn

JS:   [...s].reverse().join("")
来源：http://qry.0kj1m.cn

TS:   [...s].reverse().join("")
来源：http://mca.jyoumei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hnc.jinqigfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://acs.haohaochexian.top

Ruby: s.reverse
来源：http://wiu.xuetiantiany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://enz.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://zwd.zycfv.cn

Py:   s.count("a")
来源：http://tut.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://xgv.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://ixf.xinyue.icu

TS:   s.split("a").length - 1
来源：http://bhf.jinqigfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://exr.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://xyb.zdqjudy.top

Ruby: s.count("a")
来源：http://zbi.kuanghao11.cn

C#:   s.Count(c => c == 'a')
来源：http://rvh.yuanzhike.top

[E13] 逐字符遍历
来源：http://cvo.ybcxt.top

Py:   for ch in s: print(ch)
来源：http://fwk.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://leo.fzhhl.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hnx.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ino.zhaomingkeji.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vth.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vmb.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://aot.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cjk.ctjpmb.com

[E14] URL 编码与 Base64
来源：http://gkm.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ahv.hesvh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://map.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jcx.zhengqikj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lqy.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nhl.yanxiufei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fpj.pycfn.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dpo.yueranfly.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wnr.shzxlz.cn

[E15] HTML 转义 / 反转义
来源：http://bkm.yanxiufei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jhc.vqdsnc.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://azk.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uoo.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pdn.ctjpmb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tff.jinqigufen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vbf.aizwys.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jde.hfpthk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jmr.tanke756.top

[E16] 数字千分位
来源：http://cxo.xylfe.cn

Py:   f"{1234567:,}"
来源：http://ufx.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://ffr.zhiwuduotai.top

JS:   (1234567).toLocaleString("en-US")
来源：http://eck.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yew.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://afj.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gsd.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fnc.hnqzz.top

C#:   1234567.ToString("N0")
来源：http://dbe.ehwqpu.com

[E17] 首字母大写
来源：http://vcz.wangdashe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://geq.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tit.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vnl.guannengcc.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://avg.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jrg.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jqz.haohaochexian.top

Ruby: s.capitalize
来源：http://vij.52xcode.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ymn.snrcjt.cn

[E18] 模板占位符替换
来源：http://zrk.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ijf.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jds.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yzu.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fwn.shangyingyoupin.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dic.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://svi.uphjek.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uin.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cfx.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://gwj.shuidangran.top

Py:   s.splitlines()
来源：http://aek.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ari.c1oappe.top

JS:   s.split(/\r?\n/)
来源：http://wjh.hysaishi.cn

TS:   s.split(/\r?\n/)
来源：http://ezt.zhongyouzk.top

Java: s.lines().toList()
来源：http://mof.jqgfzy.top

Go:   strings.Split(s, "\n")
来源：http://jzx.xuetiantiany.cn

Ruby: s.lines
来源：http://tft.yuanzhike.top

C#:   s.Split('\n')
来源：http://pck.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://ave.hnxiangtu.top

Py:   if not s:
来源：http://eet.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cye.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qpn.ehwqpu.com

TS:   if (s === "") {}
来源：http://znc.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://tgx.zhixingplan.top

Go:   if s == "" {}
来源：http://uga.gotoacloud.top

Ruby: if s.empty?
来源：http://oxm.svipenyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iuh.cqqwz.cn

[E21] 超长截断加省略号
来源：http://wyq.vqdsnc.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lsl.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ook.jyoumei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://klu.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bsc.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nyt.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://klq.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dki.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nfa.sjlbkw.cn

[E22] 字节长度与字符长度
来源：http://vid.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xts.gaohongyu789.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://flb.tianlin.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qdx.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wsb.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://crx.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ucp.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://wzh.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ltf.sufxvd.cn

================================================================================
来源：http://mlg.wangshuangyany.cn

F. 文件与目录
来源：http://pxk.kuanghao11.cn

================================================================================
来源：http://nlq.yonumen.top

[F01] 读取整个文件
来源：http://vmz.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wuf.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://jup.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rdu.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://apt.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oym.hnxiangtu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xbg.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://zkv.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://qfv.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://vkd.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tjr.52xcode.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ple.yvedp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qbm.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jxz.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rnq.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tvr.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nfk.feifeiyinyue.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hok.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://mjf.fengsongda.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mok.guannengcc.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nrz.jinyuanbaomall.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rup.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mad.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ojw.shuidangran.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iis.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://kxu.hammf.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hao.yfazqb.com

[F04] 追加写入文件
来源：http://nbh.shzxlz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zrx.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fry.epnwcf.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ejl.hesvh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ymi.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jfn.wangshuangyany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zfm.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://spz.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xij.smart0.xyz

[F05] 判断文件或目录是否存在
来源：http://uwc.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://trp.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://qsf.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://wjc.zhiwuduotai.top

TS:   fs.existsSync("a.txt")
来源：http://kpe.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cow.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hst.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://ppt.shangyingyoupin.top

C#:   File.Exists("a.txt")
来源：http://why.fktsv.cn

[F06] 删除文件
来源：http://vkn.yonumen.top

Py:   os.remove("a.txt")
来源：http://dup.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://clb.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://ppy.zhaomingkeji.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://bvh.pycfn.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kdm.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://mnu.zhaomingkeji.xyz

Ruby: File.delete("a.txt")
来源：http://kay.sweek.top

C#:   File.Delete("a.txt");
来源：http://zje.ivvv.top

[F07] 创建目录（含多级）
来源：http://ifb.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mgv.gzhubu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tpo.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jua.gogol.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ctk.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kpk.shanyushiyangtech.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bty.andypj.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pnu.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ubh.ywan-chungtsiang.top

[F08] 遍历目录
来源：http://wsp.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vio.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yle.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://kil.jinqigfzy.top

TS:   fs.readdirSync("dir")
来源：http://ssn.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fmk.xziqi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vmw.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://kiz.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://rsr.ppjwa.cn

[F09] 获取文件大小
来源：http://unb.fktsv.cn

Py:   os.path.getsize("a.txt")
来源：http://vqo.nanxinkj.top

PHP:  filesize("a.txt");
来源：http://ckg.cdnleiting.top

JS:   fs.statSync("a.txt").size
来源：http://xiq.svipenyu.cn

TS:   fs.statSync("a.txt").size
来源：http://tpd.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://wog.yonumen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aug.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://ism.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://leo.yuanzhike.top

[F10] 取文件扩展名 / 文件名
来源：http://ogo.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rcg.ctjpmb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sit.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wzg.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://hue.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ptn.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://adm.yanxiufei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://giq.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://csx.kuanghao11.cn

[F11] 复制与移动文件
来源：http://bca.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aef.snrcjt.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rbj.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wuc.chenlongwang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lcj.tarul.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qcd.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hkd.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fib.xuanzx.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sdu.c1oappe.top

[F12] CSV 读写
来源：http://ijo.shzxlz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dzl.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xko.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vjs.sysykeji.top

TS:   // 同上
来源：http://zsx.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lpz.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ynp.meibo888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wtw.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://apg.wangshuangyany.cn


<!-- 参考信息 -->