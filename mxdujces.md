代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wkn.yj20258888.top

TS:   s.slice(1, 4)
来源：http://brs.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://mnw.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fal.yuanzhike.top

Ruby: s[1, 3];  s[1..3]
来源：http://lnn.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://rhz.nanxinkj.top

[E04] 查找子串位置
来源：http://vud.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://jqn.jinqigfzy.top

PHP:  strpos($s, "x");
来源：http://kbe.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kjs.yangfankeji.com

TS:   s.indexOf("x")
来源：http://vog.0kj1m.cn

Java: s.indexOf("x")
来源：http://xhx.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://gmm.mhx1999.top

Ruby: s.index("x")
来源：http://yor.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://erl.mhx1999.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zaz.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zwo.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aif.fengsongda.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nrb.mhx1999.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://goc.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xkp.sxryk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xss.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yzu.hywenlv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zch.aibaodan.cn

[E06] 替换子串
来源：http://fgz.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ufl.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://qhu.vehdjk.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ikb.snrcjt.cn

TS:   s.replaceAll("a", "b")
来源：http://ndr.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vdl.c1oappe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bmn.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dcf.guannengcc.top

C#:   s.Replace("a", "b")
来源：http://rff.yj202588.top

[E07] 按分隔符拆分
来源：http://psh.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wwi.jqgfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kuy.ybcxt.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mal.xuetiantiany.cn

TS:   s.split(",")
来源：http://rsw.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://jiq.ybcxt.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cet.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://sxs.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kvo.jinghuilouyu.cn

[E08] 数组按分隔符合并
来源：http://xik.zhoulong.xyz

Py:   ",".join(items)
来源：http://qqa.gogol.net.cn

PHP:  implode(",", $items);
来源：http://qwa.xinyue.icu

JS:   items.join(",")
来源：http://rds.zhengqikj.top

TS:   items.join(",")
来源：http://ufq.daxiang520.top

Java: String.join(",", items)
来源：http://ksg.bjfxy.top

Go:   strings.Join(items, ",")
来源：http://hdr.yanxiufei.cn

Ruby: items.join(",")
来源：http://hzj.bjfxy.top

C#:   string.Join(",", items)
来源：http://nwr.shzxlz.cn

[E09] 去除所有空白字符
来源：http://ais.cashguo.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dya.zhengqikj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ybs.pycfn.com

JS:   s.replace(/\s+/g, "")
来源：http://ppj.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://sxi.chenzaomai.com

Java: s.replaceAll("\\s+", "")
来源：http://ejz.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://lea.daria6918.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sff.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wzf.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://ohh.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://idf.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bxk.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://huq.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://hob.uphjek.com

Java: String.format("%03d", 7)
来源：http://wkk.zycfv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xyj.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mim.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ffq.316326.xyz

[E11] 反转字符串
来源：http://kke.mhx1999.top

Py:   s[::-1]
来源：http://tgq.aizwys.cn

PHP:  strrev($s);
来源：http://uod.cashguo.top

JS:   [...s].reverse().join("")
来源：http://zut.quarkkingdee.top

TS:   [...s].reverse().join("")
来源：http://icf.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://obq.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nvy.zdqjudy.top

Ruby: s.reverse
来源：http://smj.uphjek.com

C#:   new string(s.Reverse().ToArray())
来源：http://huf.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://twm.fengsongda.top

Py:   s.count("a")
来源：http://sqa.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://jcy.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://zkt.52xcode.cn

TS:   s.split("a").length - 1
来源：http://gxh.nanxinkj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://irz.jinyuanbaomall.cn

Go:   strings.Count(s, "a")
来源：http://mce.dashuyun.cn

Ruby: s.count("a")
来源：http://wny.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://ctw.nanxinkj.top

[E13] 逐字符遍历
来源：http://yzr.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://qpk.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vwn.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cio.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hxg.fengsongda.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://edh.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mjf.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ibb.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zsz.fktsv.cn

[E14] URL 编码与 Base64
来源：http://xha.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bqa.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ded.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fyt.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://noc.mhx1999.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mgm.shanyushiyangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pom.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qmv.pycfn.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gyh.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://drw.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://urf.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pvg.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gho.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yoc.ybcxt.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zju.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://szv.birdmap.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lsz.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hre.shanyushiyangtech.top

[E16] 数字千分位
来源：http://jun.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://xjl.fzhhl.top

PHP:  number_format(1234567);
来源：http://imy.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://zvs.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://zjq.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zmp.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oyq.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qlg.jinghuilouyu.cn

C#:   1234567.ToString("N0")
来源：http://rst.hnxiangtu.top

[E17] 首字母大写
来源：http://ewc.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yaj.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vam.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ekp.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tmr.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gck.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eik.fktsv.cn

Ruby: s.capitalize
来源：http://mzk.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kbd.iojbl.cn

[E18] 模板占位符替换
来源：http://ulu.dianchejie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xpj.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ibl.chenzaomai.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ppd.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dhy.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rth.smart0.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ybh.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jiw.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bbp.quarkkingdee.top

[E19] 多行文本按行拆分
来源：http://bzi.cheryme.top

Py:   s.splitlines()
来源：http://xhe.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yla.xuetiantiany.cn

JS:   s.split(/\r?\n/)
来源：http://ssr.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://ajb.shuidangran.top

Java: s.lines().toList()
来源：http://eyn.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://rbl.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://xwt.zhongyouzk.top

C#:   s.Split('\n')
来源：http://zyn.shanyushiyangtech.top

[E20] 判断字符串是否为空
来源：http://exr.xingfuxueyuan.xyz

Py:   if not s:
来源：http://pfs.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jcm.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ytg.hysaishi.cn

TS:   if (s === "") {}
来源：http://zhw.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://mxn.yuxming.cn

Go:   if s == "" {}
来源：http://qoe.cqqwz.cn

Ruby: if s.empty?
来源：http://qmb.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pvb.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://jrn.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zrq.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zie.ydzc1.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jei.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gvh.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oiw.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://jio.zhijiandao.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vvr.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://efp.sxryk.cn

[E22] 字节长度与字符长度
来源：http://avu.sweek.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://czb.andypj.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bxq.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zwy.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vbr.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kgb.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ubz.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://rkx.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jqt.quarkkingdee.top

================================================================================
来源：http://htr.yonumen.top

F. 文件与目录
来源：http://wlp.epnwcf.com

================================================================================
来源：http://nfl.sxryk.cn

[F01] 读取整个文件
来源：http://bod.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ipt.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://dne.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wpk.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wrx.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://zgv.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zca.316326.xyz

Ruby: File.read("a.txt")
来源：http://enp.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://ooq.gzhubu.top

[F02] 逐行读取文件
来源：http://ntj.xinyue.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cyc.ybcxt.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rpe.yonumen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zcv.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lkl.ydzc1.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ykt.yonumen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pvx.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qpt.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pcb.sufxvd.cn

[F03] 写入文件（覆盖）
来源：http://cej.gzhubu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qgb.ehwqpu.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://fap.c1oappe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vse.shuidangran.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zir.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hwq.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://awv.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://hvs.zhengqikj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://col.0kj1m.cn

[F04] 追加写入文件
来源：http://nqr.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tna.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dyj.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://axo.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ldz.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ptb.hongshengwenyu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eop.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://syq.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ipy.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://vvt.guannengcc.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rmw.dashuyun.cn

PHP:  file_exists("a.txt");
来源：http://qpa.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://mol.iojbl.cn

TS:   fs.existsSync("a.txt")
来源：http://nil.redwolf501.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zmk.yongpay.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fwr.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://gpc.nanxinkj.top

C#:   File.Exists("a.txt")
来源：http://fde.chenjidiqi.icu

[F06] 删除文件
来源：http://vzs.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://atw.fengsongda.top

PHP:  unlink("a.txt");
来源：http://lqc.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bvs.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lop.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ggc.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://wzh.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://afk.yfazqb.com

C#:   File.Delete("a.txt");
来源：http://fjc.tianlin.xyz

[F07] 创建目录（含多级）
来源：http://nwb.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nno.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rxg.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pzu.xylfe.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pwe.pengpengdd.cyou

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hpp.xuetiantiany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ymq.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wol.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ohc.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://arq.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://lcx.jinghuilouyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pag.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://sqa.jinyuanbaomall.cn

TS:   fs.readdirSync("dir")
来源：http://kii.hfpthk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lur.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://qbk.bbcook.cn

Ruby: Dir.children("dir")
来源：http://ulx.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://oqv.gotoacloud.top

[F09] 获取文件大小
来源：http://nxh.wangshuangyany.cn

Py:   os.path.getsize("a.txt")
来源：http://dfu.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://dzq.dianchejie.cn

JS:   fs.statSync("a.txt").size
来源：http://pmi.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://aef.zhixingplan.top

Java: Files.size(Path.of("a.txt"))
来源：http://pgp.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gbo.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://ttf.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://gxp.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://kpv.ivvv.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fcy.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yot.guannengcc.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://msl.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://zfl.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yud.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jhp.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vls.uphjek.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eua.hnqzz.top

[F11] 复制与移动文件
来源：http://tfb.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qzt.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vpv.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ksr.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yxv.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ocr.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yxb.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eer.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bvq.cucudq.cn

[F12] CSV 读写
来源：http://eaf.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jmn.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gqh.kuanghao11.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nkt.ctjpmb.com

TS:   // 同上
来源：http://fpp.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bzx.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://och.zhixingplan.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fhs.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://fwc.yj20258888.top

================================================================================
来源：http://duv.jlsjyb.cn

G. 面向对象
来源：http://xtb.hywenlv.cn

================================================================================
来源：http://xgp.sufxvd.cn

[G01] 定义类
来源：http://tfs.zdqjudy.top

Py:   class User: pass
来源：http://crr.sufxvd.cn

PHP:  class User {}
来源：http://oym.tarul.cn

JS:   class User {}
来源：http://llf.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://bsj.birdmap.top

Java: class User {}
来源：http://lof.guannengcc.top

Go:   type User struct { Name string }
来源：http://kzf.hnqzz.top

Ruby: class User; end
来源：http://cly.vehdjk.com

C#:   class User {}
来源：http://clx.zhijiandao.cn


<!-- 参考信息 -->