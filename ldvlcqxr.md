代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://bys.zhengqikj.top

C#:   s.Substring(1, 3)
来源：http://cuj.xylfe.cn

[E04] 查找子串位置
来源：http://xsi.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://vci.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://mtm.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://udl.ydzc1.top

TS:   s.indexOf("x")
来源：http://cmj.yvedp.cn

Java: s.indexOf("x")
来源：http://xgl.meibo888.top

Go:   strings.Index(s, "x")
来源：http://wrn.hcnkem.com

Ruby: s.index("x")
来源：http://vob.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://gvd.hnqzz.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://sex.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://urz.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://idz.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pdf.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zaq.jiagoushi.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hfs.jlsjyb.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jfk.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cwe.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zwf.yfazqb.com

[E06] 替换子串
来源：http://rtf.yuanzhike.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fzn.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://ohj.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://utx.zhijiandao.cn

TS:   s.replaceAll("a", "b")
来源：http://hgc.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yxn.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dbg.gzhubu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://upq.tarul.cn

C#:   s.Replace("a", "b")
来源：http://myw.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://kqt.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qxw.hywenlv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cid.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lwj.xinyue.icu

TS:   s.split(",")
来源：http://jvj.jqgfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://kdj.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ram.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://obn.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://beh.iojbl.cn

[E08] 数组按分隔符合并
来源：http://qgo.hnxiangtu.top

Py:   ",".join(items)
来源：http://bvh.bbcook.cn

PHP:  implode(",", $items);
来源：http://ovy.jinqigfzy.top

JS:   items.join(",")
来源：http://mjq.pycfn.com

TS:   items.join(",")
来源：http://nhg.redwolf501.top

Java: String.join(",", items)
来源：http://niv.ywan-chungtsiang.top

Go:   strings.Join(items, ",")
来源：http://gcp.vqdsnc.cn

Ruby: items.join(",")
来源：http://ocx.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://gzm.sxryk.cn

[E09] 去除所有空白字符
来源：http://juu.fanxiaobao.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pxj.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aad.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://yzf.quarkkingdee.top

TS:   s.replace(/\s+/g, "")
来源：http://zgh.jinqigfzy.top

Java: s.replaceAll("\\s+", "")
来源：http://vav.wangdashe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://stf.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://shi.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hwz.ctjpmb.com

[E10] 左侧补零 / 定长填充
来源：http://pcv.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xyu.yanxiufei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lqn.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://lnb.jinghuilouyu.cn

TS:   "7".padStart(3, "0")
来源：http://kbc.sweek.top

Java: String.format("%03d", 7)
来源：http://kzb.bjfxy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tbk.pycfn.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://poi.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mwu.xuetiantiany.cn

[E11] 反转字符串
来源：http://hxm.zhengqikj.top

Py:   s[::-1]
来源：http://dds.smart0.xyz

PHP:  strrev($s);
来源：http://qfm.yfazqb.com

JS:   [...s].reverse().join("")
来源：http://ett.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://qfo.chenzaomai.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ebd.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hty.chenjidiqi.icu

Ruby: s.reverse
来源：http://tos.mhx1999.top

C#:   new string(s.Reverse().ToArray())
来源：http://glc.pycfn.com

[E12] 统计某字符出现次数
来源：http://yjs.jqgfzy.top

Py:   s.count("a")
来源：http://uik.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://cuj.jqgufenzy.top

JS:   s.split("a").length - 1
来源：http://hyp.nwbrower.top

TS:   s.split("a").length - 1
来源：http://fep.hnqzz.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hgn.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://ouy.smart0.xyz

Ruby: s.count("a")
来源：http://fsu.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://ctz.ppjwa.cn

[E13] 逐字符遍历
来源：http://kik.hnqzz.top

Py:   for ch in s: print(ch)
来源：http://jia.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vve.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fjg.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wyx.yj202588.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lnj.jinyuanbaomall.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ind.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ofh.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yyc.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://jsu.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ilm.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://oeu.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nsp.epnwcf.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ehx.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://csd.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sfe.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://irb.tarul.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rrt.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://ikz.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ljc.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ydm.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zhu.hnxiangtu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fdg.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qml.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yir.sjlbkw.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wqh.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wdq.andypj.xyz

[E16] 数字千分位
来源：http://xjw.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://njv.jianghu66.top

PHP:  number_format(1234567);
来源：http://oas.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://sff.xuanzx.com

TS:   (1234567).toLocaleString("en-US")
来源：http://xir.ehwqpu.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://crm.yuxming.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ars.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ycx.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://ifj.wangdashe.top

[E17] 首字母大写
来源：http://sdd.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vms.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pik.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://thd.dashuyun.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lpk.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vrk.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xxw.yangfankeji.com

Ruby: s.capitalize
来源：http://ljr.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gym.xingfuxueyuan.xyz

[E18] 模板占位符替换
来源：http://dbh.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gzy.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rgk.shangyingyoupin.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fyk.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hlw.nanxuanxn.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qoc.xuanzx.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lsu.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cdg.meibo888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://emo.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://ztj.c1oappe.top

Py:   s.splitlines()
来源：http://dfl.sxryk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bww.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://cnr.dashuyun.cn

TS:   s.split(/\r?\n/)
来源：http://mcc.cheryme.top

Java: s.lines().toList()
来源：http://mxu.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://izx.cheryme.top

Ruby: s.lines
来源：http://qqr.fzhhl.top

C#:   s.Split('\n')
来源：http://wel.daria6918.cn

[E20] 判断字符串是否为空
来源：http://dgb.zhixingplan.top

Py:   if not s:
来源：http://qhl.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aba.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://otp.cqqwz.cn

TS:   if (s === "") {}
来源：http://mtz.quarkkingdee.top

Java: if (s.isEmpty()) {}
来源：http://ekk.hesvh.cn

Go:   if s == "" {}
来源：http://twt.ivvv.top

Ruby: if s.empty?
来源：http://yap.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rvc.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://hnx.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ves.jianghu66.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yuf.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wuw.cashguo.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hea.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tau.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://ghg.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gim.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://amd.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://ahu.sxryk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pql.aibaodan.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fzj.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iug.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://slm.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fnw.dashuyun.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://auv.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://sgt.ehwqpu.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://phj.cucudq.cn

================================================================================
来源：http://mvt.hysaishi.cn

F. 文件与目录
来源：http://ums.dashuyun.cn

================================================================================
来源：http://det.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://cpx.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qpj.fktsv.cn

PHP:  file_get_contents("a.txt");
来源：http://jwv.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kuw.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eby.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ktk.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yma.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://yzs.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://hmc.ehwqpu.com

[F02] 逐行读取文件
来源：http://glg.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ead.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wgi.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lmt.gogol.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ida.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bkr.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fcs.shanyushiyangtech.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ltv.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yui.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://bua.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qia.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kgp.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fsb.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dxu.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rjb.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://apy.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://trp.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kjo.52xcode.cn

[F04] 追加写入文件
来源：http://hlh.sysykeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rhz.hywenlv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ach.xingfuxueyuan.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://etv.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hqd.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kdz.daria6918.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://srp.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jqs.fanxiaobao.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bmb.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://jlp.quarkkingdee.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qvj.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://raj.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://noo.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://dud.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://olg.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baw.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://vht.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://stl.shzxlz.cn

[F06] 删除文件
来源：http://brp.sjlbkw.cn

Py:   os.remove("a.txt")
来源：http://aqh.hcnkem.com

PHP:  unlink("a.txt");
来源：http://hyj.aizwys.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xfr.zdbjq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mkc.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oes.guannengcc.top

Go:   os.Remove("a.txt")
来源：http://jro.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://nuh.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://aok.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://ukk.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iqr.chenjidiqi.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dev.cqqwz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://niq.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://but.vqdsnc.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://icx.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ejx.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://waa.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iak.chenjidiqi.icu

[F08] 遍历目录
来源：http://nuu.aibaodan.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xbw.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://phm.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://wfk.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://pxl.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ihz.xziqi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zkx.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://arc.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://gjb.nwbrower.top

[F09] 获取文件大小
来源：http://gww.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://dtz.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://ado.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://hvi.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://vte.birdmap.top

Java: Files.size(Path.of("a.txt"))
来源：http://rbe.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zzt.nanxinkj.top

Ruby: File.size("a.txt")
来源：http://lga.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://pcg.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://mao.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wcy.hammf.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vvd.xinyue.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://adw.cdnleiting.top

TS:   path.extname("a.txt")
来源：http://did.yongpay.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://avm.hcnkem.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nsw.fehbvm.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ndu.sysykeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hua.vqdsnc.cn

[F11] 复制与移动文件
来源：http://ove.dashuyun.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hil.chenlongwang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ojb.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ryg.zhoulong.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hpi.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vmz.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xty.meibo888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://njt.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://grt.redwolf501.top

[F12] CSV 读写
来源：http://yxu.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fel.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xik.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mlu.52xcode.cn

TS:   // 同上
来源：http://qhp.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gcr.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://etg.dashuyun.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ybx.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gju.zhoulong.xyz

================================================================================
来源：http://aft.ehwqpu.com

G. 面向对象
来源：http://xdr.ehwqpu.com

================================================================================
来源：http://muo.shzxlz.cn

[G01] 定义类
来源：http://mve.sysykeji.top

Py:   class User: pass
来源：http://msb.xziqi.cn

PHP:  class User {}
来源：http://ook.ybcxt.top

JS:   class User {}
来源：http://xhe.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://hlr.zhijiandao.cn

Java: class User {}
来源：http://vnm.hesvh.cn

Go:   type User struct { Name string }
来源：http://jha.cdnleiting.top

Ruby: class User; end
来源：http://nqu.zhoulong.xyz

C#:   class User {}
来源：http://gtc.redwolf501.top

[G02] 构造函数
来源：http://fch.hongshengwenyu.top

Py:   def __init__(self, name): self.name = name
来源：http://upe.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ybs.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://gjw.yueranfly.top


<!-- 参考信息 -->