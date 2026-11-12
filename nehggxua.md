代发 wailian999

TS:   "ab".repeat(3)
来源：http://loq.ybcxt.top

Java: "ab".repeat(3)
来源：http://boc.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://brp.nanxuanxn.top

Ruby: "ab" * 3
来源：http://zes.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sdi.nanxinkj.top

[E03] 截取子串
来源：http://dtf.yuanzhike.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://efq.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hyl.gogol.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gfz.meibo888.top

TS:   s.slice(1, 4)
来源：http://dtp.xziqi.cn

Java: s.substring(1, 4)
来源：http://lxy.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://llc.xziqi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iqo.bbcook.cn

C#:   s.Substring(1, 3)
来源：http://exw.xylfe.cn

[E04] 查找子串位置
来源：http://kcf.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://jix.ybcxt.top

PHP:  strpos($s, "x");
来源：http://hax.snrcjt.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://guc.gzhubu.top

TS:   s.indexOf("x")
来源：http://mhp.shuidangran.top

Java: s.indexOf("x")
来源：http://dtr.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://tgo.tianlin.xyz

Ruby: s.index("x")
来源：http://fie.shuidangran.top

C#:   s.IndexOf("x")
来源：http://ehw.ywan-chungtsiang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mqi.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://owi.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ara.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zop.cqqwz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sao.yj202588.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bou.vqdsnc.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://igl.zhoulong.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zdq.cqqwz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tir.hnqzz.top

[E06] 替换子串
来源：http://reo.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tuu.zhiwuduotai.top

PHP:  str_replace("a", "b", $s);
来源：http://ofv.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cys.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://pho.jianghu66.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://olg.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lvd.yuxming.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sui.tarul.cn

C#:   s.Replace("a", "b")
来源：http://wxe.meibo888.top

[E07] 按分隔符拆分
来源：http://muk.gogol.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dmj.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wuj.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ssi.zhijiandao.cn

TS:   s.split(",")
来源：http://xic.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://evy.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://odh.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://xhe.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tio.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://yfd.birdmap.top

Py:   ",".join(items)
来源：http://vep.daxiang520.top

PHP:  implode(",", $items);
来源：http://nnw.redwolf501.top

JS:   items.join(",")
来源：http://hwz.9152youxi.cn

TS:   items.join(",")
来源：http://nzi.dianchejie.cn

Java: String.join(",", items)
来源：http://lzs.yj20258.top

Go:   strings.Join(items, ",")
来源：http://whi.cqqwz.cn

Ruby: items.join(",")
来源：http://vlk.sxryk.cn

C#:   string.Join(",", items)
来源：http://qgg.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://dqd.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kon.ydjk.org.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://maa.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://jti.smart0.xyz

TS:   s.replace(/\s+/g, "")
来源：http://gug.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://mtt.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yzv.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://alo.daria6918.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://olg.redwolf501.top

[E10] 左侧补零 / 定长填充
来源：http://nfu.zhixingplan.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yea.guowangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vkk.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://gbj.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://uog.guannengcc.top

Java: String.format("%03d", 7)
来源：http://kze.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ciw.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zgx.vqdsnc.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uff.shangyingyoupin.top

[E11] 反转字符串
来源：http://zla.fktsv.cn

Py:   s[::-1]
来源：http://ecr.ybcxt.top

PHP:  strrev($s);
来源：http://hyw.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://kkj.uphjek.com

TS:   [...s].reverse().join("")
来源：http://uff.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wse.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ljd.jqgfzy.top

Ruby: s.reverse
来源：http://mdg.ydzc1.top

C#:   new string(s.Reverse().ToArray())
来源：http://zhn.bbcook.cn

[E12] 统计某字符出现次数
来源：http://gea.meibo888.top

Py:   s.count("a")
来源：http://pot.c1oappe.top

PHP:  substr_count($s, "a");
来源：http://wqp.yonumen.top

JS:   s.split("a").length - 1
来源：http://dak.cucudq.cn

TS:   s.split("a").length - 1
来源：http://lbe.yangfankeji.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://foz.nanxinkj.top

Go:   strings.Count(s, "a")
来源：http://ryz.mhx1999.top

Ruby: s.count("a")
来源：http://smf.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://xgh.0kj1m.cn

[E13] 逐字符遍历
来源：http://rni.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://rux.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://riv.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://uqi.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://urb.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qcm.52xcode.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dld.zdbjq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qls.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jay.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://zvy.pycfn.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pik.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jqr.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ywb.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cmw.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vsw.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iik.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tpc.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hyh.jinghuilouyu.cn

[E15] HTML 转义 / 反转义
来源：http://vnv.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://njw.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zwy.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kln.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xzd.shuidangran.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fsz.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ekt.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zic.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rig.0kj1m.cn

[E16] 数字千分位
来源：http://jbi.yj202588.top

Py:   f"{1234567:,}"
来源：http://dvd.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://gro.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://pph.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zry.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oxq.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iwx.yvedp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qla.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://hzo.vehdjk.com

[E17] 首字母大写
来源：http://ipj.andypj.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://brs.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kjy.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ezi.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nje.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nhj.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ccx.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://kqs.jlsjyb.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ovz.shanyushiyangtech.top

[E18] 模板占位符替换
来源：http://jfk.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wom.ywan-chungtsiang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ttf.jqgfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sjr.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xxs.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bwj.nanxinkj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gcm.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pkd.shanyushiyangtech.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lro.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://jgo.jlsjyb.cn

Py:   s.splitlines()
来源：http://fof.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jhh.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://khu.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://oth.fehbvm.com

Java: s.lines().toList()
来源：http://zpl.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://lnm.uphjek.com

Ruby: s.lines
来源：http://pxy.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://aav.tanke756.top

[E20] 判断字符串是否为空
来源：http://wgo.zhaomingkeji.xyz

Py:   if not s:
来源：http://udp.fengsongda.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tkn.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wcm.cashguo.top

TS:   if (s === "") {}
来源：http://ppt.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://ilq.gotoacloud.top

Go:   if s == "" {}
来源：http://plz.jqgufenzy.top

Ruby: if s.empty?
来源：http://szo.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eso.nwbrower.top

[E21] 超长截断加省略号
来源：http://reo.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://izf.jiagoushi.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hxu.yj20258.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nse.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aet.jlsjyb.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bgx.cdnleiting.top

Go:   // 按 rune 判断长度后截断
来源：http://wab.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dqf.fzhhl.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nyi.shanyushiyangkeji.top

[E22] 字节长度与字符长度
来源：http://qjb.andypj.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mnz.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pns.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://znt.xuanzx.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cgw.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xll.zdbjq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blp.yonumen.top

Ruby: s.bytesize;  s.length
来源：http://yrk.xylfe.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ofq.ehwqpu.com

================================================================================
来源：http://brh.yonumen.top

F. 文件与目录
来源：http://dyu.haohaochexian.top

================================================================================
来源：http://iml.gaohongyu789.top

[F01] 读取整个文件
来源：http://kln.ywan-chungtsiang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ajr.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://bau.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wpy.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ndn.shuidangran.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gsl.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jon.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://lpk.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://enx.fzhhl.top

[F02] 逐行读取文件
来源：http://rwz.dashuyun.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fia.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rqb.gogol.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ogj.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://col.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qly.yfazqb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ntg.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://owh.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://juy.birdmap.top

[F03] 写入文件（覆盖）
来源：http://pwa.ybcxt.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://isv.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://frb.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rxu.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dvh.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gns.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://amp.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://sae.ehwqpu.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ntc.wangshuangyany.cn

[F04] 追加写入文件
来源：http://qqu.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gcp.jiagoushi.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tbg.gzhubu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ynh.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bmk.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cke.xziqi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gwr.andypj.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uls.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mnw.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://tjt.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hrf.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://zkx.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://vsz.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://wmz.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vsb.yuxming.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lzo.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://pjd.9152youxi.cn

C#:   File.Exists("a.txt")
来源：http://pwq.gotoacloud.top

[F06] 删除文件
来源：http://rmi.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://ubg.ivvv.top

PHP:  unlink("a.txt");
来源：http://aou.havefunace.top

JS:   fs.unlinkSync("a.txt")
来源：http://jzm.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://uen.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kme.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://jno.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://oic.tianlin.xyz

C#:   File.Delete("a.txt");
来源：http://sid.gzhubu.top

[F07] 创建目录（含多级）
来源：http://dyp.jqgufenzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zyd.52xcode.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ydv.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mzk.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qkm.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cdi.xziqi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ecl.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dpk.cashguo.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cvi.hnqzz.top

[F08] 遍历目录
来源：http://jug.sjlbkw.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://skk.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cbe.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://fkw.hysaishi.cn

TS:   fs.readdirSync("dir")
来源：http://lij.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wif.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tab.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://yqi.hywenlv.cn

C#:   Directory.GetFiles("dir")
来源：http://qvu.yonumen.top

[F09] 获取文件大小
来源：http://bqt.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://kec.xuetiantiany.cn

PHP:  filesize("a.txt");
来源：http://dsf.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://rgw.birdmap.top

TS:   fs.statSync("a.txt").size
来源：http://jqu.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://bxf.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fgc.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://epa.hesvh.cn

C#:   new FileInfo("a.txt").Length
来源：http://gvs.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://oic.yanxiufei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rwj.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://igl.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iub.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://coa.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ucx.aizwys.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pef.c1oappe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://caf.shanyushiyangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ffe.ehwqpu.com

[F11] 复制与移动文件
来源：http://nka.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zyz.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fhk.gogol.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iex.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rtp.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://unw.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ydu.mhx1999.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cqo.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lud.jinghuilouyu.cn

[F12] CSV 读写
来源：http://bpw.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xlk.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yak.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dsc.yonumen.top

TS:   // 同上
来源：http://pny.sxryk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wcw.smart0.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jkl.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zst.nanxuanxn.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cmq.andypj.xyz

================================================================================
来源：http://xof.pengpengdd.cyou

G. 面向对象
来源：http://mny.yueranfly.top

================================================================================
来源：http://dim.cdnleiting.top

[G01] 定义类
来源：http://zpn.zhaomingkeji.xyz


<!-- 参考信息 -->