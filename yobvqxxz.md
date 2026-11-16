代发 wailian999

TS:   "ab".repeat(3)
来源：http://cwt.redwolf501.top

Java: "ab".repeat(3)
来源：http://sfn.shanyushiyangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://map.yanxiufei.cn

Ruby: "ab" * 3
来源：http://sgc.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ygx.gotoacloud.top

[E03] 截取子串
来源：http://shp.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ljw.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vjh.hnqzz.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vuc.yj20258888.top

TS:   s.slice(1, 4)
来源：http://oss.snrcjt.cn

Java: s.substring(1, 4)
来源：http://mbz.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mdz.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jpi.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://bna.xuanzx.com

[E04] 查找子串位置
来源：http://avt.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://mdj.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://tvq.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wpl.bbcook.cn

TS:   s.indexOf("x")
来源：http://whf.9152youxi.cn

Java: s.indexOf("x")
来源：http://owi.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://gay.aizwys.cn

Ruby: s.index("x")
来源：http://lqb.jinghuilouyu.cn

C#:   s.IndexOf("x")
来源：http://mxq.zhaomingkeji.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://ecm.pengpengdd.cyou

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bek.cheryme.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hau.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xmr.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iae.guowangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hkm.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gul.cqqwz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wxn.9152youxi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hxe.fehbvm.com

[E06] 替换子串
来源：http://ksl.xuanzx.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iko.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://qvw.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jmk.svipenyu.cn

TS:   s.replaceAll("a", "b")
来源：http://zkc.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kdi.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ggl.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nuy.zhijiandao.cn

C#:   s.Replace("a", "b")
来源：http://nbd.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://wai.jiagoushi.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qgw.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fwp.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wvd.guowangkeji.top

TS:   s.split(",")
来源：http://kkl.yuxming.cn

Java: s.split(",");  s.split("\\s+")
来源：http://msz.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jav.dianchejie.cn

Ruby: s.split(",");  s.split
来源：http://vxw.shanyushiyangtech.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qhy.zycfv.cn

[E08] 数组按分隔符合并
来源：http://kwe.ywan-chungtsiang.top

Py:   ",".join(items)
来源：http://okc.zhixingplan.top

PHP:  implode(",", $items);
来源：http://wjt.0kj1m.cn

JS:   items.join(",")
来源：http://nrm.haohaochexian.top

TS:   items.join(",")
来源：http://ibf.hysaishi.cn

Java: String.join(",", items)
来源：http://iqa.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://gth.jqgufenzy.top

Ruby: items.join(",")
来源：http://ohr.nanxinkj.top

C#:   string.Join(",", items)
来源：http://cfm.yfazqb.com

[E09] 去除所有空白字符
来源：http://eto.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tyo.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://frv.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://uji.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://zip.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://pws.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kkf.feifeiyinyue.top

Ruby: s.gsub(/\s+/, "")
来源：http://cxt.pengpengdd.cyou

C#:   Regex.Replace(s, @"\s+", "")
来源：http://egi.mhx1999.top

[E10] 左侧补零 / 定长填充
来源：http://fad.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mpu.sjlbkw.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wyg.vehdjk.com

JS:   "7".padStart(3, "0")
来源：http://fsm.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://yvk.tianlin.xyz

Java: String.format("%03d", 7)
来源：http://wso.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://tbl.wangshuangyany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pvj.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://are.nanxinkj.top

[E11] 反转字符串
来源：http://tbc.daxiang520.top

Py:   s[::-1]
来源：http://djn.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://ohj.shanyushiyangkeji.top

JS:   [...s].reverse().join("")
来源：http://sro.cashguo.top

TS:   [...s].reverse().join("")
来源：http://bkr.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ysj.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://epx.havefunace.top

Ruby: s.reverse
来源：http://bme.yj202588.top

C#:   new string(s.Reverse().ToArray())
来源：http://ajl.shzxlz.cn

[E12] 统计某字符出现次数
来源：http://ics.uphjek.com

Py:   s.count("a")
来源：http://stu.hnxiangtu.top

PHP:  substr_count($s, "a");
来源：http://zzw.hcnkem.com

JS:   s.split("a").length - 1
来源：http://nbr.c1oappe.top

TS:   s.split("a").length - 1
来源：http://wgn.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nfo.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://auo.sweek.top

Ruby: s.count("a")
来源：http://ztz.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://wbt.nwbrower.top

[E13] 逐字符遍历
来源：http://pvl.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://wpm.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dyq.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://eek.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://obs.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wqn.hfpthk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ffo.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sff.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sid.jinqigufen.top

[E14] URL 编码与 Base64
来源：http://fal.tianlin.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wrf.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://izm.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cfg.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://emj.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://llo.cheryme.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iep.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jmq.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mhe.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://esz.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zti.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yod.zhongyouzk.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oes.yongpay.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ruf.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://chy.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qed.ybcxt.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cdb.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bam.yuanzhike.top

[E16] 数字千分位
来源：http://xzx.daxiang520.top

Py:   f"{1234567:,}"
来源：http://xfn.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://afj.jqgfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://iun.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://jwh.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://url.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ptl.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ivd.jinqigufen.top

C#:   1234567.ToString("N0")
来源：http://ekq.hongshengwenyu.top

[E17] 首字母大写
来源：http://pft.hywenlv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://efc.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xef.yangfankeji.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qge.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qrl.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://psq.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wrj.quarkkingdee.top

Ruby: s.capitalize
来源：http://uqo.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mkf.hfpthk.cn

[E18] 模板占位符替换
来源：http://mcu.jqgfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://awx.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hki.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hwy.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kbl.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jvq.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nvu.xuetiantiany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://knf.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zqk.ydzc1.top

[E19] 多行文本按行拆分
来源：http://cym.dashuyun.cn

Py:   s.splitlines()
来源：http://ogb.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qxj.birdmap.top

JS:   s.split(/\r?\n/)
来源：http://upq.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://byy.tian-w.cn

Java: s.lines().toList()
来源：http://wct.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://oyd.wangdashe.top

Ruby: s.lines
来源：http://zxj.zycfv.cn

C#:   s.Split('\n')
来源：http://itl.gaohongyu789.top

[E20] 判断字符串是否为空
来源：http://stm.zhixingplan.top

Py:   if not s:
来源：http://bmd.shangyingyoupin.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kxt.gogol.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ids.gogol.net.cn

TS:   if (s === "") {}
来源：http://sim.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://dtd.vqdsnc.cn

Go:   if s == "" {}
来源：http://fym.52xcode.cn

Ruby: if s.empty?
来源：http://ymi.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xoi.yuanzhike.top

[E21] 超长截断加省略号
来源：http://ppe.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kqk.pycfn.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yva.hammf.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xhd.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iqx.dianchejie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nwc.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://tiv.cheryme.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nho.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rwg.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://pyu.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dpr.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kpn.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oiq.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tzp.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tzp.yj20258888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ikt.gotoacloud.top

Ruby: s.bytesize;  s.length
来源：http://sgz.ehwqpu.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lfc.nanxinkj.top

================================================================================
来源：http://ffg.nanxinkj.top

F. 文件与目录
来源：http://ugl.shanyushiyangkeji.top

================================================================================
来源：http://irg.sxryk.cn

[F01] 读取整个文件
来源：http://jiq.vqdsnc.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fxm.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://lgd.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bro.cqqwz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ppm.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hou.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rjy.sxryk.cn

Ruby: File.read("a.txt")
来源：http://ndi.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://gkf.tian-w.cn

[F02] 逐行读取文件
来源：http://vqv.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ctd.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wzh.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bfo.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zpb.hongshengwenyu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dyk.feifeiyinyue.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ooi.shzxlz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://evo.wangdashe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wkd.yanxiufei.cn

[F03] 写入文件（覆盖）
来源：http://vpz.birdmap.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xfe.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nvq.yvedp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ejf.xylfe.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wvu.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ajo.chenlongwang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://srh.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://cty.sweek.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gyt.sjlbkw.cn

[F04] 追加写入文件
来源：http://ssa.yj202588.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fxr.9152youxi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cvk.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jnr.hongshengwenyu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ncv.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xoa.aibaodan.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://afp.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jli.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://flu.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://syt.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xxm.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://fnx.chenzaomai.com

JS:   fs.existsSync("a.txt")
来源：http://ban.jqgufenzy.top

TS:   fs.existsSync("a.txt")
来源：http://vyi.hesvh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dla.yuxming.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jyu.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://tam.tianlin.xyz

C#:   File.Exists("a.txt")
来源：http://bqd.zhongyouzk.top

[F06] 删除文件
来源：http://oeh.jqgufenzy.top

Py:   os.remove("a.txt")
来源：http://jwp.yj202588.top

PHP:  unlink("a.txt");
来源：http://pfv.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://yrp.jinqigufen.top

TS:   fs.unlinkSync("a.txt")
来源：http://urf.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://akw.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://xdj.yangfankeji.com

Ruby: File.delete("a.txt")
来源：http://zpm.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://upj.sxryk.cn

[F07] 创建目录（含多级）
来源：http://fgi.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rwu.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yix.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rkv.zhixingplan.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://itc.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dok.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tan.jlsjyb.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gxh.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wnv.jinqigufen.top

[F08] 遍历目录
来源：http://iba.sjlbkw.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xug.xziqi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jar.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://dol.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://dha.quarkkingdee.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kxz.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lum.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://urk.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://fsz.feifeiyinyue.top

[F09] 获取文件大小
来源：http://alx.sxryk.cn

Py:   os.path.getsize("a.txt")
来源：http://tpv.gzhubu.top

PHP:  filesize("a.txt");
来源：http://fmj.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://hxs.sweek.top

TS:   fs.statSync("a.txt").size
来源：http://fop.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://mrd.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ktp.fehbvm.com

Ruby: File.size("a.txt")
来源：http://ooy.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://ort.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://las.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zaj.svipenyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sbg.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://urk.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://uot.snrcjt.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sdy.pycfn.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wls.quarkkingdee.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nbe.zhongyouzk.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jrd.ehwqpu.com

[F11] 复制与移动文件
来源：http://tng.shuidangran.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vzj.zdbjq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vcs.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jpy.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xnw.yuxming.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ltx.aizwys.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dda.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xvm.zhongyouzk.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qjy.hcnkem.com

[F12] CSV 读写
来源：http://pgv.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://skz.daria6918.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://htx.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qqr.yonumen.top

TS:   // 同上
来源：http://uja.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://efg.wangdashe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ejk.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ypm.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pwu.meibo888.top

================================================================================
来源：http://loq.sysykeji.top

G. 面向对象
来源：http://pzy.jlsjyb.cn

================================================================================
来源：http://frr.yj202588.top

[G01] 定义类
来源：http://dhx.fzhhl.top


<!-- 参考信息 -->