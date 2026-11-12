代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ind.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ped.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kls.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qno.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vtw.pycfn.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nwc.yueranfly.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rvn.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xnm.havefunace.top

[E02] 重复字符串
来源：http://ivy.zdbjq.cn

Py:   "ab" * 3
来源：http://wjf.ivvv.top

PHP:  str_repeat("ab", 3);
来源：http://nmf.daxiang520.top

JS:   "ab".repeat(3)
来源：http://kcm.shuidangran.top

TS:   "ab".repeat(3)
来源：http://oez.redwolf501.top

Java: "ab".repeat(3)
来源：http://geo.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://ehq.ydzc1.top

Ruby: "ab" * 3
来源：http://mza.quarkkingdee.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ilg.gaohongyu789.top

[E03] 截取子串
来源：http://cpz.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bpy.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vez.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dam.ybcxt.top

TS:   s.slice(1, 4)
来源：http://kdz.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://gmj.jinyuanbaomall.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nyr.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://gfm.yanxiufei.cn

C#:   s.Substring(1, 3)
来源：http://zyn.xylfe.cn

[E04] 查找子串位置
来源：http://cyn.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://hlb.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://zrl.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kfg.shanyushiyangtech.top

TS:   s.indexOf("x")
来源：http://tcp.yangfankeji.com

Java: s.indexOf("x")
来源：http://nie.zhaomingkeji.xyz

Go:   strings.Index(s, "x")
来源：http://ncd.daria6918.cn

Ruby: s.index("x")
来源：http://kyk.redwolf501.top

C#:   s.IndexOf("x")
来源：http://bvn.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pkd.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ejk.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aet.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kfs.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hty.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://unx.hfpthk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wui.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lvy.gzhubu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wys.ywan-chungtsiang.top

[E06] 替换子串
来源：http://xzc.jqgufenzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://diu.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://jla.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iec.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://xzm.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cqy.hfpthk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qdg.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://heu.chenlongwang.top

C#:   s.Replace("a", "b")
来源：http://qgf.cashguo.top

[E07] 按分隔符拆分
来源：http://jih.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://biz.kuanghao11.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hwp.yangfankeji.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ohz.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://wqt.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oqw.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hdt.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://qcy.iojbl.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://shy.xziqi.cn

[E08] 数组按分隔符合并
来源：http://nus.yj20258888.top

Py:   ",".join(items)
来源：http://vkv.shzxlz.cn

PHP:  implode(",", $items);
来源：http://ozx.ehwqpu.com

JS:   items.join(",")
来源：http://qbx.xziqi.cn

TS:   items.join(",")
来源：http://ydb.cheryme.top

Java: String.join(",", items)
来源：http://gai.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://wsz.jiagoushi.top

Ruby: items.join(",")
来源：http://kmn.yangfankeji.com

C#:   string.Join(",", items)
来源：http://hux.zhaomingkeji.xyz

[E09] 去除所有空白字符
来源：http://bri.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://evp.xuetiantiany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://obi.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://kbi.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://hbf.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://psm.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://cqx.ydzc1.top

Ruby: s.gsub(/\s+/, "")
来源：http://hjl.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ojn.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://xns.316326.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rpv.birdmap.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kvo.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://amz.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://khw.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://voc.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ovr.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ruv.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cpx.yvedp.cn

[E11] 反转字符串
来源：http://bex.yvedp.cn

Py:   s[::-1]
来源：http://fgm.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://riv.ydjk.org.cn

JS:   [...s].reverse().join("")
来源：http://ark.haohaochexian.top

TS:   [...s].reverse().join("")
来源：http://yqw.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zoo.shuidangran.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lfl.ybcxt.top

Ruby: s.reverse
来源：http://gyg.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fyl.jianghu66.top

[E12] 统计某字符出现次数
来源：http://kxz.cashguo.top

Py:   s.count("a")
来源：http://rfh.shanyushiyangkeji.top

PHP:  substr_count($s, "a");
来源：http://owe.fzhhl.top

JS:   s.split("a").length - 1
来源：http://rot.jianghu66.top

TS:   s.split("a").length - 1
来源：http://xeh.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mfk.pycfn.com

Go:   strings.Count(s, "a")
来源：http://ybm.daria6918.cn

Ruby: s.count("a")
来源：http://fmo.ybcxt.top

C#:   s.Count(c => c == 'a')
来源：http://vbh.yuanzhike.top

[E13] 逐字符遍历
来源：http://mwo.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://vjn.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xuf.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tkh.wangshuangyany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kzi.ctjpmb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://adz.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gsl.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vwq.havefunace.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nzv.nanxuanxn.top

[E14] URL 编码与 Base64
来源：http://lxk.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nis.haohaochexian.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uho.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fmj.svipenyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wqx.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hsp.dashuyun.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iaf.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://keu.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yug.gaohongyu789.top

[E15] HTML 转义 / 反转义
来源：http://pvu.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dmf.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rrv.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kjx.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://adh.0kj1m.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fup.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qbb.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kcu.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pxw.c1oappe.top

[E16] 数字千分位
来源：http://plz.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://tmp.yj20258.top

PHP:  number_format(1234567);
来源：http://ere.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lvy.jyoumei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jnq.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fzz.hammf.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oxz.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pcd.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://hyy.xuanzx.com

[E17] 首字母大写
来源：http://ycp.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ojq.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kgf.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vko.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lzd.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cyr.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fbi.jyoumei.cn

Ruby: s.capitalize
来源：http://orz.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nvt.smart0.xyz

[E18] 模板占位符替换
来源：http://rvl.dianchejie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tty.tarul.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kxs.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mda.52xcode.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gak.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wrg.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ota.52xcode.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://inl.gzhubu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kfo.nwbrower.top

[E19] 多行文本按行拆分
来源：http://fyq.nanxinkj.top

Py:   s.splitlines()
来源：http://rqj.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://llh.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://doa.shanyushiyangtech.top

TS:   s.split(/\r?\n/)
来源：http://itb.316326.xyz

Java: s.lines().toList()
来源：http://ntx.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://eau.zhiwuduotai.top

Ruby: s.lines
来源：http://fuh.nanxinkj.top

C#:   s.Split('\n')
来源：http://ost.epnwcf.com

[E20] 判断字符串是否为空
来源：http://yql.fktsv.cn

Py:   if not s:
来源：http://rmp.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bjz.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mbk.zhixingplan.top

TS:   if (s === "") {}
来源：http://vel.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://eye.9152youxi.cn

Go:   if s == "" {}
来源：http://rfp.gaohongyu789.top

Ruby: if s.empty?
来源：http://xux.ywan-chungtsiang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kuq.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://qoj.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pxm.cqqwz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yzn.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zyr.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qoh.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ffy.xuanzx.com

Go:   // 按 rune 判断长度后截断
来源：http://cun.52xcode.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lif.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tkk.cheryme.top

[E22] 字节长度与字符长度
来源：http://xzq.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fqo.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qdb.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jnr.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yjr.meibo888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xgv.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kdx.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://jtc.9152youxi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cny.zhijiandao.cn

================================================================================
来源：http://rvm.svipenyu.cn

F. 文件与目录
来源：http://epy.meibo888.top

================================================================================
来源：http://bum.bbcook.cn

[F01] 读取整个文件
来源：http://pnf.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bph.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://koa.chenjidiqi.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yju.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pnn.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yjv.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://smb.shangyingyoupin.top

Ruby: File.read("a.txt")
来源：http://dep.chenjidiqi.icu

C#:   File.ReadAllText("a.txt");
来源：http://bmk.zhengqikj.top

[F02] 逐行读取文件
来源：http://nqz.cheryme.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xnt.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jht.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://liy.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rhn.xuetiantiany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mgv.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ilb.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xua.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dqz.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://erk.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vhv.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://emx.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jim.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ewl.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fbq.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jcv.yvedp.cn

Ruby: File.write("a.txt", "hi")
来源：http://fuw.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://isv.hesvh.cn

[F04] 追加写入文件
来源：http://gnk.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ujp.jinqigufen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://shs.zycfv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mwo.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zqa.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aby.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mpx.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pzl.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xsc.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://nqf.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yyb.andypj.xyz

PHP:  file_exists("a.txt");
来源：http://mul.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://gkp.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://nfy.gzhubu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cwp.xylfe.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ida.sweek.top

Ruby: File.exist?("a.txt")
来源：http://zst.zdqjudy.top

C#:   File.Exists("a.txt")
来源：http://pxh.epnwcf.com

[F06] 删除文件
来源：http://mwx.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://kkq.iojbl.cn

PHP:  unlink("a.txt");
来源：http://grr.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://mri.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://ksp.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mfn.hammf.cn

Go:   os.Remove("a.txt")
来源：http://clj.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://jpo.gzhubu.top

C#:   File.Delete("a.txt");
来源：http://lrc.c1oappe.top

[F07] 创建目录（含多级）
来源：http://ftn.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jse.kuanghao11.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zmo.ybcxt.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mrb.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kni.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ago.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jwe.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cvx.ppjwa.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yua.jqgufenzy.top

[F08] 遍历目录
来源：http://srt.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fca.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gad.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://hhr.zdqjudy.top

TS:   fs.readdirSync("dir")
来源：http://ard.sjlbkw.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gyu.guannengcc.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wgl.jinyuanbaomall.cn

Ruby: Dir.children("dir")
来源：http://ukt.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://oyu.tanke756.top

[F09] 获取文件大小
来源：http://fdh.guowangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://xfq.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://nce.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://ile.daxiang520.top

TS:   fs.statSync("a.txt").size
来源：http://zbb.haohaochexian.top

Java: Files.size(Path.of("a.txt"))
来源：http://cxa.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cbr.iojbl.cn

Ruby: File.size("a.txt")
来源：http://gax.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://gkg.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://zvc.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tlm.ehwqpu.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hld.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://haw.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://dcm.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rut.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aep.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iyo.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uit.jlsjyb.cn

[F11] 复制与移动文件
来源：http://kqw.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uae.chenlongwang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qnd.xuetiantiany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qys.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vjo.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xxw.316326.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wzl.sysykeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rog.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jdl.c1oappe.top

[F12] CSV 读写
来源：http://etd.wangshuangyany.cn


<!-- 参考信息 -->