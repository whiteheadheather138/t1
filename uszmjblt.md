代发 wailian999

[E02] 重复字符串
来源：http://kth.chenlongwang.top

Py:   "ab" * 3
来源：http://nud.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://nxk.gzhubu.top

JS:   "ab".repeat(3)
来源：http://ohm.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://jsm.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://ljr.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://gyc.bbcook.cn

Ruby: "ab" * 3
来源：http://ffo.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pjs.gzhubu.top

[E03] 截取子串
来源：http://dgn.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yaq.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ndn.sxryk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wab.jinqigufen.top

TS:   s.slice(1, 4)
来源：http://plv.dianchejie.cn

Java: s.substring(1, 4)
来源：http://fgo.xziqi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fuy.jiagoushi.top

Ruby: s[1, 3];  s[1..3]
来源：http://khx.nwbrower.top

C#:   s.Substring(1, 3)
来源：http://czi.jqgufenzy.top

[E04] 查找子串位置
来源：http://sye.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://iwb.tian-w.cn

PHP:  strpos($s, "x");
来源：http://xmr.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pru.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://mom.gogol.net.cn

Java: s.indexOf("x")
来源：http://npc.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://hgv.andypj.xyz

Ruby: s.index("x")
来源：http://wjs.shuidangran.top

C#:   s.IndexOf("x")
来源：http://sgp.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qcz.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yqw.ydjk.org.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wur.yvedp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hna.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zdp.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yxa.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gxo.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yip.shanyushiyangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qvl.epnwcf.com

[E06] 替换子串
来源：http://xgc.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ful.jinqigufen.top

PHP:  str_replace("a", "b", $s);
来源：http://lpj.hnxiangtu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bhl.xuetiantiany.cn

TS:   s.replaceAll("a", "b")
来源：http://oqg.0kj1m.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wxt.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uqx.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ppn.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://bgq.hesvh.cn

[E07] 按分隔符拆分
来源：http://ycx.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lkk.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ywn.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://lya.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://atr.9152youxi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://btj.nwbrower.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oun.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://nhy.fanxiaobao.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rbl.52xcode.cn

[E08] 数组按分隔符合并
来源：http://lkc.nanxuanxn.top

Py:   ",".join(items)
来源：http://oms.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://nna.bbcook.cn

JS:   items.join(",")
来源：http://ntd.tian-w.cn

TS:   items.join(",")
来源：http://ndw.jiagoushi.top

Java: String.join(",", items)
来源：http://ohl.zhoulong.xyz

Go:   strings.Join(items, ",")
来源：http://eif.jinqigufen.top

Ruby: items.join(",")
来源：http://cbk.aizwys.cn

C#:   string.Join(",", items)
来源：http://cyo.ctjpmb.com

[E09] 去除所有空白字符
来源：http://mgt.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fvg.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://apj.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://utk.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://rgi.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://czu.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vof.yangfankeji.com

Ruby: s.gsub(/\s+/, "")
来源：http://jdq.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uzz.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://oar.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iay.9152youxi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bng.bjfxy.top

JS:   "7".padStart(3, "0")
来源：http://gxq.xylfe.cn

TS:   "7".padStart(3, "0")
来源：http://clo.fktsv.cn

Java: String.format("%03d", 7)
来源：http://muy.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yrp.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kjm.fanxiaobao.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hsj.shanyushiyangkeji.top

[E11] 反转字符串
来源：http://hip.pycfn.com

Py:   s[::-1]
来源：http://pth.shanyushiyangkeji.top

PHP:  strrev($s);
来源：http://fye.jyoumei.cn

JS:   [...s].reverse().join("")
来源：http://uvl.bjfxy.top

TS:   [...s].reverse().join("")
来源：http://jtg.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bvw.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pyr.shanyushiyangtech.top

Ruby: s.reverse
来源：http://ten.bjfxy.top

C#:   new string(s.Reverse().ToArray())
来源：http://goe.xuanzx.com

[E12] 统计某字符出现次数
来源：http://ezq.chenzaomai.com

Py:   s.count("a")
来源：http://uqx.dashuyun.cn

PHP:  substr_count($s, "a");
来源：http://xvv.jlsjyb.cn

JS:   s.split("a").length - 1
来源：http://lco.yongpay.top

TS:   s.split("a").length - 1
来源：http://jrt.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yvd.chenlongwang.top

Go:   strings.Count(s, "a")
来源：http://dap.tianlin.xyz

Ruby: s.count("a")
来源：http://vsv.hcnkem.com

C#:   s.Count(c => c == 'a')
来源：http://zca.xylfe.cn

[E13] 逐字符遍历
来源：http://abq.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://kot.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xyg.hnxiangtu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nbo.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cqx.jinqigfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iof.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xfl.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nua.smart0.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fab.gaohongyu789.top

[E14] URL 编码与 Base64
来源：http://ecp.ctjpmb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://czy.dianchejie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://upl.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rci.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rgc.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://evz.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nkn.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ems.ywan-chungtsiang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jkr.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://rsw.fengsongda.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dpr.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://irq.hfpthk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gnr.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://whv.hammf.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xey.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sgl.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yzg.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lpp.gaohongyu789.top

[E16] 数字千分位
来源：http://bvr.daria6918.cn

Py:   f"{1234567:,}"
来源：http://gle.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://uzz.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ebh.yueranfly.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lhj.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lwg.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://glt.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fab.ivvv.top

C#:   1234567.ToString("N0")
来源：http://agq.jinqigufen.top

[E17] 首字母大写
来源：http://bqe.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xmc.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lkb.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://obb.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zkv.yj202588.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pmy.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iyg.ybcxt.top

Ruby: s.capitalize
来源：http://zwa.gotoacloud.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rjd.ehwqpu.com

[E18] 模板占位符替换
来源：http://xme.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tih.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wvo.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jll.svipenyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ocz.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mho.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blu.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pgi.chenzaomai.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ywy.aizwys.cn

[E19] 多行文本按行拆分
来源：http://sfr.ppjwa.cn

Py:   s.splitlines()
来源：http://lek.zycfv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lrj.epnwcf.com

JS:   s.split(/\r?\n/)
来源：http://wdj.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://obx.fengsongda.top

Java: s.lines().toList()
来源：http://igt.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://pkt.jinghuilouyu.cn

Ruby: s.lines
来源：http://dew.hnxiangtu.top

C#:   s.Split('\n')
来源：http://mmg.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://mow.gaohongyu789.top

Py:   if not s:
来源：http://vjl.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lhn.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vld.xziqi.cn

TS:   if (s === "") {}
来源：http://nxq.jinyuanbaomall.cn

Java: if (s.isEmpty()) {}
来源：http://mxa.mhx1999.top

Go:   if s == "" {}
来源：http://gfp.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://rvo.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zkp.yueranfly.top

[E21] 超长截断加省略号
来源：http://zuu.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lmd.jinqigfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://orf.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eua.xuetiantiany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vtr.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lpo.shanyushiyangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://snu.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://noq.aibaodan.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xqt.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://wdk.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://crn.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hsw.yj202588.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ruf.feifeiyinyue.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lut.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yqr.316326.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://psz.svipenyu.cn

Ruby: s.bytesize;  s.length
来源：http://ilg.zdbjq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hfu.cqqwz.cn

================================================================================
来源：http://nyy.ctjpmb.com

F. 文件与目录
来源：http://oqh.cqqwz.cn

================================================================================
来源：http://zbi.aizwys.cn

[F01] 读取整个文件
来源：http://lca.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mbi.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://auy.hysaishi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fyu.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hbe.haohaochexian.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cxi.snrcjt.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wyk.sysykeji.top

Ruby: File.read("a.txt")
来源：http://zdg.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://uzg.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://edn.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://twv.jinyuanbaomall.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hjf.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gam.chenzaomai.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wqm.svipenyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://guh.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://thv.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uif.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jll.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://zua.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vva.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cft.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oef.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://azk.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wxh.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lks.tarul.cn

Ruby: File.write("a.txt", "hi")
来源：http://uhn.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mag.sufxvd.cn

[F04] 追加写入文件
来源：http://jdc.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eyx.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wcm.daxiang520.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qgn.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://irq.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vir.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vgb.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://taw.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ale.nanxuanxn.top

[F05] 判断文件或目录是否存在
来源：http://ouh.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wza.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://fsx.hysaishi.cn

JS:   fs.existsSync("a.txt")
来源：http://lfv.sjlbkw.cn

TS:   fs.existsSync("a.txt")
来源：http://vwz.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://gau.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sxq.fengsongda.top

Ruby: File.exist?("a.txt")
来源：http://pyu.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://xbm.fktsv.cn

[F06] 删除文件
来源：http://drt.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://bcy.yuxming.cn

PHP:  unlink("a.txt");
来源：http://etv.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://lbb.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tcn.fanxiaobao.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vjy.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://nvv.fehbvm.com

Ruby: File.delete("a.txt")
来源：http://eoh.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://xrv.aizwys.cn

[F07] 创建目录（含多级）
来源：http://szy.nanxinkj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zml.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://msh.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rdy.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rxc.gaohongyu789.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zry.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hqo.dianchejie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kfz.uphjek.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nfe.ybcxt.top

[F08] 遍历目录
来源：http://ice.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tva.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bgf.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://wvy.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://coo.guowangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pwu.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://png.cashguo.top

Ruby: Dir.children("dir")
来源：http://snn.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://fjz.sjlbkw.cn

[F09] 获取文件大小
来源：http://amo.zhaomingkeji.xyz

Py:   os.path.getsize("a.txt")
来源：http://xwk.epnwcf.com

PHP:  filesize("a.txt");
来源：http://ulo.yfazqb.com

JS:   fs.statSync("a.txt").size
来源：http://hyj.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://wzo.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ufl.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pjy.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://osb.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://oyp.cqqwz.cn

[F10] 取文件扩展名 / 文件名
来源：http://mly.fehbvm.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vht.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uwi.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uqq.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://bnf.tarul.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wto.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pve.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ssg.yanxiufei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gen.ydzc1.top

[F11] 复制与移动文件
来源：http://jtc.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kcw.yvedp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ybh.zhiwuduotai.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lai.zhoulong.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://goz.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xyp.tianlin.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hlx.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qgl.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lex.hongshengwenyu.top

[F12] CSV 读写
来源：http://kbq.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fsd.shanyushiyangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gqy.zhijiandao.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://isr.sjlbkw.cn

TS:   // 同上
来源：http://mni.jinqigufen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://csg.daxiang520.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wfd.jinqigufen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nhp.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ige.fzhhl.top


<!-- 参考信息 -->