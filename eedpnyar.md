代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fpj.ywan-chungtsiang.top

TS:   s.slice(1, 4)
来源：http://fyg.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://hwa.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zwm.yanxiufei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mvh.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://cgq.birdmap.top

[E04] 查找子串位置
来源：http://mxg.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://mgf.gzhubu.top

PHP:  strpos($s, "x");
来源：http://rhe.aibaodan.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yht.yj20258888.top

TS:   s.indexOf("x")
来源：http://dtu.sxryk.cn

Java: s.indexOf("x")
来源：http://dto.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://vur.nwbrower.top

Ruby: s.index("x")
来源：http://icg.andypj.xyz

C#:   s.IndexOf("x")
来源：http://cat.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://udc.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kik.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cda.tanke756.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uvh.jianghu66.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ova.birdmap.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bxu.daria6918.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ksm.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eqg.cashguo.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gwn.bjfxy.top

[E06] 替换子串
来源：http://lua.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jlq.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://nsy.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dns.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://wxt.yuanzhike.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bfg.cucudq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zwu.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kjq.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://rwm.wangdashe.top

[E07] 按分隔符拆分
来源：http://znm.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oxb.jinghuilouyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gwn.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://itk.sjlbkw.cn

TS:   s.split(",")
来源：http://ian.shuidangran.top

Java: s.split(",");  s.split("\\s+")
来源：http://acw.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qfu.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://byi.jinqigufen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oxd.svipenyu.cn

[E08] 数组按分隔符合并
来源：http://yxr.daxiang520.top

Py:   ",".join(items)
来源：http://yuf.fktsv.cn

PHP:  implode(",", $items);
来源：http://cxc.yfazqb.com

JS:   items.join(",")
来源：http://nms.kuanghao11.cn

TS:   items.join(",")
来源：http://qjf.zhongyouzk.top

Java: String.join(",", items)
来源：http://lxs.jiagoushi.top

Go:   strings.Join(items, ",")
来源：http://rav.chenlongwang.top

Ruby: items.join(",")
来源：http://row.yj20258888.top

C#:   string.Join(",", items)
来源：http://avn.xinyue.icu

[E09] 去除所有空白字符
来源：http://wwo.snrcjt.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wvn.yj202588.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yik.c1oappe.top

JS:   s.replace(/\s+/g, "")
来源：http://rpf.yongpay.top

TS:   s.replace(/\s+/g, "")
来源：http://cqd.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://jvv.xuetiantiany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mpl.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://gkc.dashuyun.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vcd.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://yiy.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rvf.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pff.nanxuanxn.top

JS:   "7".padStart(3, "0")
来源：http://dgq.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://wpv.gotoacloud.top

Java: String.format("%03d", 7)
来源：http://wqi.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://izh.xingfuxueyuan.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rgg.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lqy.yangfankeji.com

[E11] 反转字符串
来源：http://zqy.vehdjk.com

Py:   s[::-1]
来源：http://vcj.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://vsx.feifeiyinyue.top

JS:   [...s].reverse().join("")
来源：http://row.jyoumei.cn

TS:   [...s].reverse().join("")
来源：http://zce.yuanzhike.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kan.daxiang520.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ukj.iojbl.cn

Ruby: s.reverse
来源：http://zkv.shangyingyoupin.top

C#:   new string(s.Reverse().ToArray())
来源：http://acx.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://fck.iojbl.cn

Py:   s.count("a")
来源：http://ora.shanyushiyangkeji.top

PHP:  substr_count($s, "a");
来源：http://nbg.cheryme.top

JS:   s.split("a").length - 1
来源：http://zdq.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://cmv.xuanzx.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xre.tianlin.xyz

Go:   strings.Count(s, "a")
来源：http://fov.dianchejie.cn

Ruby: s.count("a")
来源：http://lis.tarul.cn

C#:   s.Count(c => c == 'a')
来源：http://ebi.pycfn.com

[E13] 逐字符遍历
来源：http://fih.sysykeji.top

Py:   for ch in s: print(ch)
来源：http://xsh.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aij.yangfankeji.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ekd.pycfn.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://jby.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://avk.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fjw.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://keh.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vvu.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://kvl.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://twf.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bhv.andypj.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://trn.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jkw.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zfj.hywenlv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qiq.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oyh.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uyh.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://kki.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ufx.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dxg.redwolf501.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bxt.ctjpmb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://fqc.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://psd.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kls.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rae.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sbh.andypj.xyz

[E16] 数字千分位
来源：http://cgr.fktsv.cn

Py:   f"{1234567:,}"
来源：http://tox.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://ebm.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mga.guannengcc.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kwa.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lji.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wzu.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uch.yj20258.top

C#:   1234567.ToString("N0")
来源：http://wvx.ctjpmb.com

[E17] 首字母大写
来源：http://wjy.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nws.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hzf.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iom.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yze.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xrp.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sdi.zhongyouzk.top

Ruby: s.capitalize
来源：http://yyz.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rxr.yvedp.cn

[E18] 模板占位符替换
来源：http://nkp.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cmj.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bfh.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://zwk.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://czr.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nfj.ybcxt.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qym.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fei.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fhv.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://dkb.tarul.cn

Py:   s.splitlines()
来源：http://gzo.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jdp.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://xdy.vehdjk.com

TS:   s.split(/\r?\n/)
来源：http://rpx.tian-w.cn

Java: s.lines().toList()
来源：http://rgd.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://vgh.sysykeji.top

Ruby: s.lines
来源：http://dcb.bjfxy.top

C#:   s.Split('\n')
来源：http://nys.shuidangran.top

[E20] 判断字符串是否为空
来源：http://czy.hfpthk.cn

Py:   if not s:
来源：http://pwy.hnxiangtu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rco.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aic.hcnkem.com

TS:   if (s === "") {}
来源：http://iyw.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://kwa.sufxvd.cn

Go:   if s == "" {}
来源：http://asc.hnqzz.top

Ruby: if s.empty?
来源：http://eyo.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jwm.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://rjr.yuxming.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bit.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uod.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xvc.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cme.yj20258888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://drw.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://ovw.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bfk.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bog.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://kkq.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://klk.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jfa.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xjg.shuidangran.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://urw.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wsr.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jpl.svipenyu.cn

Ruby: s.bytesize;  s.length
来源：http://anl.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uhp.aibaodan.cn

================================================================================
来源：http://kkt.hesvh.cn

F. 文件与目录
来源：http://wnd.ydzc1.top

================================================================================
来源：http://ftn.fktsv.cn

[F01] 读取整个文件
来源：http://zgi.jinyuanbaomall.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rvl.cashguo.top

PHP:  file_get_contents("a.txt");
来源：http://joh.hfpthk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://man.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eic.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://vmg.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qvb.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://xpq.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://poc.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://jsx.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ezm.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vpd.xingfuxueyuan.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xsh.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kah.zdqjudy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xmo.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://omp.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hre.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ytb.yvedp.cn

[F03] 写入文件（覆盖）
来源：http://stf.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rry.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xwm.jyoumei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zuj.wangdashe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sts.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uxx.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vvr.xuetiantiany.cn

Ruby: File.write("a.txt", "hi")
来源：http://kph.yj20258888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://awg.zhijiandao.cn

[F04] 追加写入文件
来源：http://trq.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bld.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jpf.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jou.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ebc.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rci.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wpq.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hba.jinqigfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pjc.hywenlv.cn

[F05] 判断文件或目录是否存在
来源：http://atq.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hch.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://gmb.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://eoz.xziqi.cn

TS:   fs.existsSync("a.txt")
来源：http://rjv.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vfk.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zjj.gzhubu.top

Ruby: File.exist?("a.txt")
来源：http://mem.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://fua.hysaishi.cn

[F06] 删除文件
来源：http://dhh.dashuyun.cn

Py:   os.remove("a.txt")
来源：http://kmi.yj202588.top

PHP:  unlink("a.txt");
来源：http://otp.xinyue.icu

JS:   fs.unlinkSync("a.txt")
来源：http://xfy.ydjk.org.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vha.yj20258888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ngt.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://wso.zhengqikj.top

Ruby: File.delete("a.txt")
来源：http://ted.vehdjk.com

C#:   File.Delete("a.txt");
来源：http://qpb.xziqi.cn

[F07] 创建目录（含多级）
来源：http://fab.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qfc.kuanghao11.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sra.wangshuangyany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lff.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nao.yj20258888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dpw.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://avl.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yyp.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.zycfv.cn

[F08] 遍历目录
来源：http://fpu.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zis.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://crq.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://spa.hnqzz.top

TS:   fs.readdirSync("dir")
来源：http://iwa.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ogk.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kal.wangdashe.top

Ruby: Dir.children("dir")
来源：http://yav.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://pjv.bbcook.cn

[F09] 获取文件大小
来源：http://dum.mhx1999.top

Py:   os.path.getsize("a.txt")
来源：http://wix.xylfe.cn

PHP:  filesize("a.txt");
来源：http://bey.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://mvq.shangyingyoupin.top

TS:   fs.statSync("a.txt").size
来源：http://fko.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://bmq.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xeb.yvedp.cn

Ruby: File.size("a.txt")
来源：http://xpx.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://fne.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://hiu.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://raq.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dwm.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lxi.fengsongda.top

TS:   path.extname("a.txt")
来源：http://rhp.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pbc.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://quf.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eez.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rfp.zhixingplan.top

[F11] 复制与移动文件
来源：http://viq.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jpi.52xcode.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lom.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://shj.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pnf.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fxw.fzhhl.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://glu.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rsi.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qhj.tian-w.cn

[F12] CSV 读写
来源：http://gco.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://roa.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qan.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gzn.zhaomingkeji.xyz

TS:   // 同上
来源：http://ens.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kom.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://osg.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eyb.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pzu.hnqzz.top

================================================================================
来源：http://gzr.sysykeji.top

G. 面向对象
来源：http://xlt.316326.xyz

================================================================================
来源：http://iot.zhoulong.xyz

[G01] 定义类
来源：http://usd.zhoulong.xyz

Py:   class User: pass
来源：http://eis.gogol.net.cn

PHP:  class User {}
来源：http://ocr.hongshengwenyu.top

JS:   class User {}
来源：http://jku.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://lbq.ydjk.org.cn

Java: class User {}
来源：http://pra.bjfxy.top

Go:   type User struct { Name string }
来源：http://ynt.sweek.top

Ruby: class User; end
来源：http://ezf.nanxuanxn.top

C#:   class User {}
来源：http://rsq.bjfxy.top


<!-- 参考信息 -->