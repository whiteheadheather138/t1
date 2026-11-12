代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xzv.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://jjz.gaohongyu789.top

Java: s.substring(1, 4)
来源：http://hvu.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://isn.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hox.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://zkt.zycfv.cn

[E04] 查找子串位置
来源：http://cyh.nwbrower.top

Py:   s.find("x");  s.index("x")
来源：http://pwg.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://evu.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://imc.redwolf501.top

TS:   s.indexOf("x")
来源：http://szy.daria6918.cn

Java: s.indexOf("x")
来源：http://nif.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://vjk.yvedp.cn

Ruby: s.index("x")
来源：http://squ.andypj.xyz

C#:   s.IndexOf("x")
来源：http://oxo.xuanzx.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://eew.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pxc.uphjek.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://esj.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uvs.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://pjo.yj20258.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hhg.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://phn.snrcjt.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lxp.mhx1999.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bgb.ehwqpu.com

[E06] 替换子串
来源：http://ezb.ppjwa.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://umo.aibaodan.cn

PHP:  str_replace("a", "b", $s);
来源：http://fij.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sua.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://uim.jinghuilouyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pfb.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pgl.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qau.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://ylf.yvedp.cn

[E07] 按分隔符拆分
来源：http://ztj.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xtl.zhoulong.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cix.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zri.jlsjyb.cn

TS:   s.split(",")
来源：http://rkx.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://kgr.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rvd.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://gbi.aibaodan.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gdj.uphjek.com

[E08] 数组按分隔符合并
来源：http://laj.gotoacloud.top

Py:   ",".join(items)
来源：http://cql.ctjpmb.com

PHP:  implode(",", $items);
来源：http://lsq.nanxuanxn.top

JS:   items.join(",")
来源：http://bib.guannengcc.top

TS:   items.join(",")
来源：http://yhe.jinyuanbaomall.cn

Java: String.join(",", items)
来源：http://poi.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://ylc.epnwcf.com

Ruby: items.join(",")
来源：http://sxb.ybcxt.top

C#:   string.Join(",", items)
来源：http://auq.shuidangran.top

[E09] 去除所有空白字符
来源：http://mpp.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ctl.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mfp.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://nzt.yonumen.top

TS:   s.replace(/\s+/g, "")
来源：http://isx.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://evc.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gmi.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lkn.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pxn.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://gaf.epnwcf.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mcx.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://icu.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://mbg.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://kjr.nanxuanxn.top

Java: String.format("%03d", 7)
来源：http://lif.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cjg.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rfh.shanyushiyangtech.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ajh.shanyushiyangkeji.top

[E11] 反转字符串
来源：http://bhj.yj202588.top

Py:   s[::-1]
来源：http://qzd.yj20258.top

PHP:  strrev($s);
来源：http://huf.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://tbk.ydzc1.top

TS:   [...s].reverse().join("")
来源：http://dws.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gcv.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://nnx.zhiwuduotai.top

Ruby: s.reverse
来源：http://trq.sysykeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://ybz.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://egp.ydzc1.top

Py:   s.count("a")
来源：http://jpp.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://msr.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://fke.quarkkingdee.top

TS:   s.split("a").length - 1
来源：http://slo.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fek.birdmap.top

Go:   strings.Count(s, "a")
来源：http://lon.wangshuangyany.cn

Ruby: s.count("a")
来源：http://grw.hesvh.cn

C#:   s.Count(c => c == 'a')
来源：http://vkt.yueranfly.top

[E13] 逐字符遍历
来源：http://jxt.wangshuangyany.cn

Py:   for ch in s: print(ch)
来源：http://wza.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hga.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kgu.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nhp.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://twu.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pdo.jlsjyb.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vsl.fehbvm.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zia.ybcxt.top

[E14] URL 编码与 Base64
来源：http://max.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rul.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cjk.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ajg.dashuyun.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pcd.fktsv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://shy.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ftw.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ryc.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rvt.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://xmv.uphjek.com

Py:   html.escape(s);  html.unescape(s)
来源：http://aju.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uni.haohaochexian.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cmi.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ngt.jinghuilouyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hzz.meibo888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://miv.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gwq.haohaochexian.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iny.hfpthk.cn

[E16] 数字千分位
来源：http://oeh.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://eav.svipenyu.cn

PHP:  number_format(1234567);
来源：http://fgh.yonumen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pqw.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tot.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://woy.guowangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ftf.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gvr.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://hfm.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://dfl.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zwz.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qci.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zkz.bjfxy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bxw.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://swb.nwbrower.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://glv.yongpay.top

Ruby: s.capitalize
来源：http://jqs.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fau.jlsjyb.cn

[E18] 模板占位符替换
来源：http://hru.mhx1999.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kcm.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tfd.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ncd.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://vjf.tanke756.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pdk.zhongyouzk.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lrt.yuxming.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kbf.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wpw.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://vva.guannengcc.top

Py:   s.splitlines()
来源：http://ivn.gogol.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://byx.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://xqu.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://pbw.zhengqikj.top

Java: s.lines().toList()
来源：http://qfo.xinyue.icu

Go:   strings.Split(s, "\n")
来源：http://jkq.jyoumei.cn

Ruby: s.lines
来源：http://udn.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://hio.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://rht.feifeiyinyue.top

Py:   if not s:
来源：http://zvl.andypj.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tsz.xziqi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xeq.jinqigfzy.top

TS:   if (s === "") {}
来源：http://dpl.pengpengdd.cyou

Java: if (s.isEmpty()) {}
来源：http://sgw.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://lre.sysykeji.top

Ruby: if s.empty?
来源：http://vfq.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tfn.wangdashe.top

[E21] 超长截断加省略号
来源：http://ynd.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tri.tarul.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xqc.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jhe.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ajh.sxryk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lri.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://wox.andypj.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://asq.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oon.9152youxi.cn

[E22] 字节长度与字符长度
来源：http://qng.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ezx.sxryk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qtx.shuidangran.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://itd.jiagoushi.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://evb.hfpthk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pou.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gmm.yj20258888.top

Ruby: s.bytesize;  s.length
来源：http://aer.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cze.vehdjk.com

================================================================================
来源：http://aqs.meibo888.top

F. 文件与目录
来源：http://fqz.daxiang520.top

================================================================================
来源：http://qcn.meibo888.top

[F01] 读取整个文件
来源：http://jvo.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dsn.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://fsb.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lwv.hesvh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wjl.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://abn.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qgv.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://whb.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://fkc.xuetiantiany.cn

[F02] 逐行读取文件
来源：http://yrx.jinqigfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://erm.jinghuilouyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pip.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wad.jqgufenzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yva.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eot.jqgfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dxe.yanxiufei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://trk.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rub.tanke756.top

[F03] 写入文件（覆盖）
来源：http://cbg.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bxs.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://eod.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ujg.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aan.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gcg.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mub.sysykeji.top

Ruby: File.write("a.txt", "hi")
来源：http://yxw.cheryme.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xaw.hongshengwenyu.top

[F04] 追加写入文件
来源：http://ryx.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rkj.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://goq.zhengqikj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vhq.yj202588.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xgq.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lwp.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vpn.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hwi.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://unj.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://vod.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nff.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://ijd.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://hzr.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://obs.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vnn.yuxming.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wkr.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://igd.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://ixd.shanyushiyangkeji.top

[F06] 删除文件
来源：http://kcy.daria6918.cn

Py:   os.remove("a.txt")
来源：http://stw.yongpay.top

PHP:  unlink("a.txt");
来源：http://aoz.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fjp.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hnm.shanyushiyangtech.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bjn.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://hac.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://tdg.fzhhl.top

C#:   File.Delete("a.txt");
来源：http://iyz.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://fei.0kj1m.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ise.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qez.chenjidiqi.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wmf.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hba.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://avw.andypj.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ith.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eew.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ega.tian-w.cn

[F08] 遍历目录
来源：http://evj.xuetiantiany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zuz.yuanzhike.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lam.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://bab.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://zqc.xingfuxueyuan.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cey.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fow.fzhhl.top

Ruby: Dir.children("dir")
来源：http://bgl.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://wre.chenjidiqi.icu

[F09] 获取文件大小
来源：http://enj.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://lqy.c1oappe.top

PHP:  filesize("a.txt");
来源：http://hny.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://atz.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://hna.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://tvd.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lby.cheryme.top

Ruby: File.size("a.txt")
来源：http://drv.haohaochexian.top

C#:   new FileInfo("a.txt").Length
来源：http://fld.fengsongda.top

[F10] 取文件扩展名 / 文件名
来源：http://aik.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sil.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eyf.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vwm.ivvv.top

TS:   path.extname("a.txt")
来源：http://xpi.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hho.aibaodan.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zoh.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wxm.daxiang520.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uwk.fehbvm.com

[F11] 复制与移动文件
来源：http://unu.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eod.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iww.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ubc.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oqr.gaohongyu789.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cxv.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bzp.dashuyun.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ovf.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wqi.9152youxi.cn

[F12] CSV 读写
来源：http://bdd.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wxb.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mfm.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hwn.zhijiandao.cn

TS:   // 同上
来源：http://fpp.daxiang520.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nje.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fnz.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://met.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nvs.yfazqb.com

================================================================================
来源：http://mjc.birdmap.top

G. 面向对象
来源：http://cwk.hcnkem.com

================================================================================
来源：http://gmh.fktsv.cn

[G01] 定义类
来源：http://aqt.dianchejie.cn

Py:   class User: pass
来源：http://kbe.wangdashe.top

PHP:  class User {}
来源：http://xkj.andypj.xyz

JS:   class User {}
来源：http://bij.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://gpu.ybcxt.top

Java: class User {}
来源：http://cpe.guowangkeji.top

Go:   type User struct { Name string }
来源：http://mwu.cdnleiting.top

Ruby: class User; end
来源：http://kts.hnxiangtu.top

C#:   class User {}
来源：http://eaa.ivvv.top


<!-- 参考信息 -->