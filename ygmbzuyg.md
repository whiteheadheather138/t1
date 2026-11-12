代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jqk.52xcode.cn

[E03] 截取子串
来源：http://lrf.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iqv.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cdj.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dus.xuanzx.com

TS:   s.slice(1, 4)
来源：http://vet.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://qcd.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kgj.hongshengwenyu.top

Ruby: s[1, 3];  s[1..3]
来源：http://nnu.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://eku.dianchejie.cn

[E04] 查找子串位置
来源：http://wjn.jqgfzy.top

Py:   s.find("x");  s.index("x")
来源：http://dvm.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://evl.jinqigufen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yqd.shzxlz.cn

TS:   s.indexOf("x")
来源：http://ixx.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://pgq.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://atq.ydzc1.top

Ruby: s.index("x")
来源：http://ton.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://pbb.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://nuv.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tow.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oxd.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pqm.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jeb.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zjd.tian-w.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sso.xziqi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dgz.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dtc.nwbrower.top

[E06] 替换子串
来源：http://bwm.vqdsnc.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://syt.quarkkingdee.top

PHP:  str_replace("a", "b", $s);
来源：http://nsq.aibaodan.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vxa.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://kfr.kuanghao11.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://alu.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wps.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vwb.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://whc.ehwqpu.com

[E07] 按分隔符拆分
来源：http://foi.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://geb.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gkh.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://thf.hnqzz.top

TS:   s.split(",")
来源：http://lzt.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uni.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xum.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://hmu.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gwq.smart0.xyz

[E08] 数组按分隔符合并
来源：http://soa.wangdashe.top

Py:   ",".join(items)
来源：http://ice.xuanzx.com

PHP:  implode(",", $items);
来源：http://les.daria6918.cn

JS:   items.join(",")
来源：http://vww.sxryk.cn

TS:   items.join(",")
来源：http://ova.ehwqpu.com

Java: String.join(",", items)
来源：http://sye.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://hwh.meibo888.top

Ruby: items.join(",")
来源：http://yyn.jqgfzy.top

C#:   string.Join(",", items)
来源：http://vpi.ehwqpu.com

[E09] 去除所有空白字符
来源：http://qtl.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wbc.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dez.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://usm.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://plq.guannengcc.top

Java: s.replaceAll("\\s+", "")
来源：http://nvg.gaohongyu789.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xls.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://exa.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wqd.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://zzb.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://exa.quarkkingdee.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yhr.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://ycb.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://jug.yongpay.top

Java: String.format("%03d", 7)
来源：http://sqv.zhaomingkeji.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://hyz.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://avl.zhijiandao.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://spq.nanxuanxn.top

[E11] 反转字符串
来源：http://ojt.shanyushiyangtech.top

Py:   s[::-1]
来源：http://uel.nanxuanxn.top

PHP:  strrev($s);
来源：http://dhm.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://hkd.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://sdn.guowangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zkf.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qnc.yueranfly.top

Ruby: s.reverse
来源：http://fmc.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://ykd.fengsongda.top

[E12] 统计某字符出现次数
来源：http://opm.wangdashe.top

Py:   s.count("a")
来源：http://hum.kuanghao11.cn

PHP:  substr_count($s, "a");
来源：http://vux.yonumen.top

JS:   s.split("a").length - 1
来源：http://orj.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://zkj.yfazqb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yen.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://lck.meibo888.top

Ruby: s.count("a")
来源：http://vmb.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://gxo.yueranfly.top

[E13] 逐字符遍历
来源：http://vav.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://nam.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nij.yj20258888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mgi.hongshengwenyu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://twu.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nku.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lqf.sxryk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ypw.xuetiantiany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hnl.birdmap.top

[E14] URL 编码与 Base64
来源：http://aky.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ydv.shanyushiyangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vlx.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://avi.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uhw.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qiu.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mfh.bbcook.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pdl.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://spk.kuanghao11.cn

[E15] HTML 转义 / 反转义
来源：http://ntt.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://tna.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://shd.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zzw.cqqwz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ugv.tianlin.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qif.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cyg.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wgo.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ouq.zycfv.cn

[E16] 数字千分位
来源：http://zwh.52xcode.cn

Py:   f"{1234567:,}"
来源：http://efy.zhijiandao.cn

PHP:  number_format(1234567);
来源：http://vif.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hbb.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rcd.shanyushiyangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hau.shangyingyoupin.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rso.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rlr.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://xeo.yj202588.top

[E17] 首字母大写
来源：http://ebj.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://abr.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tlm.uphjek.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dat.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tue.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vlc.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dfy.zhoulong.xyz

Ruby: s.capitalize
来源：http://tlk.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cbq.aizwys.cn

[E18] 模板占位符替换
来源：http://sbr.ivvv.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fsq.fehbvm.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xdd.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lbd.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hrt.ydzc1.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ooi.cheryme.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rlx.yuxming.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oby.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hiv.hesvh.cn

[E19] 多行文本按行拆分
来源：http://hvn.havefunace.top

Py:   s.splitlines()
来源：http://xtz.meibo888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://djw.feifeiyinyue.top

JS:   s.split(/\r?\n/)
来源：http://toi.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://doe.tianlin.xyz

Java: s.lines().toList()
来源：http://cii.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://vkj.jqgufenzy.top

Ruby: s.lines
来源：http://upu.gzhubu.top

C#:   s.Split('\n')
来源：http://bgn.sxryk.cn

[E20] 判断字符串是否为空
来源：http://qrx.ydjk.org.cn

Py:   if not s:
来源：http://xjs.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://esk.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://frl.aibaodan.cn

TS:   if (s === "") {}
来源：http://ydr.zhaomingkeji.xyz

Java: if (s.isEmpty()) {}
来源：http://maa.c1oappe.top

Go:   if s == "" {}
来源：http://rfm.bjfxy.top

Ruby: if s.empty?
来源：http://vnb.aizwys.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zue.yj20258.top

[E21] 超长截断加省略号
来源：http://axy.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ous.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ymt.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zfw.gotoacloud.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hhu.havefunace.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://itw.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://mao.bbcook.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qka.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://azo.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://tqg.mhx1999.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rjt.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://byy.ywan-chungtsiang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ffv.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zcm.chenlongwang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lri.jqgufenzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vaf.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://hge.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qdh.cdnleiting.top

================================================================================
来源：http://qes.hongshengwenyu.top

F. 文件与目录
来源：http://wcc.hywenlv.cn

================================================================================
来源：http://jtg.uphjek.com

[F01] 读取整个文件
来源：http://cnr.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dyf.ehwqpu.com

PHP:  file_get_contents("a.txt");
来源：http://uzt.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kmr.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zph.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://wrh.hnxiangtu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://njl.ybcxt.top

Ruby: File.read("a.txt")
来源：http://coz.fengsongda.top

C#:   File.ReadAllText("a.txt");
来源：http://svz.ydjk.org.cn

[F02] 逐行读取文件
来源：http://twd.vehdjk.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bqa.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vnf.daxiang520.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wib.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zer.xingfuxueyuan.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rgc.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qje.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oji.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://scv.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://jqc.ppjwa.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eaf.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fjo.xuanzx.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xnv.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lwc.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zfe.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://etf.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://wih.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zoq.ybcxt.top

[F04] 追加写入文件
来源：http://tkm.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aur.gaohongyu789.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iyj.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ewn.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jge.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qzf.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wol.svipenyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cuo.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bpc.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://orc.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ruz.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://bbq.guannengcc.top

JS:   fs.existsSync("a.txt")
来源：http://lop.quarkkingdee.top

TS:   fs.existsSync("a.txt")
来源：http://ppm.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://zil.wangdashe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lmb.cheryme.top

Ruby: File.exist?("a.txt")
来源：http://ayv.bbcook.cn

C#:   File.Exists("a.txt")
来源：http://gez.0kj1m.cn

[F06] 删除文件
来源：http://usx.jiagoushi.top

Py:   os.remove("a.txt")
来源：http://wzf.gaohongyu789.top

PHP:  unlink("a.txt");
来源：http://gtz.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://qru.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://ruw.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ese.ybcxt.top

Go:   os.Remove("a.txt")
来源：http://dvq.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://zso.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://nbh.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://lsu.yj202588.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://grq.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nwv.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pfb.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vlb.tian-w.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yud.yueranfly.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fpz.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ufw.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kbk.daxiang520.top

[F08] 遍历目录
来源：http://zou.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gbx.fktsv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zuc.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://bqx.cqqwz.cn

TS:   fs.readdirSync("dir")
来源：http://lbv.ctjpmb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mek.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://led.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://ene.hongshengwenyu.top

C#:   Directory.GetFiles("dir")
来源：http://akg.jyoumei.cn

[F09] 获取文件大小
来源：http://rpz.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://rtn.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://zne.yfazqb.com

JS:   fs.statSync("a.txt").size
来源：http://kdr.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://qgy.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://blh.yj20258888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kpw.yvedp.cn

Ruby: File.size("a.txt")
来源：http://tgl.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://ffb.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://llw.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lzt.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iaw.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rov.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://ntd.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://txz.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kjs.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oks.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qik.quarkkingdee.top

[F11] 复制与移动文件
来源：http://fhm.zhoulong.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mts.c1oappe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cfq.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wfp.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aur.meibo888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ddb.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ruz.cqqwz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://spu.andypj.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eyt.sxryk.cn

[F12] CSV 读写
来源：http://sbl.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nyt.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tpc.jlsjyb.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bya.aibaodan.cn

TS:   // 同上
来源：http://iyu.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iuz.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bmb.nanxinkj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ttw.pengpengdd.cyou

C#:   // 无内置：用 CsvHelper 库
来源：http://nvp.havefunace.top

================================================================================
来源：http://mfm.yuxming.cn

G. 面向对象
来源：http://heq.uphjek.com

================================================================================
来源：http://keu.xuetiantiany.cn

[G01] 定义类
来源：http://apd.nwbrower.top

Py:   class User: pass
来源：http://ykt.zhongyouzk.top

PHP:  class User {}
来源：http://fvm.gotoacloud.top

JS:   class User {}
来源：http://vhd.daria6918.cn

TS:   class User { name: string = ""; }
来源：http://ebl.cdnleiting.top


<!-- 参考信息 -->