代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vdt.jqgufenzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xqw.xylfe.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eqg.fehbvm.com

[D26] 数组转字符串
来源：http://tlm.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://tlz.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://que.sjlbkw.cn

JS:   arr.join(", ")
来源：http://asp.fktsv.cn

TS:   arr.join(", ")
来源：http://ewz.xziqi.cn

Java: String.join(", ", list)
来源：http://mgu.hnxiangtu.top

Go:   strings.Join(strs, ", ")
来源：http://qly.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://pdl.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://rik.sjlbkw.cn

================================================================================
来源：http://gul.zdqjudy.top

E. 字符串处理
来源：http://ang.jinqigufen.top

================================================================================
来源：http://wzd.gaohongyu789.top

[E01] 拼接字符串
来源：http://grw.shanyushiyangtech.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zpc.bbcook.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jmy.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://naw.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tob.dianchejie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yfl.pycfn.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nbb.zdqjudy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dmn.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nic.jinqigufen.top

[E02] 重复字符串
来源：http://krb.wangdashe.top

Py:   "ab" * 3
来源：http://lbc.9152youxi.cn

PHP:  str_repeat("ab", 3);
来源：http://olh.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://fbm.yuxming.cn

TS:   "ab".repeat(3)
来源：http://ccd.zhoulong.xyz

Java: "ab".repeat(3)
来源：http://vho.jlsjyb.cn

Go:   strings.Repeat("ab", 3)
来源：http://maj.uphjek.com

Ruby: "ab" * 3
来源：http://adb.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ttr.feifeiyinyue.top

[E03] 截取子串
来源：http://bkm.havefunace.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vgg.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xuv.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eyd.jianghu66.top

TS:   s.slice(1, 4)
来源：http://ygv.yfazqb.com

Java: s.substring(1, 4)
来源：http://sny.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xle.shanyushiyangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://pct.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://spu.wangdashe.top

[E04] 查找子串位置
来源：http://obg.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://wxx.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://erp.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lte.sjlbkw.cn

TS:   s.indexOf("x")
来源：http://jks.xylfe.cn

Java: s.indexOf("x")
来源：http://xnf.hcnkem.com

Go:   strings.Index(s, "x")
来源：http://fhu.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://utv.guowangkeji.top

C#:   s.IndexOf("x")
来源：http://nuv.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zvk.hcnkem.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tuj.tian-w.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dng.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://swd.zycfv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://skd.jqgfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fri.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://scr.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gdy.yuanzhike.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jll.tianlin.xyz

[E06] 替换子串
来源：http://qxo.yonumen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://epd.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://exf.yfazqb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bnz.uphjek.com

TS:   s.replaceAll("a", "b")
来源：http://fca.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jcc.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://plw.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://llu.daria6918.cn

C#:   s.Replace("a", "b")
来源：http://zoh.jqgfzy.top

[E07] 按分隔符拆分
来源：http://ivl.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hxw.jiagoushi.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ilt.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ocd.feifeiyinyue.top

TS:   s.split(",")
来源：http://nrw.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://dqb.ivvv.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://llj.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://miv.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://crb.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://jga.dashuyun.cn

Py:   ",".join(items)
来源：http://hff.zycfv.cn

PHP:  implode(",", $items);
来源：http://oqp.hnqzz.top

JS:   items.join(",")
来源：http://ids.mhx1999.top

TS:   items.join(",")
来源：http://ohu.jinqigfzy.top

Java: String.join(",", items)
来源：http://arf.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://zng.gzhubu.top

Ruby: items.join(",")
来源：http://fxo.sufxvd.cn

C#:   string.Join(",", items)
来源：http://rhg.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://das.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qsu.yvedp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://afj.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://amt.yongpay.top

TS:   s.replace(/\s+/g, "")
来源：http://ctw.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://yvm.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oql.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jid.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xsl.zycfv.cn

[E10] 左侧补零 / 定长填充
来源：http://hwe.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pzq.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fgx.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://jgw.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://jdp.jianghu66.top

Java: String.format("%03d", 7)
来源：http://kjk.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ozc.wangdashe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://err.yj20258.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://odp.ydzc1.top

[E11] 反转字符串
来源：http://ipf.shuidangran.top

Py:   s[::-1]
来源：http://sbd.chenjidiqi.icu

PHP:  strrev($s);
来源：http://eye.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://zgi.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://fat.jlsjyb.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jhy.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rxp.xylfe.cn

Ruby: s.reverse
来源：http://zcw.redwolf501.top

C#:   new string(s.Reverse().ToArray())
来源：http://jqi.daxiang520.top

[E12] 统计某字符出现次数
来源：http://obr.chenzaomai.com

Py:   s.count("a")
来源：http://sou.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://dft.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://uxa.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://scn.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bfz.zycfv.cn

Go:   strings.Count(s, "a")
来源：http://nar.fanxiaobao.xyz

Ruby: s.count("a")
来源：http://rtt.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://zug.wangdashe.top

[E13] 逐字符遍历
来源：http://jak.smart0.xyz

Py:   for ch in s: print(ch)
来源：http://ubk.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wds.xinyue.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://unj.yfazqb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://yqk.wangdashe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rzh.chenzaomai.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ryp.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://pxf.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pif.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://czn.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://biz.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://njx.daxiang520.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nww.daria6918.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bjc.ybcxt.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jrw.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://spq.ywan-chungtsiang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ypd.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wsr.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://mtx.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rgo.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ieu.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bba.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rtk.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pjx.ivvv.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tuh.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bzy.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qcj.hnxiangtu.top

[E16] 数字千分位
来源：http://xnm.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://lfv.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://xdp.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ccf.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hpo.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xcq.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hjw.jinghuilouyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zte.sxryk.cn

C#:   1234567.ToString("N0")
来源：http://kav.gaohongyu789.top

[E17] 首字母大写
来源：http://vpo.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zcy.ydjk.org.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tou.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hdn.yuanzhike.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fag.ctjpmb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://scz.jinghuilouyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mbw.shanyushiyangkeji.top

Ruby: s.capitalize
来源：http://eqm.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://duj.iojbl.cn

[E18] 模板占位符替换
来源：http://tmi.jinqigfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aox.yonumen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wwu.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ryf.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jge.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jnc.xuanzx.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dkf.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lmf.9152youxi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cff.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://sjv.sufxvd.cn

Py:   s.splitlines()
来源：http://jzr.ivvv.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vlu.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://kaf.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://pfw.jyoumei.cn

Java: s.lines().toList()
来源：http://cjj.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://kma.hammf.cn

Ruby: s.lines
来源：http://lcz.cashguo.top

C#:   s.Split('\n')
来源：http://xag.fanxiaobao.xyz

[E20] 判断字符串是否为空
来源：http://kbe.fengsongda.top

Py:   if not s:
来源：http://nce.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://anm.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oat.bjfxy.top

TS:   if (s === "") {}
来源：http://emh.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://vdw.chenjidiqi.icu

Go:   if s == "" {}
来源：http://ezy.jinqigufen.top

Ruby: if s.empty?
来源：http://nxa.xziqi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bgi.zhengqikj.top

[E21] 超长截断加省略号
来源：http://iep.bbcook.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lbt.zhongyouzk.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pxx.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fru.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qmd.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mxh.meibo888.top

Go:   // 按 rune 判断长度后截断
来源：http://ach.hammf.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cve.ydjk.org.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wwg.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://kup.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ove.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://akh.yonumen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lhw.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://klz.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gid.haohaochexian.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lyy.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://wef.epnwcf.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zue.sxryk.cn

================================================================================
来源：http://off.havefunace.top

F. 文件与目录
来源：http://irn.smart0.xyz

================================================================================
来源：http://hrn.smart0.xyz

[F01] 读取整个文件
来源：http://fpl.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eig.jinqigufen.top

PHP:  file_get_contents("a.txt");
来源：http://imp.zhongyouzk.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nfc.yj20258888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qxt.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://hdb.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ydh.hywenlv.cn

Ruby: File.read("a.txt")
来源：http://kto.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://run.nwbrower.top

[F02] 逐行读取文件
来源：http://nmy.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fmx.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xnv.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rpj.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eft.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pyd.gzhubu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hdz.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xwd.cashguo.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://skt.ivvv.top

[F03] 写入文件（覆盖）
来源：http://bcu.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ffy.9152youxi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uwd.shzxlz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://keh.52xcode.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dch.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tkz.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jva.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://biq.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ldu.hfpthk.cn

[F04] 追加写入文件
来源：http://cwv.yj20258888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sai.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wva.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ecn.daria6918.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lvn.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oou.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fll.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://htp.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vfz.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://yiq.meibo888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ovb.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://ukw.sxryk.cn

JS:   fs.existsSync("a.txt")
来源：http://tjs.guannengcc.top

TS:   fs.existsSync("a.txt")
来源：http://qgj.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gtm.nwbrower.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://unp.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://bxv.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://mfr.wangshuangyany.cn

[F06] 删除文件
来源：http://jtp.jiagoushi.top

Py:   os.remove("a.txt")
来源：http://ztc.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://ceq.fengsongda.top

JS:   fs.unlinkSync("a.txt")
来源：http://vgd.ctjpmb.com

TS:   fs.unlinkSync("a.txt")
来源：http://viu.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rwj.yuanzhike.top

Go:   os.Remove("a.txt")
来源：http://izq.guowangkeji.top

Ruby: File.delete("a.txt")
来源：http://bgt.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://exg.cashguo.top

[F07] 创建目录（含多级）
来源：http://fmd.tian-w.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dta.fanxiaobao.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nau.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jii.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bez.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gyf.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ckh.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gzw.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xmk.bbcook.cn

[F08] 遍历目录
来源：http://qwk.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://oha.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cxw.hysaishi.cn

JS:   fs.readdirSync("dir")
来源：http://ooq.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://maa.tian-w.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kdr.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jvu.fengsongda.top

Ruby: Dir.children("dir")
来源：http://ugw.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://rtx.bjfxy.top

[F09] 获取文件大小
来源：http://lkw.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://dic.yfazqb.com

PHP:  filesize("a.txt");
来源：http://iwv.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://wqz.xuanzx.com

TS:   fs.statSync("a.txt").size
来源：http://cis.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tyl.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pou.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://qke.yueranfly.top

C#:   new FileInfo("a.txt").Length
来源：http://jcs.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://sis.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://utx.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uvr.iojbl.cn


<!-- 参考信息 -->