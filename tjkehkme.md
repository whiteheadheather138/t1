代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dqt.zhijiandao.cn

[E03] 截取子串
来源：http://txn.gogol.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ymn.vqdsnc.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wvg.sweek.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fgg.hcnkem.com

TS:   s.slice(1, 4)
来源：http://blt.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://jpe.bbcook.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ugt.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ybn.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://muu.ppjwa.cn

[E04] 查找子串位置
来源：http://xwf.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://qmg.yj202588.top

PHP:  strpos($s, "x");
来源：http://vcf.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iiq.yangfankeji.com

TS:   s.indexOf("x")
来源：http://ory.andypj.xyz

Java: s.indexOf("x")
来源：http://drx.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://lju.yueranfly.top

Ruby: s.index("x")
来源：http://mlx.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://bih.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uhb.dashuyun.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ppm.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://abh.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://buh.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://azp.jianghu66.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ivh.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yag.svipenyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sak.daria6918.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hmw.fzhhl.top

[E06] 替换子串
来源：http://jjf.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://trz.jinqigufen.top

PHP:  str_replace("a", "b", $s);
来源：http://ltf.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nuv.ctjpmb.com

TS:   s.replaceAll("a", "b")
来源：http://dyq.pycfn.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xjx.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uzg.nanxinkj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kkb.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://cgf.snrcjt.cn

[E07] 按分隔符拆分
来源：http://cpi.hnxiangtu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://imk.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gzo.iojbl.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dfn.sjlbkw.cn

TS:   s.split(",")
来源：http://ppi.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qij.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bsf.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://xnf.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xpe.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://eel.daria6918.cn

Py:   ",".join(items)
来源：http://ehv.cdnleiting.top

PHP:  implode(",", $items);
来源：http://xda.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://mji.ydzc1.top

TS:   items.join(",")
来源：http://ddq.aibaodan.cn

Java: String.join(",", items)
来源：http://jwd.hesvh.cn

Go:   strings.Join(items, ",")
来源：http://pao.yj20258.top

Ruby: items.join(",")
来源：http://gcj.svipenyu.cn

C#:   string.Join(",", items)
来源：http://kok.bjfxy.top

[E09] 去除所有空白字符
来源：http://vtn.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ueb.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aws.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://nfp.redwolf501.top

TS:   s.replace(/\s+/g, "")
来源：http://zfk.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://ghs.dashuyun.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ooa.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kop.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rzr.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://xrh.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qry.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xpz.shanyushiyangtech.top

JS:   "7".padStart(3, "0")
来源：http://ctn.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://jze.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://cnn.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mga.zhongyouzk.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ltc.birdmap.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ghn.tianlin.xyz

[E11] 反转字符串
来源：http://ggw.gaohongyu789.top

Py:   s[::-1]
来源：http://ugt.zhixingplan.top

PHP:  strrev($s);
来源：http://pob.yonumen.top

JS:   [...s].reverse().join("")
来源：http://esj.zhixingplan.top

TS:   [...s].reverse().join("")
来源：http://suy.hysaishi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xlk.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://puq.cucudq.cn

Ruby: s.reverse
来源：http://yye.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://kml.shzxlz.cn

[E12] 统计某字符出现次数
来源：http://tkn.hysaishi.cn

Py:   s.count("a")
来源：http://zli.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://jiz.zhixingplan.top

JS:   s.split("a").length - 1
来源：http://ops.quarkkingdee.top

TS:   s.split("a").length - 1
来源：http://rrq.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://krv.chenjidiqi.icu

Go:   strings.Count(s, "a")
来源：http://onp.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://cra.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://kpv.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://gxy.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://pnq.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gzp.sxryk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gkz.yonumen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://byh.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://enn.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://msh.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ufa.sxryk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yfg.shangyingyoupin.top

[E14] URL 编码与 Base64
来源：http://cug.hysaishi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ytw.zycfv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dys.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yah.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vuv.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lfw.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pqt.xylfe.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tzf.hywenlv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dnt.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://zll.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pqw.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jwj.wangdashe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sif.yj202588.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ean.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ves.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hku.gogol.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ncm.tanke756.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://whs.shuidangran.top

[E16] 数字千分位
来源：http://daq.birdmap.top

Py:   f"{1234567:,}"
来源：http://vij.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://uxr.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://vkz.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mce.zhongyouzk.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qkp.hammf.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bup.aizwys.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://orw.pycfn.com

C#:   1234567.ToString("N0")
来源：http://urf.52xcode.cn

[E17] 首字母大写
来源：http://sqe.smart0.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://smw.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://huh.shzxlz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qke.yvedp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jdm.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vgh.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://htb.tarul.cn

Ruby: s.capitalize
来源：http://iye.cashguo.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jgb.snrcjt.cn

[E18] 模板占位符替换
来源：http://mun.sufxvd.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tfv.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kks.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zsa.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://kyy.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://shu.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jzt.daria6918.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://glk.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pyx.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://lkb.zhixingplan.top

Py:   s.splitlines()
来源：http://daw.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gxo.nanxuanxn.top

JS:   s.split(/\r?\n/)
来源：http://ujv.hywenlv.cn

TS:   s.split(/\r?\n/)
来源：http://jjt.hywenlv.cn

Java: s.lines().toList()
来源：http://ojl.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://iep.iojbl.cn

Ruby: s.lines
来源：http://pqe.dianchejie.cn

C#:   s.Split('\n')
来源：http://qwv.chenjidiqi.icu

[E20] 判断字符串是否为空
来源：http://knn.daxiang520.top

Py:   if not s:
来源：http://smo.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wmf.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bdm.redwolf501.top

TS:   if (s === "") {}
来源：http://naa.quarkkingdee.top

Java: if (s.isEmpty()) {}
来源：http://twb.zhoulong.xyz

Go:   if s == "" {}
来源：http://whq.iojbl.cn

Ruby: if s.empty?
来源：http://hnu.tanke756.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://crh.c1oappe.top

[E21] 超长截断加省略号
来源：http://mql.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kub.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hnd.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://smg.fzhhl.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lqg.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gme.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://fit.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xsc.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uzy.nanxuanxn.top

[E22] 字节长度与字符长度
来源：http://xlv.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sfx.yvedp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://erl.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kal.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kux.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yxl.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xez.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://rhb.tianlin.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pte.zycfv.cn

================================================================================
来源：http://rbc.sweek.top

F. 文件与目录
来源：http://aop.jinqigfzy.top

================================================================================
来源：http://okq.tianlin.xyz

[F01] 读取整个文件
来源：http://vaf.svipenyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qqc.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://nzg.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mcm.dashuyun.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uqj.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://oxz.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mfa.daxiang520.top

Ruby: File.read("a.txt")
来源：http://xve.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://rcx.jlsjyb.cn

[F02] 逐行读取文件
来源：http://kjs.cheryme.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fsp.kuanghao11.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://swr.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gkr.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://smx.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gov.yuxming.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wyr.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pzm.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nci.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://frr.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yqx.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rfk.vehdjk.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xpj.sxryk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tsp.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://twh.kuanghao11.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uby.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://uzm.xylfe.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hts.yanxiufei.cn

[F04] 追加写入文件
来源：http://eyn.guowangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yvv.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uid.epnwcf.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iux.hongshengwenyu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vyy.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://joh.sweek.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wcg.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xuh.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vzx.hnxiangtu.top

[F05] 判断文件或目录是否存在
来源：http://tsv.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aup.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://zaq.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://tgt.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://nyk.0kj1m.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gvg.ivvv.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ohu.zhengqikj.top

Ruby: File.exist?("a.txt")
来源：http://rhl.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://qzr.zdbjq.cn

[F06] 删除文件
来源：http://ssp.yuanzhike.top

Py:   os.remove("a.txt")
来源：http://boj.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://unq.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://oce.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://xqb.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ujj.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://lvo.0kj1m.cn

Ruby: File.delete("a.txt")
来源：http://cqu.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://por.wangdashe.top

[F07] 创建目录（含多级）
来源：http://euz.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pbv.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pxb.chenjidiqi.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xdm.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tbo.zdbjq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vqg.zhaomingkeji.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xim.smart0.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eoc.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nvg.cashguo.top

[F08] 遍历目录
来源：http://sgs.ctjpmb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://cpq.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zvu.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://ywq.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://you.epnwcf.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://szq.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vdb.havefunace.top

Ruby: Dir.children("dir")
来源：http://kez.jinghuilouyu.cn

C#:   Directory.GetFiles("dir")
来源：http://whe.snrcjt.cn

[F09] 获取文件大小
来源：http://gci.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://ils.jianghu66.top

PHP:  filesize("a.txt");
来源：http://ypl.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://uqh.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://zei.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://nok.yonumen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xch.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://mvc.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://yjo.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://ezy.ivvv.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iuo.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yec.zhaomingkeji.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://igi.vehdjk.com

TS:   path.extname("a.txt")
来源：http://nhl.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tcg.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lsz.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xrj.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zsk.aibaodan.cn

[F11] 复制与移动文件
来源：http://swr.ywan-chungtsiang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dwn.hfpthk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://reg.ehwqpu.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oaa.yongpay.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cds.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zwp.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gbj.chenzaomai.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lrm.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ueq.tanke756.top

[F12] CSV 读写
来源：http://hud.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zkq.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uvp.hesvh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ann.gaohongyu789.top

TS:   // 同上
来源：http://jwd.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ojf.kuanghao11.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://msj.gogol.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ekh.zhoulong.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://bva.tianlin.xyz

================================================================================
来源：http://ojt.vqdsnc.cn

G. 面向对象
来源：http://tih.ydjk.org.cn

================================================================================
来源：http://bpv.ctjpmb.com

[G01] 定义类
来源：http://hfl.pycfn.com

Py:   class User: pass
来源：http://agz.pengpengdd.cyou

PHP:  class User {}
来源：http://owr.zhoulong.xyz

JS:   class User {}
来源：http://bll.cheryme.top

TS:   class User { name: string = ""; }
来源：http://kvy.vqdsnc.cn


<!-- 参考信息 -->