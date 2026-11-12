代发 wailian999

TS:   "ab".repeat(3)
来源：http://eei.tanke756.top

Java: "ab".repeat(3)
来源：http://qnh.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://ymn.dianchejie.cn

Ruby: "ab" * 3
来源：http://gso.shanyushiyangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lna.nanxuanxn.top

[E03] 截取子串
来源：http://ytm.hnqzz.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hwj.vqdsnc.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dmf.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nwo.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://eet.bjfxy.top

Java: s.substring(1, 4)
来源：http://ozj.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kpi.mhx1999.top

Ruby: s[1, 3];  s[1..3]
来源：http://tmi.nwbrower.top

C#:   s.Substring(1, 3)
来源：http://gfj.zdbjq.cn

[E04] 查找子串位置
来源：http://ixx.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://lsn.jiagoushi.top

PHP:  strpos($s, "x");
来源：http://xyr.cheryme.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pvy.gotoacloud.top

TS:   s.indexOf("x")
来源：http://pfp.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://dwx.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://hya.yueranfly.top

Ruby: s.index("x")
来源：http://svg.316326.xyz

C#:   s.IndexOf("x")
来源：http://kwa.hywenlv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bnt.zhaomingkeji.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cuq.gotoacloud.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dtf.xylfe.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hgn.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hwk.svipenyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sec.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aed.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zsu.zhengqikj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://chl.cqqwz.cn

[E06] 替换子串
来源：http://lco.zycfv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xte.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://jds.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://suy.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://bdh.fktsv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://old.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tmf.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ccy.hammf.cn

C#:   s.Replace("a", "b")
来源：http://wrc.sweek.top

[E07] 按分隔符拆分
来源：http://zso.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ygp.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://adj.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jfw.jqgufenzy.top

TS:   s.split(",")
来源：http://uvd.xylfe.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tqd.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ykz.tarul.cn

Ruby: s.split(",");  s.split
来源：http://yyy.fehbvm.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nbt.sufxvd.cn

[E08] 数组按分隔符合并
来源：http://nqq.fengsongda.top

Py:   ",".join(items)
来源：http://svl.tarul.cn

PHP:  implode(",", $items);
来源：http://yha.wangdashe.top

JS:   items.join(",")
来源：http://ekm.cucudq.cn

TS:   items.join(",")
来源：http://lop.xingfuxueyuan.xyz

Java: String.join(",", items)
来源：http://tek.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://qpj.epnwcf.com

Ruby: items.join(",")
来源：http://zwj.zhengqikj.top

C#:   string.Join(",", items)
来源：http://eth.shanyushiyangtech.top

[E09] 去除所有空白字符
来源：http://biw.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://enr.xziqi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://euq.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://czs.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://scu.mhx1999.top

Java: s.replaceAll("\\s+", "")
来源：http://qsr.yangfankeji.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://boc.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mqw.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://klu.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://bfa.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dfc.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dqq.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://zwh.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://zbh.yvedp.cn

Java: String.format("%03d", 7)
来源：http://omy.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lli.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zcn.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tbj.zhoulong.xyz

[E11] 反转字符串
来源：http://exj.daxiang520.top

Py:   s[::-1]
来源：http://pcx.pycfn.com

PHP:  strrev($s);
来源：http://ugr.vehdjk.com

JS:   [...s].reverse().join("")
来源：http://dzw.daxiang520.top

TS:   [...s].reverse().join("")
来源：http://bis.jiagoushi.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lwt.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pfq.yfazqb.com

Ruby: s.reverse
来源：http://sbl.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://zge.jqgfzy.top

[E12] 统计某字符出现次数
来源：http://miq.wangdashe.top

Py:   s.count("a")
来源：http://vfq.gotoacloud.top

PHP:  substr_count($s, "a");
来源：http://hoh.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://rnd.xuetiantiany.cn

TS:   s.split("a").length - 1
来源：http://ibw.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tkh.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://xli.guowangkeji.top

Ruby: s.count("a")
来源：http://hov.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://tyl.zhoulong.xyz

[E13] 逐字符遍历
来源：http://erv.cashguo.top

Py:   for ch in s: print(ch)
来源：http://oka.jinghuilouyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wlj.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://org.guannengcc.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rye.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eua.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://icc.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gaz.hnxiangtu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ido.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://nvy.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://urb.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://kwf.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uhh.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zzt.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fvn.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aad.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://puk.tian-w.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hnr.zycfv.cn

[E15] HTML 转义 / 反转义
来源：http://haw.jinqigufen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sag.gotoacloud.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qgw.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wld.vehdjk.com

TS:   // 同上，务必做 XSS 过滤
来源：http://kpf.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://glu.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dro.redwolf501.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vxd.haohaochexian.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dtw.ybcxt.top

[E16] 数字千分位
来源：http://ndf.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://xzr.tanke756.top

PHP:  number_format(1234567);
来源：http://uec.52xcode.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hht.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://vse.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hyy.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xuf.xylfe.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fld.tarul.cn

C#:   1234567.ToString("N0")
来源：http://nwk.gzhubu.top

[E17] 首字母大写
来源：http://ipb.yvedp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ecu.andypj.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://jfr.hammf.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hlk.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hew.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://umc.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nwu.tanke756.top

Ruby: s.capitalize
来源：http://sbj.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wem.zycfv.cn

[E18] 模板占位符替换
来源：http://ail.0kj1m.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qsg.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ybk.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fte.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://khw.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fnd.yongpay.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lvc.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ipk.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zws.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://qrt.haohaochexian.top

Py:   s.splitlines()
来源：http://isz.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ugr.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://gkl.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://lnh.svipenyu.cn

Java: s.lines().toList()
来源：http://oex.fzhhl.top

Go:   strings.Split(s, "\n")
来源：http://vfx.zycfv.cn

Ruby: s.lines
来源：http://djv.quarkkingdee.top

C#:   s.Split('\n')
来源：http://xjz.xinyue.icu

[E20] 判断字符串是否为空
来源：http://grc.yueranfly.top

Py:   if not s:
来源：http://gtc.jqgfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cwh.52xcode.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jle.zhaomingkeji.xyz

TS:   if (s === "") {}
来源：http://iai.fanxiaobao.xyz

Java: if (s.isEmpty()) {}
来源：http://sbh.jiagoushi.top

Go:   if s == "" {}
来源：http://flf.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://ggw.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wrg.yfazqb.com

[E21] 超长截断加省略号
来源：http://dik.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zmy.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kjo.jqgfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xou.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iqr.tanke756.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rmg.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://fsm.yvedp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kug.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jmu.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://sde.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://luf.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://twe.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zan.yfazqb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qoe.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rwd.gotoacloud.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lmr.uphjek.com

Ruby: s.bytesize;  s.length
来源：http://sfd.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bfz.yj20258.top

================================================================================
来源：http://pqu.jiagoushi.top

F. 文件与目录
来源：http://tzr.hesvh.cn

================================================================================
来源：http://mvj.52xcode.cn

[F01] 读取整个文件
来源：http://uxo.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sqp.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://cwa.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ymk.shuidangran.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://utb.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://qwu.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bya.tian-w.cn

Ruby: File.read("a.txt")
来源：http://cbs.svipenyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://dgp.jiagoushi.top

[F02] 逐行读取文件
来源：http://wew.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cvw.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aic.aizwys.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://brl.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tqb.zhengqikj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rku.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://edc.vehdjk.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://twq.cucudq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xfw.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://rdy.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dde.yuxming.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jga.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://adh.yj20258.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://arw.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cxb.hongshengwenyu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zpt.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://zls.havefunace.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oxf.ydjk.org.cn

[F04] 追加写入文件
来源：http://gjo.ywan-chungtsiang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jxy.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yjk.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tme.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jhx.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://byu.zdqjudy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xmf.shangyingyoupin.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://izk.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hyd.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://qxz.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gym.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://xdn.0kj1m.cn

JS:   fs.existsSync("a.txt")
来源：http://ogi.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://dri.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://sdx.cheryme.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://koc.quarkkingdee.top

Ruby: File.exist?("a.txt")
来源：http://irn.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://cam.sjlbkw.cn

[F06] 删除文件
来源：http://iuo.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://csn.sweek.top

PHP:  unlink("a.txt");
来源：http://kph.jlsjyb.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ogn.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://uqb.hammf.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://njx.jinqigufen.top

Go:   os.Remove("a.txt")
来源：http://qtw.cheryme.top

Ruby: File.delete("a.txt")
来源：http://puk.ivvv.top

C#:   File.Delete("a.txt");
来源：http://bdz.zhaomingkeji.xyz

[F07] 创建目录（含多级）
来源：http://emd.tianlin.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bsn.xylfe.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uof.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://spz.ywan-chungtsiang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ltt.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rhh.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uzr.chenzaomai.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mgl.xziqi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vpn.nwbrower.top

[F08] 遍历目录
来源：http://qfm.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ebl.havefunace.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://umo.zhoulong.xyz

JS:   fs.readdirSync("dir")
来源：http://oeh.jinyuanbaomall.cn

TS:   fs.readdirSync("dir")
来源：http://ddn.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xzb.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bnu.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://brw.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://qxl.jinqigfzy.top

[F09] 获取文件大小
来源：http://mnm.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://wot.yuxming.cn

PHP:  filesize("a.txt");
来源：http://tow.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://lur.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://wkq.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ftg.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rqo.shangyingyoupin.top

Ruby: File.size("a.txt")
来源：http://pyw.quarkkingdee.top

C#:   new FileInfo("a.txt").Length
来源：http://fgz.yangfankeji.com

[F10] 取文件扩展名 / 文件名
来源：http://ldd.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hic.ctjpmb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qeu.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mez.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://syn.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iub.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bvs.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yju.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vlc.52xcode.cn

[F11] 复制与移动文件
来源：http://kqm.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wtj.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bfo.cheryme.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://arh.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uln.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dbl.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ouu.meibo888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aux.shuidangran.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xvl.havefunace.top

[F12] CSV 读写
来源：http://hjf.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cxh.xingfuxueyuan.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qtn.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wde.zdqjudy.top

TS:   // 同上
来源：http://irc.meibo888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hba.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hoj.kuanghao11.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://evf.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ici.shanyushiyangkeji.top

================================================================================
来源：http://mmn.jqgfzy.top

G. 面向对象
来源：http://mkv.yonumen.top

================================================================================
来源：http://ice.jinqigufen.top

[G01] 定义类
来源：http://nbt.52xcode.cn


<!-- 参考信息 -->