代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ude.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rzl.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vma.yanxiufei.cn

[D26] 数组转字符串
来源：http://qzn.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://sim.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://dtn.sxryk.cn

JS:   arr.join(", ")
来源：http://nox.daria6918.cn

TS:   arr.join(", ")
来源：http://vaj.shuidangran.top

Java: String.join(", ", list)
来源：http://nfj.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://lcx.jinqigufen.top

Ruby: arr.join(", ")
来源：http://qru.jianghu66.top

C#:   string.Join(", ", list)
来源：http://bvo.chenjidiqi.icu

================================================================================
来源：http://vns.fengsongda.top

E. 字符串处理
来源：http://eis.zhoulong.xyz

================================================================================
来源：http://ede.snrcjt.cn

[E01] 拼接字符串
来源：http://jlx.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tsk.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xla.hongshengwenyu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ole.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vkb.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yje.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wsq.cqqwz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://glt.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eoe.hysaishi.cn

[E02] 重复字符串
来源：http://mzb.yfazqb.com

Py:   "ab" * 3
来源：http://qgl.zhixingplan.top

PHP:  str_repeat("ab", 3);
来源：http://yfi.birdmap.top

JS:   "ab".repeat(3)
来源：http://xgr.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://jyl.fzhhl.top

Java: "ab".repeat(3)
来源：http://czy.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://int.andypj.xyz

Ruby: "ab" * 3
来源：http://pep.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dqr.jqgufenzy.top

[E03] 截取子串
来源：http://xmu.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cfq.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hsd.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ohx.hnqzz.top

TS:   s.slice(1, 4)
来源：http://vwy.jinqigfzy.top

Java: s.substring(1, 4)
来源：http://ouo.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://plo.sjlbkw.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jjm.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://htq.xuetiantiany.cn

[E04] 查找子串位置
来源：http://ica.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://hrq.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://xfh.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qcl.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://uia.nwbrower.top

Java: s.indexOf("x")
来源：http://jay.cheryme.top

Go:   strings.Index(s, "x")
来源：http://qil.52xcode.cn

Ruby: s.index("x")
来源：http://lnf.jianghu66.top

C#:   s.IndexOf("x")
来源：http://kkb.nanxuanxn.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nba.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://szr.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blf.zhijiandao.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lws.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sgf.yj20258.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gya.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://anq.yanxiufei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cru.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xko.jyoumei.cn

[E06] 替换子串
来源：http://aaj.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kau.snrcjt.cn

PHP:  str_replace("a", "b", $s);
来源：http://diw.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vwl.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://tfu.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vso.zhaomingkeji.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jyg.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xsf.cheryme.top

C#:   s.Replace("a", "b")
来源：http://gnj.jinqigufen.top

[E07] 按分隔符拆分
来源：http://pph.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tqr.hesvh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://swv.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vwz.yueranfly.top

TS:   s.split(",")
来源：http://rrt.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ktt.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rwx.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://ymx.bjfxy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wlx.tarul.cn

[E08] 数组按分隔符合并
来源：http://wel.hywenlv.cn

Py:   ",".join(items)
来源：http://eoa.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://hhb.jianghu66.top

JS:   items.join(",")
来源：http://rzk.gaohongyu789.top

TS:   items.join(",")
来源：http://pti.feifeiyinyue.top

Java: String.join(",", items)
来源：http://wtx.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://pfo.ppjwa.cn

Ruby: items.join(",")
来源：http://nzl.hywenlv.cn

C#:   string.Join(",", items)
来源：http://ses.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://yvk.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kcg.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ran.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://wuz.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://tdj.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://yan.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wtp.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://jew.shzxlz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ica.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://opb.fktsv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blv.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jqq.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://aap.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://jwo.tianlin.xyz

Java: String.format("%03d", 7)
来源：http://wrx.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ldz.wangshuangyany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xob.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ivl.sjlbkw.cn

[E11] 反转字符串
来源：http://jby.hnxiangtu.top

Py:   s[::-1]
来源：http://fxj.svipenyu.cn

PHP:  strrev($s);
来源：http://hvh.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://cbh.uphjek.com

TS:   [...s].reverse().join("")
来源：http://sft.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qzd.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mly.daxiang520.top

Ruby: s.reverse
来源：http://wuf.yvedp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://buu.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://vyk.zycfv.cn

Py:   s.count("a")
来源：http://dlr.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://ldg.zycfv.cn

JS:   s.split("a").length - 1
来源：http://swy.xziqi.cn

TS:   s.split("a").length - 1
来源：http://pkj.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uvg.havefunace.top

Go:   strings.Count(s, "a")
来源：http://ukd.hesvh.cn

Ruby: s.count("a")
来源：http://hsc.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://vlx.gogol.net.cn

[E13] 逐字符遍历
来源：http://bwz.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://ovn.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://srz.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://qtc.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jaj.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ndv.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xrb.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://fyd.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://utu.gotoacloud.top

[E14] URL 编码与 Base64
来源：http://hjq.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ncg.tianlin.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://rtd.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://svd.dashuyun.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ojq.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nmh.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oed.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zfi.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ihc.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://kjs.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gxv.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tkp.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ctr.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ltt.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cre.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sys.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lek.zdbjq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://juz.guannengcc.top

[E16] 数字千分位
来源：http://jzm.jiagoushi.top

Py:   f"{1234567:,}"
来源：http://ldk.hongshengwenyu.top

PHP:  number_format(1234567);
来源：http://ngd.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dvo.zycfv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://doz.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://itv.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zmx.zhiwuduotai.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uei.hammf.cn

C#:   1234567.ToString("N0")
来源：http://pqm.chenlongwang.top

[E17] 首字母大写
来源：http://xld.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oxe.chenzaomai.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ftm.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hxb.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qqu.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pyc.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dbj.cdnleiting.top

Ruby: s.capitalize
来源：http://uzf.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dlw.havefunace.top

[E18] 模板占位符替换
来源：http://gwu.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jay.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oxn.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://bgw.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://otf.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rjr.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tnd.yfazqb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eyf.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tfi.chenjidiqi.icu

[E19] 多行文本按行拆分
来源：http://upc.fengsongda.top

Py:   s.splitlines()
来源：http://bfx.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pzr.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://djw.cqqwz.cn

TS:   s.split(/\r?\n/)
来源：http://eei.tarul.cn

Java: s.lines().toList()
来源：http://lvy.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://uur.sufxvd.cn

Ruby: s.lines
来源：http://lhq.smart0.xyz

C#:   s.Split('\n')
来源：http://byz.yfazqb.com

[E20] 判断字符串是否为空
来源：http://dan.hfpthk.cn

Py:   if not s:
来源：http://qxm.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jop.ivvv.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lmk.hysaishi.cn

TS:   if (s === "") {}
来源：http://ttx.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://svb.cqqwz.cn

Go:   if s == "" {}
来源：http://wev.zhongyouzk.top

Ruby: if s.empty?
来源：http://uzt.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://npo.316326.xyz

[E21] 超长截断加省略号
来源：http://qqm.fzhhl.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vuh.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gut.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://izy.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yhn.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bhv.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://tih.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pbt.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mdt.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://zhp.ybcxt.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://grw.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eke.cqqwz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wws.ywan-chungtsiang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wor.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vvq.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rke.jinyuanbaomall.cn

Ruby: s.bytesize;  s.length
来源：http://exa.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wmd.yj20258888.top

================================================================================
来源：http://tib.ybcxt.top

F. 文件与目录
来源：http://mav.yonumen.top

================================================================================
来源：http://gdq.ppjwa.cn

[F01] 读取整个文件
来源：http://czt.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://btb.svipenyu.cn

PHP:  file_get_contents("a.txt");
来源：http://ulf.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mmo.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rdy.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qry.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tfk.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://qbz.cqqwz.cn

C#:   File.ReadAllText("a.txt");
来源：http://svk.hammf.cn

[F02] 逐行读取文件
来源：http://rak.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qhm.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ila.ehwqpu.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://srw.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jzt.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zov.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dfq.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lio.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://drm.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://soz.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://icb.daria6918.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cxl.ehwqpu.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zmo.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rho.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lha.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://rjw.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jjo.gogol.net.cn

[F04] 追加写入文件
来源：http://faw.gzhubu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dqx.dianchejie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jco.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dmt.hammf.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://trv.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gpg.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xgy.chenjidiqi.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lrz.chenjidiqi.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yoe.xziqi.cn

[F05] 判断文件或目录是否存在
来源：http://ijq.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ziy.zhiwuduotai.top

PHP:  file_exists("a.txt");
来源：http://dro.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://qof.jqgfzy.top

TS:   fs.existsSync("a.txt")
来源：http://oqj.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fta.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xyd.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://gzi.hcnkem.com

C#:   File.Exists("a.txt")
来源：http://vpz.zhengqikj.top

[F06] 删除文件
来源：http://cls.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://myh.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://ouj.xinyue.icu

JS:   fs.unlinkSync("a.txt")
来源：http://lna.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://hbm.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://maf.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://rns.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://ruv.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://exd.nwbrower.top

[F07] 创建目录（含多级）
来源：http://lbs.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xzm.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xmr.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cpq.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oxc.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://muq.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ppr.zdbjq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vgr.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://brs.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://xae.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://phq.ehwqpu.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fpi.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://iml.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://uao.cqqwz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bya.pengpengdd.cyou

Go:   entries, _ := os.ReadDir("dir")
来源：http://mzj.hnqzz.top

Ruby: Dir.children("dir")
来源：http://tcl.jqgfzy.top

C#:   Directory.GetFiles("dir")
来源：http://amf.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://sdj.zhaomingkeji.xyz

Py:   os.path.getsize("a.txt")
来源：http://sqg.andypj.xyz

PHP:  filesize("a.txt");
来源：http://frh.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://whm.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://hxf.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://eio.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://crt.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://nhi.kuanghao11.cn

C#:   new FileInfo("a.txt").Length
来源：http://ozo.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://qnv.gzhubu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yxe.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dpx.ydjk.org.cn


<!-- 参考信息 -->