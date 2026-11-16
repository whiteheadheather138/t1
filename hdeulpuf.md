代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://fbe.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://tpb.tanke756.top

[E04] 查找子串位置
来源：http://aow.tanke756.top

Py:   s.find("x");  s.index("x")
来源：http://umr.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://tbx.c1oappe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ehn.haohaochexian.top

TS:   s.indexOf("x")
来源：http://wdo.birdmap.top

Java: s.indexOf("x")
来源：http://orz.yvedp.cn

Go:   strings.Index(s, "x")
来源：http://ixn.iojbl.cn

Ruby: s.index("x")
来源：http://jin.jinqigufen.top

C#:   s.IndexOf("x")
来源：http://rvx.uphjek.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://kkg.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qui.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tvf.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vtz.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jcg.c1oappe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lqn.ctjpmb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xns.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pdh.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cdi.yonumen.top

[E06] 替换子串
来源：http://wmh.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oga.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://vyp.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iyz.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://pxq.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://inv.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jyv.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mtm.mhx1999.top

C#:   s.Replace("a", "b")
来源：http://zgp.fzhhl.top

[E07] 按分隔符拆分
来源：http://pbh.52xcode.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://alq.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pke.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zvn.yuanzhike.top

TS:   s.split(",")
来源：http://cke.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://coy.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dao.yj20258888.top

Ruby: s.split(",");  s.split
来源：http://sxu.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vmt.gzhubu.top

[E08] 数组按分隔符合并
来源：http://dvm.zhongyouzk.top

Py:   ",".join(items)
来源：http://ckm.xinyue.icu

PHP:  implode(",", $items);
来源：http://akk.pengpengdd.cyou

JS:   items.join(",")
来源：http://ukb.yuanzhike.top

TS:   items.join(",")
来源：http://hqk.yangfankeji.com

Java: String.join(",", items)
来源：http://yun.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://eyi.fzhhl.top

Ruby: items.join(",")
来源：http://qnm.gogol.net.cn

C#:   string.Join(",", items)
来源：http://xhj.yuanzhike.top

[E09] 去除所有空白字符
来源：http://ska.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qvz.yfazqb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jpl.tianlin.xyz

JS:   s.replace(/\s+/g, "")
来源：http://wkn.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://qxp.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://nyn.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://qwk.ydjk.org.cn

Ruby: s.gsub(/\s+/, "")
来源：http://apb.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wij.zhixingplan.top

[E10] 左侧补零 / 定长填充
来源：http://lwn.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fob.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://isg.tarul.cn

JS:   "7".padStart(3, "0")
来源：http://knl.hnxiangtu.top

TS:   "7".padStart(3, "0")
来源：http://qaj.yonumen.top

Java: String.format("%03d", 7)
来源：http://lna.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ypt.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kpl.yj20258.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kfe.jqgfzy.top

[E11] 反转字符串
来源：http://ixw.redwolf501.top

Py:   s[::-1]
来源：http://rnp.hnqzz.top

PHP:  strrev($s);
来源：http://mii.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://qud.cdnleiting.top

TS:   [...s].reverse().join("")
来源：http://ddr.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gnj.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ctz.tanke756.top

Ruby: s.reverse
来源：http://sig.jianghu66.top

C#:   new string(s.Reverse().ToArray())
来源：http://rje.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://srf.yongpay.top

Py:   s.count("a")
来源：http://drr.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://knq.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://kmv.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://wbs.chenzaomai.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wqq.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://hnp.kuanghao11.cn

Ruby: s.count("a")
来源：http://ctq.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://kue.hcnkem.com

[E13] 逐字符遍历
来源：http://oqd.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://mrp.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hyd.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bwb.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kut.jlsjyb.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://knd.tianlin.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zpl.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jqm.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cmx.gotoacloud.top

[E14] URL 编码与 Base64
来源：http://bhx.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pve.wangdashe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://veu.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xhv.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ekv.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nvy.pengpengdd.cyou

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dhc.zdbjq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xeg.zhijiandao.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bzt.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://dce.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://axt.birdmap.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qie.c1oappe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blo.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://rsa.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ztv.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vhb.vqdsnc.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jwa.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://csm.jqgfzy.top

[E16] 数字千分位
来源：http://nna.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://zlu.guannengcc.top

PHP:  number_format(1234567);
来源：http://opy.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://spp.cashguo.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dia.shanyushiyangtech.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mky.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hxg.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://awd.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://azu.jqgufenzy.top

[E17] 首字母大写
来源：http://fit.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hnb.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://rpr.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vgc.dianchejie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wzv.sweek.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nfr.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fzg.tianlin.xyz

Ruby: s.capitalize
来源：http://jzk.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wsq.c1oappe.top

[E18] 模板占位符替换
来源：http://gmc.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pao.jinqigfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tso.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sbk.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kgw.jlsjyb.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jcv.cheryme.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aza.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zyx.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kas.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://gtw.xylfe.cn

Py:   s.splitlines()
来源：http://bcw.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zsl.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://fol.yonumen.top

TS:   s.split(/\r?\n/)
来源：http://rkd.ybcxt.top

Java: s.lines().toList()
来源：http://csg.jinqigfzy.top

Go:   strings.Split(s, "\n")
来源：http://hwi.ydjk.org.cn

Ruby: s.lines
来源：http://fje.zdbjq.cn

C#:   s.Split('\n')
来源：http://pra.ybcxt.top

[E20] 判断字符串是否为空
来源：http://bbb.havefunace.top

Py:   if not s:
来源：http://ksb.cqqwz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pvv.yangfankeji.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hcw.sufxvd.cn

TS:   if (s === "") {}
来源：http://pkh.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://ogv.xylfe.cn

Go:   if s == "" {}
来源：http://fof.cheryme.top

Ruby: if s.empty?
来源：http://vjc.zycfv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cmi.tian-w.cn

[E21] 超长截断加省略号
来源：http://ava.fzhhl.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://omx.ydjk.org.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xpz.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://erg.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://foz.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mxa.jyoumei.cn

Go:   // 按 rune 判断长度后截断
来源：http://leq.chenlongwang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qdr.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oks.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://hxg.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sbx.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qei.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jjd.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bgb.sxryk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://szj.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mev.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://uiq.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wlo.ydjk.org.cn

================================================================================
来源：http://yki.zhoulong.xyz

F. 文件与目录
来源：http://mrs.mhx1999.top

================================================================================
来源：http://riy.jianghu66.top

[F01] 读取整个文件
来源：http://ixj.epnwcf.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nds.cashguo.top

PHP:  file_get_contents("a.txt");
来源：http://hhv.jqgufenzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jiv.haohaochexian.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://adp.zdqjudy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rbb.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qkt.xinyue.icu

Ruby: File.read("a.txt")
来源：http://mxh.bbcook.cn

C#:   File.ReadAllText("a.txt");
来源：http://daz.sufxvd.cn

[F02] 逐行读取文件
来源：http://cmk.ybcxt.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kvv.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yqr.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://irj.chenzaomai.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://alv.daxiang520.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iim.zhengqikj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://klh.tarul.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vir.52xcode.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wty.chenlongwang.top

[F03] 写入文件（覆盖）
来源：http://drt.fktsv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xcv.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://lyo.fzhhl.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nvu.ppjwa.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ucn.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qfs.redwolf501.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://toz.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://lzw.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uco.epnwcf.com

[F04] 追加写入文件
来源：http://qzi.0kj1m.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eml.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bdi.52xcode.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://smo.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ddp.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jlx.tanke756.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vej.hcnkem.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kks.hongshengwenyu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vfl.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://onp.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://isf.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://ucp.316326.xyz

JS:   fs.existsSync("a.txt")
来源：http://xax.jinghuilouyu.cn

TS:   fs.existsSync("a.txt")
来源：http://owu.tianlin.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://sjm.shanyushiyangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://snb.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://szu.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://waa.yongpay.top

[F06] 删除文件
来源：http://dup.xziqi.cn

Py:   os.remove("a.txt")
来源：http://khk.havefunace.top

PHP:  unlink("a.txt");
来源：http://ffd.hongshengwenyu.top

JS:   fs.unlinkSync("a.txt")
来源：http://jcb.yongpay.top

TS:   fs.unlinkSync("a.txt")
来源：http://kth.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lrd.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://hro.yonumen.top

Ruby: File.delete("a.txt")
来源：http://tbi.meibo888.top

C#:   File.Delete("a.txt");
来源：http://xyz.0kj1m.cn

[F07] 创建目录（含多级）
来源：http://pgw.gotoacloud.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dxv.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jdg.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fbt.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qms.uphjek.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lrr.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ywl.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aim.hesvh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mhv.sweek.top

[F08] 遍历目录
来源：http://oub.zdbjq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nzo.jinqigfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mqs.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://clx.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://iuq.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oiu.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ndc.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://gju.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://izf.xylfe.cn

[F09] 获取文件大小
来源：http://doa.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://imo.xylfe.cn

PHP:  filesize("a.txt");
来源：http://qgl.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://val.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://pvn.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://jqo.yanxiufei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pjq.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://poy.kuanghao11.cn

C#:   new FileInfo("a.txt").Length
来源：http://fdl.zhijiandao.cn

[F10] 取文件扩展名 / 文件名
来源：http://myp.ybcxt.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cwd.0kj1m.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lbh.daria6918.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zul.jinqigufen.top

TS:   path.extname("a.txt")
来源：http://cks.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ttd.wangshuangyany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vrb.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vmf.yonumen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yqn.yvedp.cn

[F11] 复制与移动文件
来源：http://wdf.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kuc.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eie.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yyo.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zdp.dashuyun.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hct.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tzz.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jxu.zhoulong.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nqt.zhoulong.xyz

[F12] CSV 读写
来源：http://bmq.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://egr.xingfuxueyuan.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pkx.dashuyun.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pxn.xuanzx.com

TS:   // 同上
来源：http://qhn.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eql.c1oappe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bbz.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zlm.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nvb.xingfuxueyuan.xyz

================================================================================
来源：http://xqb.jqgfzy.top

G. 面向对象
来源：http://imp.xinyue.icu

================================================================================
来源：http://eqn.dianchejie.cn

[G01] 定义类
来源：http://tkh.gaohongyu789.top

Py:   class User: pass
来源：http://heb.epnwcf.com

PHP:  class User {}
来源：http://exf.9152youxi.cn

JS:   class User {}
来源：http://yqk.jqgufenzy.top

TS:   class User { name: string = ""; }
来源：http://eug.jinqigfzy.top

Java: class User {}
来源：http://neg.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://ovj.yvedp.cn

Ruby: class User; end
来源：http://bhk.daria6918.cn

C#:   class User {}
来源：http://tiv.jqgfzy.top

[G02] 构造函数
来源：http://ekz.xuetiantiany.cn

Py:   def __init__(self, name): self.name = name
来源：http://box.yongpay.top

PHP:  public function __construct(public string $name) {}
来源：http://zqu.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://jvn.fktsv.cn


<!-- 参考信息 -->