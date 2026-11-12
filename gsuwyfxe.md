代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ppc.vqdsnc.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qbq.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hfg.aizwys.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ffs.aizwys.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oad.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lqa.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://umt.hesvh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://isw.yonumen.top

[E06] 替换子串
来源：http://hxu.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wsa.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://ypf.jinqigufen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sas.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://cfe.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ktl.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://euz.hesvh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://urw.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://dwo.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://mut.fengsongda.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gme.jlsjyb.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hpu.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zra.xuetiantiany.cn

TS:   s.split(",")
来源：http://vce.wangshuangyany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://adm.yfazqb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jqv.jqgfzy.top

Ruby: s.split(",");  s.split
来源：http://ojq.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rhp.tarul.cn

[E08] 数组按分隔符合并
来源：http://gvg.gzhubu.top

Py:   ",".join(items)
来源：http://kzi.yfazqb.com

PHP:  implode(",", $items);
来源：http://ihi.tarul.cn

JS:   items.join(",")
来源：http://tox.uphjek.com

TS:   items.join(",")
来源：http://qvb.sjlbkw.cn

Java: String.join(",", items)
来源：http://giz.nanxinkj.top

Go:   strings.Join(items, ",")
来源：http://sri.zhongyouzk.top

Ruby: items.join(",")
来源：http://zek.fzhhl.top

C#:   string.Join(",", items)
来源：http://kec.ivvv.top

[E09] 去除所有空白字符
来源：http://cjx.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ajs.iojbl.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mqp.daxiang520.top

JS:   s.replace(/\s+/g, "")
来源：http://gcc.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://myt.snrcjt.cn

Java: s.replaceAll("\\s+", "")
来源：http://zoe.haohaochexian.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gyo.ydzc1.top

Ruby: s.gsub(/\s+/, "")
来源：http://lwp.wangshuangyany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jzr.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://bjz.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ysu.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oti.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://ibn.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://vvz.yonumen.top

Java: String.format("%03d", 7)
来源：http://eco.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://irm.svipenyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vnf.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qnn.sufxvd.cn

[E11] 反转字符串
来源：http://qld.shangyingyoupin.top

Py:   s[::-1]
来源：http://dli.zhengqikj.top

PHP:  strrev($s);
来源：http://enh.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://exc.xylfe.cn

TS:   [...s].reverse().join("")
来源：http://xoq.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://clk.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nty.xingfuxueyuan.xyz

Ruby: s.reverse
来源：http://gci.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uaf.sweek.top

[E12] 统计某字符出现次数
来源：http://bnk.aizwys.cn

Py:   s.count("a")
来源：http://vdq.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://suv.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://wke.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://qkf.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yje.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://tkx.sweek.top

Ruby: s.count("a")
来源：http://xrp.zhengqikj.top

C#:   s.Count(c => c == 'a')
来源：http://kmb.jyoumei.cn

[E13] 逐字符遍历
来源：http://lrp.yanxiufei.cn

Py:   for ch in s: print(ch)
来源：http://cly.yueranfly.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mqr.sxryk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jxp.zdbjq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://klf.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qin.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tue.zhiwuduotai.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xns.xuetiantiany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ikb.uphjek.com

[E14] URL 编码与 Base64
来源：http://boz.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lok.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bxy.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zup.xuetiantiany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pok.xingfuxueyuan.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hct.vqdsnc.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ewq.0kj1m.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://scw.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jwy.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://ycn.zdqjudy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xvm.yvedp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ndi.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://biu.sxryk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ies.sysykeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hsn.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tyr.shangyingyoupin.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jhg.316326.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://srb.wangshuangyany.cn

[E16] 数字千分位
来源：http://rwh.wangdashe.top

Py:   f"{1234567:,}"
来源：http://wzw.tarul.cn

PHP:  number_format(1234567);
来源：http://oby.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://igi.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mnx.tanke756.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fgs.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vxg.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nyh.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://izq.ehwqpu.com

[E17] 首字母大写
来源：http://rdq.fengsongda.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lwo.ybcxt.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gzd.yangfankeji.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ifu.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://upy.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://daz.pycfn.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://txr.shuidangran.top

Ruby: s.capitalize
来源：http://slz.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tuu.shzxlz.cn

[E18] 模板占位符替换
来源：http://vfg.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zij.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rzc.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bll.wangdashe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lve.hesvh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gge.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rxe.9152youxi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tre.gogol.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ucw.hesvh.cn

[E19] 多行文本按行拆分
来源：http://ljf.bjfxy.top

Py:   s.splitlines()
来源：http://woe.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wih.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://sbg.cashguo.top

TS:   s.split(/\r?\n/)
来源：http://lkj.jinqigfzy.top

Java: s.lines().toList()
来源：http://hrd.zdqjudy.top

Go:   strings.Split(s, "\n")
来源：http://lym.tarul.cn

Ruby: s.lines
来源：http://qpf.andypj.xyz

C#:   s.Split('\n')
来源：http://tbv.yueranfly.top

[E20] 判断字符串是否为空
来源：http://ubb.nanxuanxn.top

Py:   if not s:
来源：http://heq.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ius.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lpa.ehwqpu.com

TS:   if (s === "") {}
来源：http://wbb.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://alo.cheryme.top

Go:   if s == "" {}
来源：http://ebi.yfazqb.com

Ruby: if s.empty?
来源：http://jdy.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://she.0kj1m.cn

[E21] 超长截断加省略号
来源：http://hws.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kwa.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ztp.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ptz.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://trl.jyoumei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ilh.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://byr.cqqwz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gph.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ywt.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://bhi.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ptl.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kfh.redwolf501.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://flw.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qff.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qgl.gotoacloud.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uof.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://qkr.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aso.zycfv.cn

================================================================================
来源：http://dgd.chenzaomai.com

F. 文件与目录
来源：http://odc.hongshengwenyu.top

================================================================================
来源：http://tmj.hnqzz.top

[F01] 读取整个文件
来源：http://aki.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nxm.9152youxi.cn

PHP:  file_get_contents("a.txt");
来源：http://xsy.jqgufenzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bju.yangfankeji.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xxm.hysaishi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dcy.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kpq.redwolf501.top

Ruby: File.read("a.txt")
来源：http://zqa.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://pin.dashuyun.cn

[F02] 逐行读取文件
来源：http://bid.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qpz.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gun.yongpay.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cwl.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gsz.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vca.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ejp.ybcxt.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qzb.xuetiantiany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dez.sweek.top

[F03] 写入文件（覆盖）
来源：http://tzd.hongshengwenyu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qhb.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bpi.havefunace.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jnh.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nwv.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://orb.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nsu.ywan-chungtsiang.top

Ruby: File.write("a.txt", "hi")
来源：http://hkl.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://und.jinqigfzy.top

[F04] 追加写入文件
来源：http://hbj.zhongyouzk.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ygs.sweek.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tgc.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mqd.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://adh.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vnh.zycfv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://adg.sufxvd.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gmh.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eid.quarkkingdee.top

[F05] 判断文件或目录是否存在
来源：http://gfe.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kes.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://okv.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://hca.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://jmm.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gjy.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cxo.bjfxy.top

Ruby: File.exist?("a.txt")
来源：http://snt.fengsongda.top

C#:   File.Exists("a.txt")
来源：http://bpo.zhongyouzk.top

[F06] 删除文件
来源：http://fnd.ywan-chungtsiang.top

Py:   os.remove("a.txt")
来源：http://ywm.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://pib.gotoacloud.top

JS:   fs.unlinkSync("a.txt")
来源：http://kbw.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://vji.xylfe.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xmi.gaohongyu789.top

Go:   os.Remove("a.txt")
来源：http://ftm.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://uci.tarul.cn

C#:   File.Delete("a.txt");
来源：http://xbd.shuidangran.top

[F07] 创建目录（含多级）
来源：http://nhf.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nqb.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jqz.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kik.gaohongyu789.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ydc.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xml.jinqigfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sex.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fht.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bhv.cheryme.top

[F08] 遍历目录
来源：http://pyh.sufxvd.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bxs.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fvn.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://uvi.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://srq.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dox.cheryme.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ufn.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://lau.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://uja.ppjwa.cn

[F09] 获取文件大小
来源：http://lrl.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://nds.bjfxy.top

PHP:  filesize("a.txt");
来源：http://cvh.hywenlv.cn

JS:   fs.statSync("a.txt").size
来源：http://kxp.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://yyc.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://gvc.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fgr.yonumen.top

Ruby: File.size("a.txt")
来源：http://zdb.bbcook.cn

C#:   new FileInfo("a.txt").Length
来源：http://vcl.nwbrower.top

[F10] 取文件扩展名 / 文件名
来源：http://fop.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ujt.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xpo.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uxc.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://svg.daxiang520.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nyu.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xyg.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://owj.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wuw.cucudq.cn

[F11] 复制与移动文件
来源：http://bzq.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kdy.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gtl.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rjb.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nlf.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://efe.dashuyun.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kom.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ziy.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kjx.zdbjq.cn

[F12] CSV 读写
来源：http://upl.dianchejie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ubp.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lnn.jinqigufen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://voh.zycfv.cn

TS:   // 同上
来源：http://qlk.ctjpmb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://akb.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eil.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pwz.nanxuanxn.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ezz.ybcxt.top

================================================================================
来源：http://ost.chenzaomai.com

G. 面向对象
来源：http://hwy.pengpengdd.cyou

================================================================================
来源：http://agk.xylfe.cn

[G01] 定义类
来源：http://xtt.9152youxi.cn

Py:   class User: pass
来源：http://gzu.ydjk.org.cn

PHP:  class User {}
来源：http://mok.guannengcc.top

JS:   class User {}
来源：http://nrn.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://gwc.dianchejie.cn

Java: class User {}
来源：http://iex.hfpthk.cn

Go:   type User struct { Name string }
来源：http://mvg.hfpthk.cn

Ruby: class User; end
来源：http://dmi.mhx1999.top

C#:   class User {}
来源：http://vhl.0kj1m.cn

[G02] 构造函数
来源：http://yxg.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://wwy.chenlongwang.top

PHP:  public function __construct(public string $name) {}
来源：http://hcf.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://drn.wangdashe.top

TS:   constructor(public name: string) {}
来源：http://ldq.wangshuangyany.cn

Java: User(String name) { this.name = name; }
来源：http://cvl.cashguo.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gbr.hnxiangtu.top

Ruby: def initialize(name); @name = name; end
来源：http://qkw.nanxuanxn.top

C#:   public User(string name) { Name = name; }
来源：http://wtu.nwbrower.top

[G03] 实例属性
来源：http://jxr.andypj.xyz

Py:   self.name = "x"
来源：http://znv.yangfankeji.com

PHP:  public string $name = "x";
来源：http://efi.dashuyun.cn

JS:   this.name = "x";
来源：http://agx.zdbjq.cn

TS:   name: string = "x";
来源：http://nrh.gzhubu.top

Java: private String name;
来源：http://gwk.jinqigufen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fzu.zhixingplan.top


<!-- 参考信息 -->