代发 wailian999

PHP:  strpos($s, "x");
来源：http://kod.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rpt.yongpay.top

TS:   s.indexOf("x")
来源：http://uqb.jianghu66.top

Java: s.indexOf("x")
来源：http://iov.yj20258.top

Go:   strings.Index(s, "x")
来源：http://ahv.aibaodan.cn

Ruby: s.index("x")
来源：http://mju.nwbrower.top

C#:   s.IndexOf("x")
来源：http://yvx.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pgk.pengpengdd.cyou

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qpk.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jpc.yonumen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kuv.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wch.cucudq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uvn.quarkkingdee.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sdh.hesvh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ypz.jyoumei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oqq.ydjk.org.cn

[E06] 替换子串
来源：http://dsy.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bhb.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://mxr.bjfxy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aqc.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://tyx.iojbl.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mkd.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dsf.yuxming.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ygb.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://gat.aibaodan.cn

[E07] 按分隔符拆分
来源：http://kfi.feifeiyinyue.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://msv.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jik.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mrk.yanxiufei.cn

TS:   s.split(",")
来源：http://lxb.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bzs.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kii.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://vjd.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aox.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://yjs.nwbrower.top

Py:   ",".join(items)
来源：http://boc.cheryme.top

PHP:  implode(",", $items);
来源：http://ypa.shangyingyoupin.top

JS:   items.join(",")
来源：http://kbv.cdnleiting.top

TS:   items.join(",")
来源：http://fzl.yanxiufei.cn

Java: String.join(",", items)
来源：http://neb.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://eum.gogol.net.cn

Ruby: items.join(",")
来源：http://qit.jqgfzy.top

C#:   string.Join(",", items)
来源：http://grz.9152youxi.cn

[E09] 去除所有空白字符
来源：http://hgm.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://srk.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://luy.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://ozg.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://ovf.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://cmn.zhengqikj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jue.cashguo.top

Ruby: s.gsub(/\s+/, "")
来源：http://orc.fktsv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://awk.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://xsy.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://icg.zhoulong.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://trw.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://azf.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://qqj.hammf.cn

Java: String.format("%03d", 7)
来源：http://zdw.gzhubu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://piy.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lxe.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pnp.zhixingplan.top

[E11] 反转字符串
来源：http://fmf.guowangkeji.top

Py:   s[::-1]
来源：http://ted.jyoumei.cn

PHP:  strrev($s);
来源：http://ncd.yfazqb.com

JS:   [...s].reverse().join("")
来源：http://xsa.havefunace.top

TS:   [...s].reverse().join("")
来源：http://uif.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kxa.hnxiangtu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://phx.yuxming.cn

Ruby: s.reverse
来源：http://idy.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://rjb.yj20258888.top

[E12] 统计某字符出现次数
来源：http://nzx.andypj.xyz

Py:   s.count("a")
来源：http://qxj.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://jqh.xuanzx.com

JS:   s.split("a").length - 1
来源：http://yqs.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://gyv.snrcjt.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yjx.jiagoushi.top

Go:   strings.Count(s, "a")
来源：http://owr.dashuyun.cn

Ruby: s.count("a")
来源：http://fyk.gogol.net.cn

C#:   s.Count(c => c == 'a')
来源：http://lnx.316326.xyz

[E13] 逐字符遍历
来源：http://bmk.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://tmj.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bus.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hyh.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bbm.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ahq.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ihr.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sqx.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://itv.jianghu66.top

[E14] URL 编码与 Base64
来源：http://pao.hysaishi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ulz.jyoumei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://txz.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xkj.gzhubu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vtx.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://llw.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jlf.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pup.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qwg.daxiang520.top

[E15] HTML 转义 / 反转义
来源：http://nql.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iwu.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vqh.shanyushiyangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gob.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ayq.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nmq.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rgu.ybcxt.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pbn.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://btv.jinyuanbaomall.cn

[E16] 数字千分位
来源：http://fyi.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://bkq.nanxinkj.top

PHP:  number_format(1234567);
来源：http://zdt.fanxiaobao.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://jxb.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://apk.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gyr.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://svk.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gku.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://wpx.snrcjt.cn

[E17] 首字母大写
来源：http://zuz.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ecw.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://eeq.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ruu.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xxo.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://epk.yj20258.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kmu.shzxlz.cn

Ruby: s.capitalize
来源：http://wnw.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fcx.jinyuanbaomall.cn

[E18] 模板占位符替换
来源：http://wnu.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://atj.316326.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ybh.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bgw.jyoumei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pld.ppjwa.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vgy.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bmk.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bpw.fanxiaobao.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qfr.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://awj.shangyingyoupin.top

Py:   s.splitlines()
来源：http://fbr.quarkkingdee.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tzv.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://oeb.jiagoushi.top

TS:   s.split(/\r?\n/)
来源：http://wyf.yj202588.top

Java: s.lines().toList()
来源：http://tlk.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://iru.snrcjt.cn

Ruby: s.lines
来源：http://vbg.hysaishi.cn

C#:   s.Split('\n')
来源：http://ycc.cheryme.top

[E20] 判断字符串是否为空
来源：http://wwq.chenjidiqi.icu

Py:   if not s:
来源：http://vab.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qem.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tgm.yfazqb.com

TS:   if (s === "") {}
来源：http://wqf.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://pzt.tian-w.cn

Go:   if s == "" {}
来源：http://vyb.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://jfi.tanke756.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://byr.cheryme.top

[E21] 超长截断加省略号
来源：http://rsn.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pbm.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jzs.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://adk.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oyo.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://psn.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://fqw.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rbk.jinqigufen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://srq.yvedp.cn

[E22] 字节长度与字符长度
来源：http://rhx.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qas.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bni.316326.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dxa.tanke756.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sfw.gzhubu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zxg.havefunace.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oit.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://iva.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hed.birdmap.top

================================================================================
来源：http://slb.ybcxt.top

F. 文件与目录
来源：http://ajn.gzhubu.top

================================================================================
来源：http://alp.ydzc1.top

[F01] 读取整个文件
来源：http://ihr.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://irn.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://vdt.hysaishi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://afj.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qsq.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kkc.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kdb.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://xrl.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://dvi.cucudq.cn

[F02] 逐行读取文件
来源：http://ngk.ybcxt.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ceb.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dfe.ywan-chungtsiang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tqe.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lyx.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pka.shanyushiyangtech.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vtt.vqdsnc.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nhd.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://chw.9152youxi.cn

[F03] 写入文件（覆盖）
来源：http://lwn.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vhv.jyoumei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://elw.zdbjq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jlx.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wsn.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xdx.ydzc1.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gon.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://ypk.fehbvm.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qua.hysaishi.cn

[F04] 追加写入文件
来源：http://wuy.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lff.zhengqikj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kya.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gth.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ian.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vbh.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cmu.c1oappe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iov.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fcf.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://ymt.nanxuanxn.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ste.guannengcc.top

PHP:  file_exists("a.txt");
来源：http://vpt.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://cpf.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://twc.kuanghao11.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xrl.yongpay.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kpf.yongpay.top

Ruby: File.exist?("a.txt")
来源：http://dgs.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://xhi.fanxiaobao.xyz

[F06] 删除文件
来源：http://gvh.cheryme.top

Py:   os.remove("a.txt")
来源：http://khf.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://vqw.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://blf.cashguo.top

TS:   fs.unlinkSync("a.txt")
来源：http://bgl.vqdsnc.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tlm.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://pta.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://mcx.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://rol.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://tfw.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://srp.cheryme.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dwk.nanxinkj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dqr.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jnq.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iyu.yj20258888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://crq.tanke756.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://adz.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://njd.nanxinkj.top

[F08] 遍历目录
来源：http://mny.yj20258.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cja.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qha.tianlin.xyz

JS:   fs.readdirSync("dir")
来源：http://dbc.cqqwz.cn

TS:   fs.readdirSync("dir")
来源：http://sgc.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://usq.yonumen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://slb.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://cus.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://ctp.zhixingplan.top

[F09] 获取文件大小
来源：http://dzf.shzxlz.cn

Py:   os.path.getsize("a.txt")
来源：http://wkc.xziqi.cn

PHP:  filesize("a.txt");
来源：http://dsu.vehdjk.com

JS:   fs.statSync("a.txt").size
来源：http://muy.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://kaj.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://xuw.0kj1m.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bzd.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://mtp.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://rpv.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://zoc.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aqp.jqgfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fgu.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://maf.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://iua.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qpr.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ylt.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://enk.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rmp.jinqigufen.top

[F11] 复制与移动文件
来源：http://qmb.fanxiaobao.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uke.zdqjudy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zjc.gzhubu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vho.shuidangran.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fhj.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ecu.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bxq.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lqy.cdnleiting.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ldp.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://pew.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jgz.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uxi.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jke.svipenyu.cn

TS:   // 同上
来源：http://ozj.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lnb.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uss.zhixingplan.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xmj.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://owv.yfazqb.com

================================================================================
来源：http://uua.yanxiufei.cn

G. 面向对象
来源：http://mnd.yanxiufei.cn

================================================================================
来源：http://mod.haohaochexian.top

[G01] 定义类
来源：http://tym.hcnkem.com

Py:   class User: pass
来源：http://ylk.zhaomingkeji.xyz

PHP:  class User {}
来源：http://gpi.zdqjudy.top

JS:   class User {}
来源：http://bqu.uphjek.com

TS:   class User { name: string = ""; }
来源：http://qnb.gotoacloud.top

Java: class User {}
来源：http://bgn.yuanzhike.top

Go:   type User struct { Name string }
来源：http://gyj.vqdsnc.cn

Ruby: class User; end
来源：http://ooy.hcnkem.com

C#:   class User {}
来源：http://xfg.yueranfly.top

[G02] 构造函数
来源：http://vga.shangyingyoupin.top

Py:   def __init__(self, name): self.name = name
来源：http://fvi.zhiwuduotai.top

PHP:  public function __construct(public string $name) {}
来源：http://bpu.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://xxt.wangdashe.top

TS:   constructor(public name: string) {}
来源：http://mge.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://our.yfazqb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lin.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://jwf.zycfv.cn


<!-- 参考信息 -->