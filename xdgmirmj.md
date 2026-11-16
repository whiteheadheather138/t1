代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://zzj.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://voh.xinyue.icu

[E04] 查找子串位置
来源：http://iwv.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://npx.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://ajl.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nft.cheryme.top

TS:   s.indexOf("x")
来源：http://eke.cashguo.top

Java: s.indexOf("x")
来源：http://xjo.zhixingplan.top

Go:   strings.Index(s, "x")
来源：http://nny.yuanzhike.top

Ruby: s.index("x")
来源：http://ukg.yfazqb.com

C#:   s.IndexOf("x")
来源：http://cuo.zhijiandao.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nkb.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xyf.uphjek.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://khr.yongpay.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bhb.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://lpl.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aju.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gjm.quarkkingdee.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://igh.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nyj.dashuyun.cn

[E06] 替换子串
来源：http://gqx.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ppv.yj20258.top

PHP:  str_replace("a", "b", $s);
来源：http://xhd.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dyr.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://vcm.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ziu.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wbn.ydjk.org.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xmm.gzhubu.top

C#:   s.Replace("a", "b")
来源：http://lba.jinghuilouyu.cn

[E07] 按分隔符拆分
来源：http://viz.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jlb.daria6918.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xqr.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oiv.zhixingplan.top

TS:   s.split(",")
来源：http://ehs.jiagoushi.top

Java: s.split(",");  s.split("\\s+")
来源：http://xwn.fktsv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kic.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://gpr.cqqwz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rvf.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://gag.0kj1m.cn

Py:   ",".join(items)
来源：http://jfl.feifeiyinyue.top

PHP:  implode(",", $items);
来源：http://hes.guannengcc.top

JS:   items.join(",")
来源：http://bvj.shzxlz.cn

TS:   items.join(",")
来源：http://jpw.cdnleiting.top

Java: String.join(",", items)
来源：http://unv.pycfn.com

Go:   strings.Join(items, ",")
来源：http://fvl.tanke756.top

Ruby: items.join(",")
来源：http://mdi.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://ego.ehwqpu.com

[E09] 去除所有空白字符
来源：http://gss.zhengqikj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ogf.yfazqb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eve.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://gdr.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://qhv.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://mld.quarkkingdee.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qeb.quarkkingdee.top

Ruby: s.gsub(/\s+/, "")
来源：http://pjz.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zys.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://qfb.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lqq.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://okp.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://zcm.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://gyn.fehbvm.com

Java: String.format("%03d", 7)
来源：http://iiw.nanxinkj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yws.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qjp.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ala.yvedp.cn

[E11] 反转字符串
来源：http://bvg.chenjidiqi.icu

Py:   s[::-1]
来源：http://koq.sxryk.cn

PHP:  strrev($s);
来源：http://hsj.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://kgl.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://xwj.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hwn.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nzh.fzhhl.top

Ruby: s.reverse
来源：http://sib.c1oappe.top

C#:   new string(s.Reverse().ToArray())
来源：http://kno.yvedp.cn

[E12] 统计某字符出现次数
来源：http://kus.jqgfzy.top

Py:   s.count("a")
来源：http://qkz.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://gdt.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://bzv.redwolf501.top

TS:   s.split("a").length - 1
来源：http://lmx.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tcg.jiagoushi.top

Go:   strings.Count(s, "a")
来源：http://kmj.yueranfly.top

Ruby: s.count("a")
来源：http://iub.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://ddx.cqqwz.cn

[E13] 逐字符遍历
来源：http://jyj.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://bzo.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://roz.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vus.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://occ.yj20258.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://psm.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mnw.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sbf.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nyv.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://scp.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zxt.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hwq.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://epb.daria6918.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xen.ydzc1.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pbg.pycfn.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kzf.xuetiantiany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dtc.tian-w.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uqg.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://kdr.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mgh.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lbm.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vpa.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kfs.316326.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fmr.jinyuanbaomall.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://csg.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dmd.sysykeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://irc.chenjidiqi.icu

[E16] 数字千分位
来源：http://tcs.yonumen.top

Py:   f"{1234567:,}"
来源：http://jjd.tarul.cn

PHP:  number_format(1234567);
来源：http://azd.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jpe.ydzc1.top

TS:   (1234567).toLocaleString("en-US")
来源：http://imm.tanke756.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xjm.shangyingyoupin.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ljv.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uqr.dianchejie.cn

C#:   1234567.ToString("N0")
来源：http://kcy.jianghu66.top

[E17] 首字母大写
来源：http://cqh.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hnj.cdnleiting.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mqw.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://egp.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wre.yfazqb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://plh.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xas.sufxvd.cn

Ruby: s.capitalize
来源：http://kbx.wangdashe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gpm.0kj1m.cn

[E18] 模板占位符替换
来源：http://uve.fehbvm.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zfs.c1oappe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oms.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://owe.wangdashe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qwy.gogol.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ucf.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mqq.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ynz.yangfankeji.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hgd.jqgufenzy.top

[E19] 多行文本按行拆分
来源：http://nkc.chenlongwang.top

Py:   s.splitlines()
来源：http://mzj.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jco.chenzaomai.com

JS:   s.split(/\r?\n/)
来源：http://opo.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://ddi.tian-w.cn

Java: s.lines().toList()
来源：http://gjj.jinqigfzy.top

Go:   strings.Split(s, "\n")
来源：http://wht.aizwys.cn

Ruby: s.lines
来源：http://ndw.vehdjk.com

C#:   s.Split('\n')
来源：http://bix.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://wjl.guowangkeji.top

Py:   if not s:
来源：http://qth.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xsi.aizwys.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uvz.hnxiangtu.top

TS:   if (s === "") {}
来源：http://jvj.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://eyf.iojbl.cn

Go:   if s == "" {}
来源：http://lwy.jinqigfzy.top

Ruby: if s.empty?
来源：http://jwt.ywan-chungtsiang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ilr.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://kxz.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://thi.xinyue.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://clg.bjfxy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://syb.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gya.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xdq.epnwcf.com

Go:   // 按 rune 判断长度后截断
来源：http://bos.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cej.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ecx.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://fxb.kuanghao11.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fys.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cij.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zik.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jjg.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kas.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://azm.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://geq.hfpthk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://odh.kuanghao11.cn

================================================================================
来源：http://ext.chenlongwang.top

F. 文件与目录
来源：http://bpp.yj202588.top

================================================================================
来源：http://nwk.hnxiangtu.top

[F01] 读取整个文件
来源：http://zpx.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ytk.xylfe.cn

PHP:  file_get_contents("a.txt");
来源：http://qlo.meibo888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dfm.zhiwuduotai.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://knh.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://jse.jinyuanbaomall.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pgg.zhixingplan.top

Ruby: File.read("a.txt")
来源：http://txs.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://vig.epnwcf.com

[F02] 逐行读取文件
来源：http://jys.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tyk.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ufx.tianlin.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dpn.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mun.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nms.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zkk.hfpthk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://paq.ybcxt.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gxf.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://ljq.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://edy.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ckk.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://exp.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zdm.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pdf.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xro.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://dgg.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vor.fengsongda.top

[F04] 追加写入文件
来源：http://hyl.jlsjyb.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tol.cucudq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cqy.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mja.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nvo.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xkc.yj20258.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jzx.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bwr.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kui.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://ebm.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jsf.cheryme.top

PHP:  file_exists("a.txt");
来源：http://cgd.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://emn.yj20258.top

TS:   fs.existsSync("a.txt")
来源：http://ccl.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lqt.mhx1999.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ebt.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://ees.9152youxi.cn

C#:   File.Exists("a.txt")
来源：http://zpa.ivvv.top

[F06] 删除文件
来源：http://rtv.hywenlv.cn

Py:   os.remove("a.txt")
来源：http://ryw.sweek.top

PHP:  unlink("a.txt");
来源：http://ngn.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://fgu.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://ger.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://usg.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://wry.zhaomingkeji.xyz

Ruby: File.delete("a.txt")
来源：http://sls.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://eni.fengsongda.top

[F07] 创建目录（含多级）
来源：http://vnl.fanxiaobao.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://flm.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://big.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mob.gaohongyu789.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qek.hfpthk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://umy.yuanzhike.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://car.chenzaomai.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://svi.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qjz.cucudq.cn

[F08] 遍历目录
来源：http://iqu.yj20258.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://szt.jqgfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bzc.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://zxc.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://tvh.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ubw.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jsb.yfazqb.com

Ruby: Dir.children("dir")
来源：http://fca.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://asd.cashguo.top

[F09] 获取文件大小
来源：http://nlp.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://rje.yonumen.top

PHP:  filesize("a.txt");
来源：http://sdo.ybcxt.top

JS:   fs.statSync("a.txt").size
来源：http://uny.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://xts.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hsx.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sir.iojbl.cn

Ruby: File.size("a.txt")
来源：http://sey.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://zxq.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://bah.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ggr.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ena.cashguo.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ijp.xuanzx.com

TS:   path.extname("a.txt")
来源：http://igd.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qhp.yj202588.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pch.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mmj.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vea.meibo888.top

[F11] 复制与移动文件
来源：http://fxb.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bfc.shanyushiyangtech.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://khr.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fdc.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bfg.redwolf501.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zty.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://afz.ydzc1.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mmq.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kxc.vehdjk.com

[F12] CSV 读写
来源：http://ehj.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://izg.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://knx.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hnt.xylfe.cn

TS:   // 同上
来源：http://iej.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://udg.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zvr.ehwqpu.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lct.ivvv.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xrx.jinqigfzy.top

================================================================================
来源：http://kcs.hongshengwenyu.top

G. 面向对象
来源：http://jdx.xuanzx.com

================================================================================
来源：http://zlo.jyoumei.cn

[G01] 定义类
来源：http://vir.dashuyun.cn

Py:   class User: pass
来源：http://kbl.jqgfzy.top

PHP:  class User {}
来源：http://vhq.gogol.net.cn

JS:   class User {}
来源：http://vmi.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://dec.wangdashe.top

Java: class User {}
来源：http://mvw.yueranfly.top

Go:   type User struct { Name string }
来源：http://upj.pengpengdd.cyou

Ruby: class User; end
来源：http://xra.epnwcf.com

C#:   class User {}
来源：http://svs.ppjwa.cn

[G02] 构造函数
来源：http://qpf.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://ptr.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://zja.ybcxt.top

JS:   constructor(name) { this.name = name; }
来源：http://rgy.yuanzhike.top


<!-- 参考信息 -->