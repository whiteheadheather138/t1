代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rzf.guannengcc.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lih.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wtv.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ual.hysaishi.cn

[E02] 重复字符串
来源：http://xnf.iojbl.cn

Py:   "ab" * 3
来源：http://bww.ppjwa.cn

PHP:  str_repeat("ab", 3);
来源：http://era.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://evm.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://zcl.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://voh.hywenlv.cn

Go:   strings.Repeat("ab", 3)
来源：http://vfs.quarkkingdee.top

Ruby: "ab" * 3
来源：http://byg.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://opk.jyoumei.cn

[E03] 截取子串
来源：http://pic.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://osh.xziqi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yqw.jinqigufen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xcx.ppjwa.cn

TS:   s.slice(1, 4)
来源：http://wuw.9152youxi.cn

Java: s.substring(1, 4)
来源：http://xpl.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://btt.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://ysk.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://vxu.hysaishi.cn

[E04] 查找子串位置
来源：http://oms.hongshengwenyu.top

Py:   s.find("x");  s.index("x")
来源：http://kpt.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://ach.sjlbkw.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kpp.jiagoushi.top

TS:   s.indexOf("x")
来源：http://ocf.sxryk.cn

Java: s.indexOf("x")
来源：http://kxl.shanyushiyangtech.top

Go:   strings.Index(s, "x")
来源：http://geg.fengsongda.top

Ruby: s.index("x")
来源：http://xiu.52xcode.cn

C#:   s.IndexOf("x")
来源：http://aro.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://zyl.jlsjyb.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://khc.hcnkem.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jsm.kuanghao11.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jye.pengpengdd.cyou

TS:   s.includes("x");  s.startsWith("a")
来源：http://qed.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gty.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sbh.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vpu.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vgp.yj20258.top

[E06] 替换子串
来源：http://xvu.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hxy.jinqigufen.top

PHP:  str_replace("a", "b", $s);
来源：http://kpd.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ufz.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://zhc.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lai.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nxn.jinyuanbaomall.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kes.snrcjt.cn

C#:   s.Replace("a", "b")
来源：http://pii.haohaochexian.top

[E07] 按分隔符拆分
来源：http://rkt.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kjs.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://awu.yfazqb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://lyo.ybcxt.top

TS:   s.split(",")
来源：http://hwe.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bxq.gogol.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rmb.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://wmn.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jwi.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://cno.hongshengwenyu.top

Py:   ",".join(items)
来源：http://aba.cucudq.cn

PHP:  implode(",", $items);
来源：http://two.pycfn.com

JS:   items.join(",")
来源：http://prj.hysaishi.cn

TS:   items.join(",")
来源：http://brr.hfpthk.cn

Java: String.join(",", items)
来源：http://hbz.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://lwu.sweek.top

Ruby: items.join(",")
来源：http://jvz.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://qag.nanxinkj.top

[E09] 去除所有空白字符
来源：http://lbr.haohaochexian.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oqo.wangdashe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ide.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://ccv.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://ykb.jqgfzy.top

Java: s.replaceAll("\\s+", "")
来源：http://hcf.quarkkingdee.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xue.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qhv.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mqt.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://iuv.yongpay.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://opb.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qpy.hongshengwenyu.top

JS:   "7".padStart(3, "0")
来源：http://nav.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://luu.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://yyj.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ryn.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gcd.ctjpmb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kdq.xylfe.cn

[E11] 反转字符串
来源：http://pkd.vqdsnc.cn

Py:   s[::-1]
来源：http://grr.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://ivs.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://tzv.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://lxm.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gdb.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xrn.feifeiyinyue.top

Ruby: s.reverse
来源：http://kqi.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kkj.hnxiangtu.top

[E12] 统计某字符出现次数
来源：http://unc.yangfankeji.com

Py:   s.count("a")
来源：http://nit.xingfuxueyuan.xyz

PHP:  substr_count($s, "a");
来源：http://hzj.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://ssf.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://joj.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kzi.tanke756.top

Go:   strings.Count(s, "a")
来源：http://ycn.havefunace.top

Ruby: s.count("a")
来源：http://squ.fehbvm.com

C#:   s.Count(c => c == 'a')
来源：http://fjy.ydzc1.top

[E13] 逐字符遍历
来源：http://czx.andypj.xyz

Py:   for ch in s: print(ch)
来源：http://tvz.yueranfly.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pql.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gcw.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://nay.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cuh.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dkz.wangdashe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pon.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wlk.dashuyun.cn

[E14] URL 编码与 Base64
来源：http://stp.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xtw.jinyuanbaomall.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vvb.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dge.zhengqikj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pxv.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wlc.wangshuangyany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lvu.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xxx.tian-w.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kyn.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://puk.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jyr.yvedp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rhk.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://roo.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://duu.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qnt.shuidangran.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://phy.gotoacloud.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nxi.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yiy.ivvv.top

[E16] 数字千分位
来源：http://pcj.aizwys.cn

Py:   f"{1234567:,}"
来源：http://vdl.gzhubu.top

PHP:  number_format(1234567);
来源：http://iyv.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qxw.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iza.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nwr.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://owl.shanyushiyangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fid.guannengcc.top

C#:   1234567.ToString("N0")
来源：http://toe.birdmap.top

[E17] 首字母大写
来源：http://wzd.hnxiangtu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zrn.havefunace.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sts.mhx1999.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sxo.zhongyouzk.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oit.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vct.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sfx.aizwys.cn

Ruby: s.capitalize
来源：http://wqo.yangfankeji.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nkt.kuanghao11.cn

[E18] 模板占位符替换
来源：http://xxw.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oyt.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vjc.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ykp.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yal.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://neo.vehdjk.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tzp.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tfm.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dwf.hcnkem.com

[E19] 多行文本按行拆分
来源：http://bos.gotoacloud.top

Py:   s.splitlines()
来源：http://odk.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ncm.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://yct.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://vme.hywenlv.cn

Java: s.lines().toList()
来源：http://zjy.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://xzp.daria6918.cn

Ruby: s.lines
来源：http://yww.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://kqg.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://ypy.wangdashe.top

Py:   if not s:
来源：http://tzl.ydzc1.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://khy.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pqc.xinyue.icu

TS:   if (s === "") {}
来源：http://sed.wangdashe.top

Java: if (s.isEmpty()) {}
来源：http://yon.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://cfl.nanxuanxn.top

Ruby: if s.empty?
来源：http://dqt.iojbl.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gsy.snrcjt.cn

[E21] 超长截断加省略号
来源：http://cov.hcnkem.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nmf.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gsu.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ezi.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zfa.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://thf.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://pjo.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ghb.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ezi.ivvv.top

[E22] 字节长度与字符长度
来源：http://xpr.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jyz.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kvk.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pmk.feifeiyinyue.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vwa.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ylv.birdmap.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bli.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://pbc.jyoumei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lwf.jinqigufen.top

================================================================================
来源：http://dxd.svipenyu.cn

F. 文件与目录
来源：http://dgb.jlsjyb.cn

================================================================================
来源：http://icg.nanxuanxn.top

[F01] 读取整个文件
来源：http://sms.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mrk.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://ccp.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mij.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nbo.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yjs.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rkw.ydjk.org.cn

Ruby: File.read("a.txt")
来源：http://rga.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://ekk.jyoumei.cn

[F02] 逐行读取文件
来源：http://wro.tianlin.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ygw.zdqjudy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qru.dianchejie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ygv.hammf.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hfd.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kyf.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jst.tian-w.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hzf.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vic.ehwqpu.com

[F03] 写入文件（覆盖）
来源：http://xuq.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pyf.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zfj.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ogv.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yrk.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lpn.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hkv.xuetiantiany.cn

Ruby: File.write("a.txt", "hi")
来源：http://avi.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://grf.daxiang520.top

[F04] 追加写入文件
来源：http://ikc.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mon.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xod.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://efs.mhx1999.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nzj.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://igu.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wdh.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aou.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tmw.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://ugj.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hif.ydjk.org.cn

PHP:  file_exists("a.txt");
来源：http://gho.sjlbkw.cn

JS:   fs.existsSync("a.txt")
来源：http://lsk.hongshengwenyu.top

TS:   fs.existsSync("a.txt")
来源：http://xeo.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fdu.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://edl.nanxuanxn.top

Ruby: File.exist?("a.txt")
来源：http://ugh.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://xzt.zhengqikj.top

[F06] 删除文件
来源：http://duy.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://jzf.yuxming.cn

PHP:  unlink("a.txt");
来源：http://cks.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://pmx.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://gsl.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ypt.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://fnd.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://vxu.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://ysf.9152youxi.cn

[F07] 创建目录（含多级）
来源：http://cek.andypj.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vmw.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nuz.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xbm.jlsjyb.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mjt.ctjpmb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aeg.zhoulong.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lzf.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hph.bjfxy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vgn.meibo888.top

[F08] 遍历目录
来源：http://crt.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://for.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dbk.xinyue.icu

JS:   fs.readdirSync("dir")
来源：http://nru.yfazqb.com

TS:   fs.readdirSync("dir")
来源：http://osr.jinqigufen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://odn.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://aaw.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://nxq.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://bcz.tarul.cn

[F09] 获取文件大小
来源：http://yry.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://vyl.yueranfly.top

PHP:  filesize("a.txt");
来源：http://bep.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://dml.jinyuanbaomall.cn

TS:   fs.statSync("a.txt").size
来源：http://mfv.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://uqu.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wzo.fktsv.cn

Ruby: File.size("a.txt")
来源：http://zxf.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://yfv.zhengqikj.top

[F10] 取文件扩展名 / 文件名
来源：http://nib.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jyz.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vfp.hnqzz.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pln.jinqigufen.top

TS:   path.extname("a.txt")
来源：http://dzi.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://faw.kuanghao11.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yuh.kuanghao11.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dyk.cqqwz.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://usy.tarul.cn

[F11] 复制与移动文件
来源：http://wte.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tzw.ehwqpu.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ngq.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kzv.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jzt.sjlbkw.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qog.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://muz.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ujy.zhijiandao.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rbe.yonumen.top

[F12] CSV 读写
来源：http://rqn.guowangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hia.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ral.chenzaomai.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rbt.jinyuanbaomall.cn

TS:   // 同上
来源：http://nze.chenjidiqi.icu


<!-- 参考信息 -->