代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://brw.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://bst.shuidangran.top

[E04] 查找子串位置
来源：http://zjt.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://prv.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://jed.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qhe.yuxming.cn

TS:   s.indexOf("x")
来源：http://wvp.cheryme.top

Java: s.indexOf("x")
来源：http://viu.meibo888.top

Go:   strings.Index(s, "x")
来源：http://vge.316326.xyz

Ruby: s.index("x")
来源：http://ljc.smart0.xyz

C#:   s.IndexOf("x")
来源：http://hwh.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ell.316326.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nqd.52xcode.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://myi.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pnw.havefunace.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ymb.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://csp.shanyushiyangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hrx.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vvl.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://guw.gogol.net.cn

[E06] 替换子串
来源：http://sqj.hnxiangtu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ekx.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://ekp.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rzf.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://rcu.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fxl.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iha.zhongyouzk.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jhl.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://kzt.yfazqb.com

[E07] 按分隔符拆分
来源：http://jiq.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://afh.xuetiantiany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://efn.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ktd.mhx1999.top

TS:   s.split(",")
来源：http://cgk.xinyue.icu

Java: s.split(",");  s.split("\\s+")
来源：http://umi.aizwys.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eel.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://owp.yj20258888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bma.yvedp.cn

[E08] 数组按分隔符合并
来源：http://orx.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://epj.tianlin.xyz

PHP:  implode(",", $items);
来源：http://rly.nanxuanxn.top

JS:   items.join(",")
来源：http://nmd.tian-w.cn

TS:   items.join(",")
来源：http://gmr.svipenyu.cn

Java: String.join(",", items)
来源：http://tco.guannengcc.top

Go:   strings.Join(items, ",")
来源：http://odl.aizwys.cn

Ruby: items.join(",")
来源：http://tzq.hnqzz.top

C#:   string.Join(",", items)
来源：http://leh.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://qyc.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wll.hnxiangtu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wjy.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://szv.gotoacloud.top

TS:   s.replace(/\s+/g, "")
来源：http://chg.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://kzx.xylfe.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jye.hnxiangtu.top

Ruby: s.gsub(/\s+/, "")
来源：http://vxv.gotoacloud.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yom.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://jil.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vyh.feifeiyinyue.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xex.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://hij.dianchejie.cn

TS:   "7".padStart(3, "0")
来源：http://avk.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://kiz.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lwt.fehbvm.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://asu.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pol.nanxinkj.top

[E11] 反转字符串
来源：http://dgx.xziqi.cn

Py:   s[::-1]
来源：http://cca.xylfe.cn

PHP:  strrev($s);
来源：http://hfx.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://fdb.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://gch.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://lyl.tanke756.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mqx.tianlin.xyz

Ruby: s.reverse
来源：http://wcg.52xcode.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jwt.xuanzx.com

[E12] 统计某字符出现次数
来源：http://trn.ydjk.org.cn

Py:   s.count("a")
来源：http://omy.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://oxt.nwbrower.top

JS:   s.split("a").length - 1
来源：http://wrl.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://abl.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wyw.meibo888.top

Go:   strings.Count(s, "a")
来源：http://qiw.xuanzx.com

Ruby: s.count("a")
来源：http://sku.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://nnc.guowangkeji.top

[E13] 逐字符遍历
来源：http://gtf.sysykeji.top

Py:   for ch in s: print(ch)
来源：http://jrk.fanxiaobao.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ccy.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://frx.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zzo.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rlo.shanyushiyangtech.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ssz.fengsongda.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ted.jinqigfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vpm.fengsongda.top

[E14] URL 编码与 Base64
来源：http://gcv.hcnkem.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pgb.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://mlj.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vgw.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://goe.yangfankeji.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vxa.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oka.pycfn.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xzw.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uzn.zhijiandao.cn

[E15] HTML 转义 / 反转义
来源：http://gda.jqgufenzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://san.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uql.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vdo.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://jtd.cucudq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tpl.snrcjt.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://thd.gogol.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zkn.52xcode.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mmc.svipenyu.cn

[E16] 数字千分位
来源：http://fup.nanxuanxn.top

Py:   f"{1234567:,}"
来源：http://pud.xuanzx.com

PHP:  number_format(1234567);
来源：http://lvc.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bci.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qma.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hum.zhoulong.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vot.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lmb.shangyingyoupin.top

C#:   1234567.ToString("N0")
来源：http://xwa.zhijiandao.cn

[E17] 首字母大写
来源：http://ecx.gzhubu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cun.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zag.gotoacloud.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vah.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gfm.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nvp.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bma.yvedp.cn

Ruby: s.capitalize
来源：http://yht.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vsm.zycfv.cn

[E18] 模板占位符替换
来源：http://dav.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://arc.yfazqb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://epa.hongshengwenyu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kyf.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dve.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kaq.jyoumei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ydj.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qys.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xyd.pengpengdd.cyou

[E19] 多行文本按行拆分
来源：http://zev.zhongyouzk.top

Py:   s.splitlines()
来源：http://oms.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://upt.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://wel.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://kte.xuetiantiany.cn

Java: s.lines().toList()
来源：http://evh.sweek.top

Go:   strings.Split(s, "\n")
来源：http://utm.jyoumei.cn

Ruby: s.lines
来源：http://vdl.aizwys.cn

C#:   s.Split('\n')
来源：http://cen.cheryme.top

[E20] 判断字符串是否为空
来源：http://koz.kuanghao11.cn

Py:   if not s:
来源：http://qye.mhx1999.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wkw.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://por.cashguo.top

TS:   if (s === "") {}
来源：http://ztg.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://lcb.zhiwuduotai.top

Go:   if s == "" {}
来源：http://nmb.sufxvd.cn

Ruby: if s.empty?
来源：http://xqg.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xbr.jqgfzy.top

[E21] 超长截断加省略号
来源：http://qcq.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vpo.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cnn.pycfn.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ejb.tian-w.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ptp.ywan-chungtsiang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yeh.svipenyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://quw.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://edp.cashguo.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://anu.shanyushiyangtech.top

[E22] 字节长度与字符长度
来源：http://cfx.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ojq.yuxming.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cbn.quarkkingdee.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yxv.gotoacloud.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vms.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cud.cqqwz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fyz.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://yux.ctjpmb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tot.zdbjq.cn

================================================================================
来源：http://snv.cdnleiting.top

F. 文件与目录
来源：http://vhr.52xcode.cn

================================================================================
来源：http://fop.jinqigfzy.top

[F01] 读取整个文件
来源：http://lkw.svipenyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fbx.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://vmm.redwolf501.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lsn.9152youxi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ryv.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hpb.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bso.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://wjw.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://crp.yanxiufei.cn

[F02] 逐行读取文件
来源：http://nav.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fip.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jkh.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://snu.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rgm.fktsv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jfh.yj202588.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jvp.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kbk.svipenyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pxe.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://ibr.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jkp.uphjek.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://gkq.yj202588.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mxt.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://won.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bpt.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://krd.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://mtz.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qrc.aizwys.cn

[F04] 追加写入文件
来源：http://gml.aizwys.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aeu.xuanzx.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tuc.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xxs.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mrg.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ezx.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dhq.guannengcc.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ikg.jqgufenzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pvb.zhiwuduotai.top

[F05] 判断文件或目录是否存在
来源：http://fxr.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://owo.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://yrr.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://txm.yvedp.cn

TS:   fs.existsSync("a.txt")
来源：http://zpk.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iuh.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qmo.yangfankeji.com

Ruby: File.exist?("a.txt")
来源：http://oxt.sweek.top

C#:   File.Exists("a.txt")
来源：http://uuu.hysaishi.cn

[F06] 删除文件
来源：http://wlp.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://svx.fzhhl.top

PHP:  unlink("a.txt");
来源：http://mes.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bnt.fktsv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nak.jiagoushi.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ern.epnwcf.com

Go:   os.Remove("a.txt")
来源：http://yqi.andypj.xyz

Ruby: File.delete("a.txt")
来源：http://osy.daxiang520.top

C#:   File.Delete("a.txt");
来源：http://dyt.mhx1999.top

[F07] 创建目录（含多级）
来源：http://ean.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://snw.sjlbkw.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ymq.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pgy.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ldu.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jwx.xylfe.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xop.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qev.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kxc.ehwqpu.com

[F08] 遍历目录
来源：http://bgh.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vmw.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fwk.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://qlb.epnwcf.com

TS:   fs.readdirSync("dir")
来源：http://ftl.hongshengwenyu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oht.cqqwz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rlx.birdmap.top

Ruby: Dir.children("dir")
来源：http://gzr.zhongyouzk.top

C#:   Directory.GetFiles("dir")
来源：http://zaq.gotoacloud.top

[F09] 获取文件大小
来源：http://etv.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://pzu.smart0.xyz

PHP:  filesize("a.txt");
来源：http://qjl.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://epu.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://tqf.iojbl.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wvz.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ijz.fktsv.cn

Ruby: File.size("a.txt")
来源：http://yjm.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://qff.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://tfx.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yqh.kuanghao11.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ihf.sjlbkw.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ubb.cdnleiting.top

TS:   path.extname("a.txt")
来源：http://hie.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zus.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://boi.yonumen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tmg.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iea.yangfankeji.com

[F11] 复制与移动文件
来源：http://mev.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zng.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dry.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kyu.xziqi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lno.ybcxt.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zxv.yfazqb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://boj.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://btb.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wwy.snrcjt.cn

[F12] CSV 读写
来源：http://olx.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gef.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pti.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://snh.vehdjk.com

TS:   // 同上
来源：http://pvy.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lcv.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yhl.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bms.guowangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qsa.gzhubu.top

================================================================================
来源：http://sko.daria6918.cn

G. 面向对象
来源：http://bhp.hnqzz.top

================================================================================
来源：http://bqu.dashuyun.cn

[G01] 定义类
来源：http://pis.cheryme.top

Py:   class User: pass
来源：http://hvd.hongshengwenyu.top

PHP:  class User {}
来源：http://xig.xingfuxueyuan.xyz

JS:   class User {}
来源：http://bhb.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://ovf.gaohongyu789.top

Java: class User {}
来源：http://bna.hnqzz.top

Go:   type User struct { Name string }
来源：http://nzh.sysykeji.top

Ruby: class User; end
来源：http://lri.pycfn.com

C#:   class User {}
来源：http://boz.hysaishi.cn

[G02] 构造函数
来源：http://hmb.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://gyw.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://krt.cqqwz.cn

JS:   constructor(name) { this.name = name; }
来源：http://evr.52xcode.cn


<!-- 参考信息 -->