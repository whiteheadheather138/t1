代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://auu.meibo888.top

C#:   s.Substring(1, 3)
来源：http://hcu.ydzc1.top

[E04] 查找子串位置
来源：http://tru.chenjidiqi.icu

Py:   s.find("x");  s.index("x")
来源：http://tpw.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://gfn.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xyh.sjlbkw.cn

TS:   s.indexOf("x")
来源：http://ios.mhx1999.top

Java: s.indexOf("x")
来源：http://ilu.zhaomingkeji.xyz

Go:   strings.Index(s, "x")
来源：http://zxw.fengsongda.top

Ruby: s.index("x")
来源：http://rhr.tian-w.cn

C#:   s.IndexOf("x")
来源：http://sqm.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://elh.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vxp.ywan-chungtsiang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xfs.epnwcf.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vlz.zhijiandao.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ybj.0kj1m.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cwf.bbcook.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mje.hnqzz.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://njm.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hst.zhijiandao.cn

[E06] 替换子串
来源：http://fem.vehdjk.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yla.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://pnw.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bwq.jianghu66.top

TS:   s.replaceAll("a", "b")
来源：http://drh.xziqi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://joy.zhongyouzk.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ewr.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yvq.yonumen.top

C#:   s.Replace("a", "b")
来源：http://wvv.ehwqpu.com

[E07] 按分隔符拆分
来源：http://llp.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lxn.jinyuanbaomall.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dee.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ftn.tarul.cn

TS:   s.split(",")
来源：http://oeo.ybcxt.top

Java: s.split(",");  s.split("\\s+")
来源：http://kgz.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pfl.pycfn.com

Ruby: s.split(",");  s.split
来源：http://owx.iojbl.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nse.zhixingplan.top

[E08] 数组按分隔符合并
来源：http://avb.zhaomingkeji.xyz

Py:   ",".join(items)
来源：http://yzf.iojbl.cn

PHP:  implode(",", $items);
来源：http://ntn.pengpengdd.cyou

JS:   items.join(",")
来源：http://icg.shanyushiyangkeji.top

TS:   items.join(",")
来源：http://tkp.gaohongyu789.top

Java: String.join(",", items)
来源：http://tan.ctjpmb.com

Go:   strings.Join(items, ",")
来源：http://vtj.c1oappe.top

Ruby: items.join(",")
来源：http://peo.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://ljp.iojbl.cn

[E09] 去除所有空白字符
来源：http://fsb.ehwqpu.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://drm.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tug.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://tyv.yvedp.cn

TS:   s.replace(/\s+/g, "")
来源：http://qsa.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://kng.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dtd.sufxvd.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ted.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gfm.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://gis.havefunace.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://woz.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qvc.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://dkz.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://qwj.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://fjp.yvedp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vpw.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iwn.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nlo.kuanghao11.cn

[E11] 反转字符串
来源：http://joo.sysykeji.top

Py:   s[::-1]
来源：http://flk.sufxvd.cn

PHP:  strrev($s);
来源：http://hio.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://ojc.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://hke.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xdg.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ukc.zhaomingkeji.xyz

Ruby: s.reverse
来源：http://yje.feifeiyinyue.top

C#:   new string(s.Reverse().ToArray())
来源：http://diy.guowangkeji.top

[E12] 统计某字符出现次数
来源：http://swv.pengpengdd.cyou

Py:   s.count("a")
来源：http://yhu.aizwys.cn

PHP:  substr_count($s, "a");
来源：http://irr.jqgfzy.top

JS:   s.split("a").length - 1
来源：http://ttg.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://pyo.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fed.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://hdq.cheryme.top

Ruby: s.count("a")
来源：http://qru.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://sno.zhoulong.xyz

[E13] 逐字符遍历
来源：http://skm.yvedp.cn

Py:   for ch in s: print(ch)
来源：http://pjn.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yxm.ydjk.org.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mvd.shzxlz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://klv.zycfv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qvi.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oad.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oij.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qfi.yj20258.top

[E14] URL 编码与 Base64
来源：http://gyj.yj20258.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hlg.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kpb.shuidangran.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nvz.birdmap.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hwu.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://muq.cheryme.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://awa.chenlongwang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pgz.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zwf.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://czh.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://tqi.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ohp.shanyushiyangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://awf.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://myh.sufxvd.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cbw.meibo888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sbe.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pal.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jll.xuanzx.com

[E16] 数字千分位
来源：http://ojg.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://jke.pycfn.com

PHP:  number_format(1234567);
来源：http://zrg.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xqy.yongpay.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zog.316326.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jqs.hfpthk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hcf.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qwj.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://xcf.316326.xyz

[E17] 首字母大写
来源：http://mmw.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://adm.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ays.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vku.xinyue.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://low.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zzh.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://msv.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://teo.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dct.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://fck.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lvn.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vca.ctjpmb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://sqz.shuidangran.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lqf.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vyl.gotoacloud.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ttf.sweek.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hfu.zhongyouzk.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kof.dianchejie.cn

[E19] 多行文本按行拆分
来源：http://lha.cdnleiting.top

Py:   s.splitlines()
来源：http://xvs.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://apm.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://cum.svipenyu.cn

TS:   s.split(/\r?\n/)
来源：http://kcl.sufxvd.cn

Java: s.lines().toList()
来源：http://qov.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://qbz.quarkkingdee.top

Ruby: s.lines
来源：http://mxr.snrcjt.cn

C#:   s.Split('\n')
来源：http://aaz.hcnkem.com

[E20] 判断字符串是否为空
来源：http://vcn.jiagoushi.top

Py:   if not s:
来源：http://dki.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wyw.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ast.aibaodan.cn

TS:   if (s === "") {}
来源：http://oxo.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://qci.mhx1999.top

Go:   if s == "" {}
来源：http://zye.cdnleiting.top

Ruby: if s.empty?
来源：http://mhs.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ywp.pycfn.com

[E21] 超长截断加省略号
来源：http://kss.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vmo.daria6918.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ifc.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nrj.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kwu.sxryk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bar.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://aqk.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://win.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rfi.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://npv.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uxv.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lkg.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oth.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ldh.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zge.andypj.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mlr.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://fnp.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pro.cucudq.cn

================================================================================
来源：http://cpi.316326.xyz

F. 文件与目录
来源：http://htr.ybcxt.top

================================================================================
来源：http://dva.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://iue.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vpt.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://nfa.nwbrower.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pwk.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ywq.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gbr.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bgg.hnqzz.top

Ruby: File.read("a.txt")
来源：http://mmf.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://xbd.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://skl.xinyue.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wlv.52xcode.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wbu.cashguo.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://swa.sufxvd.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fag.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zjm.zdbjq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://olu.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mzy.ctjpmb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wre.yuanzhike.top

[F03] 写入文件（覆盖）
来源：http://hpk.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jht.yongpay.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xlm.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://act.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ify.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ybi.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xoa.quarkkingdee.top

Ruby: File.write("a.txt", "hi")
来源：http://ubn.iojbl.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jtd.haohaochexian.top

[F04] 追加写入文件
来源：http://ohr.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zvt.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zja.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uhh.ydzc1.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nkn.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://isv.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xgp.sweek.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sio.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nhr.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://xgl.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fdj.316326.xyz

PHP:  file_exists("a.txt");
来源：http://oid.guannengcc.top

JS:   fs.existsSync("a.txt")
来源：http://dhd.sweek.top

TS:   fs.existsSync("a.txt")
来源：http://xyc.tian-w.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://edb.ybcxt.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://heh.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://buq.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://lmp.bjfxy.top

[F06] 删除文件
来源：http://nsq.yj20258888.top

Py:   os.remove("a.txt")
来源：http://iws.chenjidiqi.icu

PHP:  unlink("a.txt");
来源：http://czd.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ybo.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://hjh.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zea.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://pxd.bjfxy.top

Ruby: File.delete("a.txt")
来源：http://orm.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://sod.pycfn.com

[F07] 创建目录（含多级）
来源：http://zqr.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bwg.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ogq.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://btg.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xtg.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sfi.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vix.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dir.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bca.zhengqikj.top

[F08] 遍历目录
来源：http://qdk.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://teq.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zyn.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://nub.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://agy.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xyi.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://xic.yj20258.top

Ruby: Dir.children("dir")
来源：http://wkc.jyoumei.cn

C#:   Directory.GetFiles("dir")
来源：http://lbh.hcnkem.com

[F09] 获取文件大小
来源：http://quq.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://fmh.fanxiaobao.xyz

PHP:  filesize("a.txt");
来源：http://oau.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://bti.pycfn.com

TS:   fs.statSync("a.txt").size
来源：http://mbs.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://rrp.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yud.hnxiangtu.top

Ruby: File.size("a.txt")
来源：http://qdn.yj202588.top

C#:   new FileInfo("a.txt").Length
来源：http://yal.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://ptk.fzhhl.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mss.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://war.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nal.vehdjk.com

TS:   path.extname("a.txt")
来源：http://qyb.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hws.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://upt.gaohongyu789.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tbs.jqgfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://got.yfazqb.com

[F11] 复制与移动文件
来源：http://xme.hfpthk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://swh.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://igi.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://whf.yanxiufei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pwh.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fwg.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xbi.hfpthk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lcq.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eks.ehwqpu.com

[F12] CSV 读写
来源：http://qad.sjlbkw.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xiu.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jqq.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://noy.tanke756.top

TS:   // 同上
来源：http://ljt.kuanghao11.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sit.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://stt.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hzk.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cgo.tianlin.xyz

================================================================================
来源：http://hwl.zhaomingkeji.xyz

G. 面向对象
来源：http://vou.ywan-chungtsiang.top

================================================================================
来源：http://svb.vqdsnc.cn

[G01] 定义类
来源：http://owo.zdqjudy.top

Py:   class User: pass
来源：http://mss.redwolf501.top

PHP:  class User {}
来源：http://gya.jiagoushi.top

JS:   class User {}
来源：http://nmm.yongpay.top

TS:   class User { name: string = ""; }
来源：http://kfv.jqgfzy.top

Java: class User {}
来源：http://cma.yonumen.top

Go:   type User struct { Name string }
来源：http://vpv.yangfankeji.com

Ruby: class User; end
来源：http://xrp.vehdjk.com

C#:   class User {}
来源：http://wjk.chenjidiqi.icu

[G02] 构造函数
来源：http://uvy.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://ciu.vehdjk.com

PHP:  public function __construct(public string $name) {}
来源：http://wpu.shzxlz.cn

JS:   constructor(name) { this.name = name; }
来源：http://baf.fehbvm.com


<!-- 参考信息 -->