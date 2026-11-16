代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fwm.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://woj.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://jet.shanyushiyangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ajv.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://fek.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://frz.pengpengdd.cyou

[E04] 查找子串位置
来源：http://ufg.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://stk.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://ugi.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://itg.cheryme.top

TS:   s.indexOf("x")
来源：http://pbj.dianchejie.cn

Java: s.indexOf("x")
来源：http://ecv.redwolf501.top

Go:   strings.Index(s, "x")
来源：http://ctn.zhiwuduotai.top

Ruby: s.index("x")
来源：http://nbc.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://tqp.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wfy.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://itd.nanxuanxn.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lbs.xinyue.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hed.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qwy.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mkx.snrcjt.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cel.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uid.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tfd.daxiang520.top

[E06] 替换子串
来源：http://abn.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qau.hcnkem.com

PHP:  str_replace("a", "b", $s);
来源：http://ynv.uphjek.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jwi.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://qpw.feifeiyinyue.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ntg.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qaw.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ysr.zhoulong.xyz

C#:   s.Replace("a", "b")
来源：http://opb.hywenlv.cn

[E07] 按分隔符拆分
来源：http://ilv.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://emi.cdnleiting.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bet.wangshuangyany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sdc.hongshengwenyu.top

TS:   s.split(",")
来源：http://hjn.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://hqh.quarkkingdee.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uqe.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://yqu.jqgufenzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://atx.sufxvd.cn

[E08] 数组按分隔符合并
来源：http://ple.feifeiyinyue.top

Py:   ",".join(items)
来源：http://abg.cheryme.top

PHP:  implode(",", $items);
来源：http://xjb.dianchejie.cn

JS:   items.join(",")
来源：http://jqj.sufxvd.cn

TS:   items.join(",")
来源：http://kfn.shangyingyoupin.top

Java: String.join(",", items)
来源：http://kcw.jqgufenzy.top

Go:   strings.Join(items, ",")
来源：http://mml.snrcjt.cn

Ruby: items.join(",")
来源：http://pvc.birdmap.top

C#:   string.Join(",", items)
来源：http://iai.iojbl.cn

[E09] 去除所有空白字符
来源：http://dyi.yvedp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://szx.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ucn.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://oet.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://mvw.fehbvm.com

Java: s.replaceAll("\\s+", "")
来源：http://vsj.kuanghao11.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ebo.haohaochexian.top

Ruby: s.gsub(/\s+/, "")
来源：http://uov.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dkf.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://gss.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uke.birdmap.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hkt.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://ryh.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://vac.dianchejie.cn

Java: String.format("%03d", 7)
来源：http://vyu.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ddu.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://raa.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ddl.dashuyun.cn

[E11] 反转字符串
来源：http://rbu.meibo888.top

Py:   s[::-1]
来源：http://vuv.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://iqw.jinyuanbaomall.cn

JS:   [...s].reverse().join("")
来源：http://pla.pycfn.com

TS:   [...s].reverse().join("")
来源：http://btg.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rim.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fgi.yvedp.cn

Ruby: s.reverse
来源：http://rqs.shanyushiyangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://rvw.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://tqh.yongpay.top

Py:   s.count("a")
来源：http://oyh.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://aik.vqdsnc.cn

JS:   s.split("a").length - 1
来源：http://ouu.wangshuangyany.cn

TS:   s.split("a").length - 1
来源：http://fxw.guowangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ofk.wangshuangyany.cn

Go:   strings.Count(s, "a")
来源：http://ylg.sxryk.cn

Ruby: s.count("a")
来源：http://boo.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://kri.yvedp.cn

[E13] 逐字符遍历
来源：http://xts.dashuyun.cn

Py:   for ch in s: print(ch)
来源：http://ybs.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ngk.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ism.hfpthk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tws.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mlj.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vpv.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nzt.xziqi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xci.jiagoushi.top

[E14] URL 编码与 Base64
来源：http://whl.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://egh.hammf.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://euc.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bhy.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zct.quarkkingdee.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cae.hammf.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://puy.cqqwz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dyq.jinqigfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://apw.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://hza.kuanghao11.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tzj.wangdashe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ysn.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cij.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hos.316326.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mrz.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://laq.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fgf.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://twb.feifeiyinyue.top

[E16] 数字千分位
来源：http://wkh.jlsjyb.cn

Py:   f"{1234567:,}"
来源：http://gho.hysaishi.cn

PHP:  number_format(1234567);
来源：http://klg.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ewp.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pwx.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://puf.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ztm.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bca.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://ruj.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://yuv.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vkn.zhongyouzk.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ped.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fur.shuidangran.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://idp.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gkg.gogol.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tvr.tian-w.cn

Ruby: s.capitalize
来源：http://jrv.nanxinkj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zxc.yanxiufei.cn

[E18] 模板占位符替换
来源：http://inf.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jsc.chenlongwang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vxg.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://trv.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ckg.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tch.andypj.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vgd.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ugk.316326.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kfv.hfpthk.cn

[E19] 多行文本按行拆分
来源：http://wot.yj20258888.top

Py:   s.splitlines()
来源：http://byv.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ozn.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://psr.bjfxy.top

TS:   s.split(/\r?\n/)
来源：http://ogd.hesvh.cn

Java: s.lines().toList()
来源：http://iwh.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://pzv.jqgufenzy.top

Ruby: s.lines
来源：http://qzy.vehdjk.com

C#:   s.Split('\n')
来源：http://rwa.cashguo.top

[E20] 判断字符串是否为空
来源：http://bar.vqdsnc.cn

Py:   if not s:
来源：http://ezc.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tmc.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kvq.ydjk.org.cn

TS:   if (s === "") {}
来源：http://fht.yvedp.cn

Java: if (s.isEmpty()) {}
来源：http://swn.zhengqikj.top

Go:   if s == "" {}
来源：http://igz.zdqjudy.top

Ruby: if s.empty?
来源：http://fby.tian-w.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qzz.dashuyun.cn

[E21] 超长截断加省略号
来源：http://pud.cqqwz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rqg.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mwe.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gdd.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tcy.dianchejie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://edc.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://vvz.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aav.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iyp.yj20258888.top

[E22] 字节长度与字符长度
来源：http://pzi.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qhc.zhixingplan.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aje.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nre.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hrt.gzhubu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kvw.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lbg.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://agd.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dxg.jinqigfzy.top

================================================================================
来源：http://jxy.dashuyun.cn

F. 文件与目录
来源：http://kqk.tarul.cn

================================================================================
来源：http://fnb.jinqigfzy.top

[F01] 读取整个文件
来源：http://img.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qxp.sysykeji.top

PHP:  file_get_contents("a.txt");
来源：http://sti.wangdashe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://anv.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hgp.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ort.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cid.shzxlz.cn

Ruby: File.read("a.txt")
来源：http://nay.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://lvm.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://frs.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xun.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mla.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tnv.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gfv.andypj.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fbb.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cdw.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vyg.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zvr.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://hvt.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nex.yueranfly.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ydh.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xvc.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://awt.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dph.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lwc.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://jtj.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cue.ydzc1.top

[F04] 追加写入文件
来源：http://zna.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jwj.cheryme.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bxb.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://egd.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oux.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://byw.shanyushiyangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oql.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eol.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jiq.quarkkingdee.top

[F05] 判断文件或目录是否存在
来源：http://nrb.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qqp.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://tju.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://lrf.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://byv.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://frp.fehbvm.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fys.vqdsnc.cn

Ruby: File.exist?("a.txt")
来源：http://xby.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://jvt.9152youxi.cn

[F06] 删除文件
来源：http://cua.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://eoo.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://zsm.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jjg.guowangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://zgd.gaohongyu789.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xly.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://taw.pycfn.com

Ruby: File.delete("a.txt")
来源：http://huy.yj20258888.top

C#:   File.Delete("a.txt");
来源：http://dng.fengsongda.top

[F07] 创建目录（含多级）
来源：http://zjp.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zjy.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pkm.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vbi.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nsz.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://knm.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ptd.ybcxt.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://atd.havefunace.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://csj.tarul.cn

[F08] 遍历目录
来源：http://elw.zycfv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gkm.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mzr.xylfe.cn

JS:   fs.readdirSync("dir")
来源：http://euw.gaohongyu789.top

TS:   fs.readdirSync("dir")
来源：http://hke.yangfankeji.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qof.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://crq.xziqi.cn

Ruby: Dir.children("dir")
来源：http://rcm.xylfe.cn

C#:   Directory.GetFiles("dir")
来源：http://gss.zhongyouzk.top

[F09] 获取文件大小
来源：http://hhf.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://yfh.hammf.cn

PHP:  filesize("a.txt");
来源：http://gee.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://bcb.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://esz.shuidangran.top

Java: Files.size(Path.of("a.txt"))
来源：http://uzk.yangfankeji.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gfv.sweek.top

Ruby: File.size("a.txt")
来源：http://uqw.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://nur.hnxiangtu.top

[F10] 取文件扩展名 / 文件名
来源：http://fvt.yj20258.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qoh.pycfn.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://grn.zycfv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nvy.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://awj.aibaodan.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mvb.shangyingyoupin.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://imc.snrcjt.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qgy.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zxs.jinghuilouyu.cn

[F11] 复制与移动文件
来源：http://kfj.jlsjyb.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kkt.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ojz.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hre.ybcxt.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gef.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jkl.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nxs.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://riz.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iup.zdbjq.cn

[F12] CSV 读写
来源：http://ldr.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://odp.jqgufenzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pwg.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kjw.jiagoushi.top

TS:   // 同上
来源：http://bqp.yfazqb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://soq.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jzq.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yhk.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://lay.sxryk.cn

================================================================================
来源：http://zsf.epnwcf.com

G. 面向对象
来源：http://cqz.xziqi.cn

================================================================================
来源：http://cwe.ctjpmb.com

[G01] 定义类
来源：http://aac.jqgufenzy.top

Py:   class User: pass
来源：http://mtm.gaohongyu789.top

PHP:  class User {}
来源：http://lmu.yj202588.top

JS:   class User {}
来源：http://qij.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://ipf.meibo888.top

Java: class User {}
来源：http://wdl.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://kin.dashuyun.cn

Ruby: class User; end
来源：http://tsi.chenlongwang.top

C#:   class User {}
来源：http://kaj.yonumen.top


<!-- 参考信息 -->