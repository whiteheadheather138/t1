代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://phw.yfazqb.com

C#:   s.Substring(1, 3)
来源：http://gqz.jianghu66.top

[E04] 查找子串位置
来源：http://gsy.guannengcc.top

Py:   s.find("x");  s.index("x")
来源：http://wis.hfpthk.cn

PHP:  strpos($s, "x");
来源：http://kis.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://djd.tanke756.top

TS:   s.indexOf("x")
来源：http://oql.guowangkeji.top

Java: s.indexOf("x")
来源：http://dir.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://adi.zhongyouzk.top

Ruby: s.index("x")
来源：http://hqm.yvedp.cn

C#:   s.IndexOf("x")
来源：http://dab.hysaishi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://itf.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zgx.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qgi.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pwj.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://igx.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zuo.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fxu.snrcjt.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ego.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qna.bjfxy.top

[E06] 替换子串
来源：http://wkj.chenlongwang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gch.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://qhs.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nol.cqqwz.cn

TS:   s.replaceAll("a", "b")
来源：http://tph.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://byo.birdmap.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bfb.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xuq.shangyingyoupin.top

C#:   s.Replace("a", "b")
来源：http://fwh.jinqigufen.top

[E07] 按分隔符拆分
来源：http://ibj.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mof.fzhhl.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bzo.jyoumei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://thb.yuanzhike.top

TS:   s.split(",")
来源：http://xtr.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://nap.svipenyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fql.fktsv.cn

Ruby: s.split(",");  s.split
来源：http://lun.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://quc.hnxiangtu.top

[E08] 数组按分隔符合并
来源：http://win.fzhhl.top

Py:   ",".join(items)
来源：http://qzi.guowangkeji.top

PHP:  implode(",", $items);
来源：http://epk.jlsjyb.cn

JS:   items.join(",")
来源：http://ibk.yj20258.top

TS:   items.join(",")
来源：http://yse.shanyushiyangkeji.top

Java: String.join(",", items)
来源：http://qhc.yj202588.top

Go:   strings.Join(items, ",")
来源：http://ish.yuanzhike.top

Ruby: items.join(",")
来源：http://zzn.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://tea.jianghu66.top

[E09] 去除所有空白字符
来源：http://wjw.daria6918.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qdr.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vsc.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://egq.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://ovq.cqqwz.cn

Java: s.replaceAll("\\s+", "")
来源：http://yoi.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sjn.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://yqh.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qgu.aibaodan.cn

[E10] 左侧补零 / 定长填充
来源：http://jwz.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://drc.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aux.dianchejie.cn

JS:   "7".padStart(3, "0")
来源：http://ifw.yj202588.top

TS:   "7".padStart(3, "0")
来源：http://eqc.yongpay.top

Java: String.format("%03d", 7)
来源：http://iub.nanxinkj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zwp.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dbn.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://moz.ehwqpu.com

[E11] 反转字符串
来源：http://slj.wangshuangyany.cn

Py:   s[::-1]
来源：http://xgx.jyoumei.cn

PHP:  strrev($s);
来源：http://sgq.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://cea.hywenlv.cn

TS:   [...s].reverse().join("")
来源：http://zrq.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vlq.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://koh.chenjidiqi.icu

Ruby: s.reverse
来源：http://beu.hnqzz.top

C#:   new string(s.Reverse().ToArray())
来源：http://zzx.ydzc1.top

[E12] 统计某字符出现次数
来源：http://tnu.c1oappe.top

Py:   s.count("a")
来源：http://xwx.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://pdb.andypj.xyz

JS:   s.split("a").length - 1
来源：http://qxh.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://qsh.yfazqb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xpt.yuxming.cn

Go:   strings.Count(s, "a")
来源：http://sjg.zhongyouzk.top

Ruby: s.count("a")
来源：http://cxy.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://bwe.chenzaomai.com

[E13] 逐字符遍历
来源：http://tkz.gzhubu.top

Py:   for ch in s: print(ch)
来源：http://fdu.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://waa.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://gvx.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uhw.ctjpmb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tee.andypj.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jmq.cashguo.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xxx.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yxl.smart0.xyz

[E14] URL 编码与 Base64
来源：http://cbq.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zee.chenjidiqi.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://syv.bjfxy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hbt.zhijiandao.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tnh.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hmf.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wyw.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xkh.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dyw.smart0.xyz

[E15] HTML 转义 / 反转义
来源：http://pzb.yj20258.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gyt.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://woa.cucudq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://agr.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://waz.sweek.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zyw.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vzb.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yud.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cqm.316326.xyz

[E16] 数字千分位
来源：http://jzf.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://cbd.mhx1999.top

PHP:  number_format(1234567);
来源：http://xgl.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qoa.cashguo.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qvo.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kua.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uxz.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fxa.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://qpc.yj20258.top

[E17] 首字母大写
来源：http://xzq.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wnu.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://wmj.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://npq.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mju.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mwn.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://daf.sufxvd.cn

Ruby: s.capitalize
来源：http://nrp.xuanzx.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xpt.chenzaomai.com

[E18] 模板占位符替换
来源：http://wge.fengsongda.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cnd.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hcz.svipenyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tvq.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gxi.hesvh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://krs.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zdp.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://flj.sjlbkw.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pjf.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://vbl.cashguo.top

Py:   s.splitlines()
来源：http://tti.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jot.jqgufenzy.top

JS:   s.split(/\r?\n/)
来源：http://yzm.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://cep.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://cjt.fzhhl.top

Go:   strings.Split(s, "\n")
来源：http://chv.ydjk.org.cn

Ruby: s.lines
来源：http://rqc.jianghu66.top

C#:   s.Split('\n')
来源：http://vun.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://hby.xuetiantiany.cn

Py:   if not s:
来源：http://jng.jlsjyb.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pse.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ibp.vehdjk.com

TS:   if (s === "") {}
来源：http://qab.jiagoushi.top

Java: if (s.isEmpty()) {}
来源：http://zzi.yuxming.cn

Go:   if s == "" {}
来源：http://cci.ctjpmb.com

Ruby: if s.empty?
来源：http://tol.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qmz.hfpthk.cn

[E21] 超长截断加省略号
来源：http://qrn.kuanghao11.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sas.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fyx.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nwy.316326.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iqk.dashuyun.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qyw.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://wiv.cashguo.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hdl.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ygy.cqqwz.cn

[E22] 字节长度与字符长度
来源：http://jxq.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ipt.zhixingplan.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lnt.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://btv.cdnleiting.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://raf.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sah.fengsongda.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wvx.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://zst.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wfj.gaohongyu789.top

================================================================================
来源：http://jej.wangdashe.top

F. 文件与目录
来源：http://gph.jqgufenzy.top

================================================================================
来源：http://szw.sxryk.cn

[F01] 读取整个文件
来源：http://hjb.yfazqb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rcx.kuanghao11.cn

PHP:  file_get_contents("a.txt");
来源：http://yuk.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wde.sysykeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ezi.jyoumei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vnx.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xre.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://rdu.cucudq.cn

C#:   File.ReadAllText("a.txt");
来源：http://vaq.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://ipy.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fzq.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xgv.wangdashe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://prn.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aew.xingfuxueyuan.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mtt.yuanzhike.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dkn.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ros.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qfr.vehdjk.com

[F03] 写入文件（覆盖）
来源：http://bjf.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vco.9152youxi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bvr.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tiy.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://coi.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dxn.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wtt.epnwcf.com

Ruby: File.write("a.txt", "hi")
来源：http://bnk.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dku.nanxuanxn.top

[F04] 追加写入文件
来源：http://xxw.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ddp.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sra.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mre.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yzs.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nwq.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dsb.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bza.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dcv.feifeiyinyue.top

[F05] 判断文件或目录是否存在
来源：http://qmz.hywenlv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iij.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://bdo.jinghuilouyu.cn

JS:   fs.existsSync("a.txt")
来源：http://njn.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://dah.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://llg.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jdw.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://sqx.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://btu.xuanzx.com

[F06] 删除文件
来源：http://fpc.bbcook.cn

Py:   os.remove("a.txt")
来源：http://vhw.yvedp.cn

PHP:  unlink("a.txt");
来源：http://egw.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zph.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hnr.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pvc.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://dun.zhoulong.xyz

Ruby: File.delete("a.txt")
来源：http://buq.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://xjs.zhaomingkeji.xyz

[F07] 创建目录（含多级）
来源：http://fjb.yongpay.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nif.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eob.sxryk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fyp.zhixingplan.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mxz.shuidangran.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ley.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jhr.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dip.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dvu.cqqwz.cn

[F08] 遍历目录
来源：http://jmh.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://atk.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zsy.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://wkn.epnwcf.com

TS:   fs.readdirSync("dir")
来源：http://wgb.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dpq.9152youxi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qve.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://zpy.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://wmx.gotoacloud.top

[F09] 获取文件大小
来源：http://mvj.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://mgi.yuxming.cn

PHP:  filesize("a.txt");
来源：http://mzy.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://otr.sweek.top

TS:   fs.statSync("a.txt").size
来源：http://wwa.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://vzx.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mew.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://xjn.epnwcf.com

C#:   new FileInfo("a.txt").Length
来源：http://heh.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://awm.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nqn.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ihd.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://riq.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://mlz.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zjc.0kj1m.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yev.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gqx.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kat.hesvh.cn

[F11] 复制与移动文件
来源：http://dow.yanxiufei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dbc.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kbh.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qih.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oof.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dys.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://afp.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bhn.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ccr.hnqzz.top

[F12] CSV 读写
来源：http://keo.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pce.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ach.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://url.jianghu66.top

TS:   // 同上
来源：http://yxb.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tst.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://div.zdbjq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://upq.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ftx.yuxming.cn

================================================================================
来源：http://zvp.aibaodan.cn

G. 面向对象
来源：http://cow.sufxvd.cn

================================================================================
来源：http://ugg.iojbl.cn

[G01] 定义类
来源：http://tjr.hcnkem.com

Py:   class User: pass
来源：http://ghe.shanyushiyangkeji.top

PHP:  class User {}
来源：http://idy.zhengqikj.top

JS:   class User {}
来源：http://cnw.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://pca.yonumen.top

Java: class User {}
来源：http://qal.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://dzo.pycfn.com

Ruby: class User; end
来源：http://bbd.tianlin.xyz

C#:   class User {}
来源：http://tms.9152youxi.cn

[G02] 构造函数
来源：http://bhw.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://jkx.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://rrs.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://nas.gaohongyu789.top


<!-- 参考信息 -->