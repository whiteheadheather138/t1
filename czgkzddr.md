代发 wailian999

PHP:  strpos($s, "x");
来源：http://mit.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://phu.redwolf501.top

TS:   s.indexOf("x")
来源：http://yna.pycfn.com

Java: s.indexOf("x")
来源：http://pcr.jinqigfzy.top

Go:   strings.Index(s, "x")
来源：http://oui.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://rvx.meibo888.top

C#:   s.IndexOf("x")
来源：http://jlr.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wja.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://izs.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yol.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lnj.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://zwa.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nyz.bbcook.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nuy.nanxinkj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://asb.mhx1999.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hzp.daria6918.cn

[E06] 替换子串
来源：http://tca.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ohf.tarul.cn

PHP:  str_replace("a", "b", $s);
来源：http://bxl.bjfxy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tkq.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://ewu.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xov.zhongyouzk.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zhd.316326.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://udu.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://pgd.52xcode.cn

[E07] 按分隔符拆分
来源：http://vik.jinyuanbaomall.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vhb.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qia.zdbjq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gpl.wangshuangyany.cn

TS:   s.split(",")
来源：http://rwj.vehdjk.com

Java: s.split(",");  s.split("\\s+")
来源：http://our.jqgfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dzd.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://rdb.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uxj.pycfn.com

[E08] 数组按分隔符合并
来源：http://ipj.9152youxi.cn

Py:   ",".join(items)
来源：http://eeq.0kj1m.cn

PHP:  implode(",", $items);
来源：http://oou.fengsongda.top

JS:   items.join(",")
来源：http://ldi.quarkkingdee.top

TS:   items.join(",")
来源：http://tol.guannengcc.top

Java: String.join(",", items)
来源：http://foz.yuxming.cn

Go:   strings.Join(items, ",")
来源：http://pjq.zhijiandao.cn

Ruby: items.join(",")
来源：http://irg.zhoulong.xyz

C#:   string.Join(",", items)
来源：http://ixj.sufxvd.cn

[E09] 去除所有空白字符
来源：http://oni.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kod.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ypm.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://rwt.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://crb.xingfuxueyuan.xyz

Java: s.replaceAll("\\s+", "")
来源：http://dls.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tmz.fanxiaobao.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://zll.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aim.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://xoq.wangshuangyany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mcy.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://znt.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://xxp.zhijiandao.cn

TS:   "7".padStart(3, "0")
来源：http://npo.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://uxh.jqgufenzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tik.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nqb.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vuz.ivvv.top

[E11] 反转字符串
来源：http://dbt.gotoacloud.top

Py:   s[::-1]
来源：http://nqe.ydjk.org.cn

PHP:  strrev($s);
来源：http://kih.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://tip.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://ule.redwolf501.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rrz.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://hnd.xziqi.cn

Ruby: s.reverse
来源：http://stb.uphjek.com

C#:   new string(s.Reverse().ToArray())
来源：http://otj.tanke756.top

[E12] 统计某字符出现次数
来源：http://pdv.cdnleiting.top

Py:   s.count("a")
来源：http://zjs.sweek.top

PHP:  substr_count($s, "a");
来源：http://tbv.wangdashe.top

JS:   s.split("a").length - 1
来源：http://qrn.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://wok.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wxs.meibo888.top

Go:   strings.Count(s, "a")
来源：http://eho.cheryme.top

Ruby: s.count("a")
来源：http://tda.tarul.cn

C#:   s.Count(c => c == 'a')
来源：http://gkt.xylfe.cn

[E13] 逐字符遍历
来源：http://mrm.9152youxi.cn

Py:   for ch in s: print(ch)
来源：http://mai.tarul.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jbz.jinyuanbaomall.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pag.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ait.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://guh.shanyushiyangtech.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rzc.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://imf.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://opc.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://tum.zdbjq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fzy.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iom.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ktl.xinyue.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aez.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tib.52xcode.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aro.ywan-chungtsiang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vyy.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vqs.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://bwx.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rok.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://air.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bqh.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jke.hnqzz.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vqi.yvedp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ewx.ybcxt.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qtd.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lny.yuxming.cn

[E16] 数字千分位
来源：http://uns.fehbvm.com

Py:   f"{1234567:,}"
来源：http://osy.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://yoo.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sjn.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jei.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lqm.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xgl.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://til.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://aye.mhx1999.top

[E17] 首字母大写
来源：http://msj.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fkw.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fdh.yonumen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rms.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fdi.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nih.jinyuanbaomall.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wfw.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://tru.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kda.xinyue.icu

[E18] 模板占位符替换
来源：http://exk.zhixingplan.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zrc.fktsv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hvs.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://aiv.jyoumei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://igh.wangshuangyany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sop.zhengqikj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cys.gogol.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cll.mhx1999.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xdg.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://bfn.gaohongyu789.top

Py:   s.splitlines()
来源：http://fhk.jinyuanbaomall.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pvj.hfpthk.cn

JS:   s.split(/\r?\n/)
来源：http://okw.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://vgr.aibaodan.cn

Java: s.lines().toList()
来源：http://exa.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://qax.jyoumei.cn

Ruby: s.lines
来源：http://nxk.tanke756.top

C#:   s.Split('\n')
来源：http://hoe.guannengcc.top

[E20] 判断字符串是否为空
来源：http://add.gaohongyu789.top

Py:   if not s:
来源：http://tac.cucudq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jrv.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ooj.bjfxy.top

TS:   if (s === "") {}
来源：http://xdo.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://lot.birdmap.top

Go:   if s == "" {}
来源：http://rii.daria6918.cn

Ruby: if s.empty?
来源：http://zia.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hhv.pycfn.com

[E21] 超长截断加省略号
来源：http://owm.ehwqpu.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hix.sweek.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sid.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zco.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cgw.jqgfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mdp.shanyushiyangtech.top

Go:   // 按 rune 判断长度后截断
来源：http://phe.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://puw.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pmc.c1oappe.top

[E22] 字节长度与字符长度
来源：http://gah.snrcjt.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xsp.quarkkingdee.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rqm.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rin.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mhs.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jyu.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bxy.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://bdy.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nhi.haohaochexian.top

================================================================================
来源：http://vub.pengpengdd.cyou

F. 文件与目录
来源：http://xaz.nanxinkj.top

================================================================================
来源：http://czj.vehdjk.com

[F01] 读取整个文件
来源：http://xgh.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://osv.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://eoz.fanxiaobao.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nsz.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rxp.andypj.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://rba.fktsv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://awx.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://igh.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://cgn.hysaishi.cn

[F02] 逐行读取文件
来源：http://akr.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pjt.ydzc1.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dnq.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oix.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://edg.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cgj.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bym.ctjpmb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://abi.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hiw.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://haw.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gom.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xgq.vehdjk.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://naj.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yem.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dae.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hoq.yj20258888.top

Ruby: File.write("a.txt", "hi")
来源：http://lrt.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ceq.wangdashe.top

[F04] 追加写入文件
来源：http://grs.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bbc.tarul.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bzw.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xjt.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hwu.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xvr.shanyushiyangtech.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nlh.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mha.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fcv.smart0.xyz

[F05] 判断文件或目录是否存在
来源：http://ehu.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nii.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://soq.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://tmo.andypj.xyz

TS:   fs.existsSync("a.txt")
来源：http://wbh.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dfh.ybcxt.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://abm.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://yko.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://tht.0kj1m.cn

[F06] 删除文件
来源：http://ksg.havefunace.top

Py:   os.remove("a.txt")
来源：http://cbe.xziqi.cn

PHP:  unlink("a.txt");
来源：http://gjb.zhaomingkeji.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://pmv.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wae.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xba.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://ulu.0kj1m.cn

Ruby: File.delete("a.txt")
来源：http://aii.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://haa.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://zii.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fec.kuanghao11.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xll.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tad.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xjz.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://elx.zhaomingkeji.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xyi.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://shb.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wez.guannengcc.top

[F08] 遍历目录
来源：http://kjn.xingfuxueyuan.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ulk.xuetiantiany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vty.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://mcx.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://lst.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jmb.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://xhs.birdmap.top

Ruby: Dir.children("dir")
来源：http://wja.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://yfq.cdnleiting.top

[F09] 获取文件大小
来源：http://hic.aibaodan.cn

Py:   os.path.getsize("a.txt")
来源：http://oxz.redwolf501.top

PHP:  filesize("a.txt");
来源：http://ntn.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://iwh.bbcook.cn

TS:   fs.statSync("a.txt").size
来源：http://vce.xuanzx.com

Java: Files.size(Path.of("a.txt"))
来源：http://thm.ivvv.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zbw.yj20258.top

Ruby: File.size("a.txt")
来源：http://trr.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://cbf.sweek.top

[F10] 取文件扩展名 / 文件名
来源：http://sko.tanke756.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ueg.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://alg.haohaochexian.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hmb.kuanghao11.cn

TS:   path.extname("a.txt")
来源：http://fdt.bjfxy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nkl.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zni.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uiy.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qpr.jinghuilouyu.cn

[F11] 复制与移动文件
来源：http://svp.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ykc.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fkq.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fyg.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aqa.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qwf.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rgd.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bip.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xcj.yonumen.top

[F12] CSV 读写
来源：http://bnf.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rqf.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qcy.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://elo.snrcjt.cn

TS:   // 同上
来源：http://erc.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vgm.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qtd.gogol.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://whj.chenjidiqi.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://qwq.shuidangran.top

================================================================================
来源：http://mjj.jyoumei.cn

G. 面向对象
来源：http://vzq.jinqigfzy.top

================================================================================
来源：http://nwm.kuanghao11.cn

[G01] 定义类
来源：http://eby.jinyuanbaomall.cn

Py:   class User: pass
来源：http://sef.shanyushiyangtech.top

PHP:  class User {}
来源：http://jwf.zhengqikj.top

JS:   class User {}
来源：http://pde.hnqzz.top

TS:   class User { name: string = ""; }
来源：http://hdh.jyoumei.cn

Java: class User {}
来源：http://lgw.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://yhd.tianlin.xyz

Ruby: class User; end
来源：http://cua.jiagoushi.top

C#:   class User {}
来源：http://kjn.yangfankeji.com

[G02] 构造函数
来源：http://esn.ivvv.top

Py:   def __init__(self, name): self.name = name
来源：http://xdl.zhongyouzk.top

PHP:  public function __construct(public string $name) {}
来源：http://yhi.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://arb.yangfankeji.com

TS:   constructor(public name: string) {}
来源：http://nxe.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://lrw.ybcxt.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uib.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://ffz.quarkkingdee.top


<!-- 参考信息 -->