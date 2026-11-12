代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://htx.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://php.cucudq.cn

Java: s.substring(1, 4)
来源：http://vna.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://meh.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://urk.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://ofi.c1oappe.top

[E04] 查找子串位置
来源：http://vuo.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://oro.zhiwuduotai.top

PHP:  strpos($s, "x");
来源：http://ylp.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tiy.c1oappe.top

TS:   s.indexOf("x")
来源：http://vrz.bjfxy.top

Java: s.indexOf("x")
来源：http://bzj.wangdashe.top

Go:   strings.Index(s, "x")
来源：http://rxj.c1oappe.top

Ruby: s.index("x")
来源：http://qmg.smart0.xyz

C#:   s.IndexOf("x")
来源：http://ucb.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://amn.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hvk.uphjek.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://czs.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lem.fanxiaobao.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://qbe.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yxp.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pxk.9152youxi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mre.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vog.yj20258.top

[E06] 替换子串
来源：http://znq.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://los.52xcode.cn

PHP:  str_replace("a", "b", $s);
来源：http://htv.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vhu.bbcook.cn

TS:   s.replaceAll("a", "b")
来源：http://sta.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://btr.shangyingyoupin.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tge.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fky.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://zyq.pycfn.com

[E07] 按分隔符拆分
来源：http://cbp.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xsi.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ama.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://ebc.yuanzhike.top

TS:   s.split(",")
来源：http://wgn.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sjl.ybcxt.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://odu.cheryme.top

Ruby: s.split(",");  s.split
来源：http://vuk.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://amq.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://qkb.meibo888.top

Py:   ",".join(items)
来源：http://sej.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://wbd.yueranfly.top

JS:   items.join(",")
来源：http://qfd.gaohongyu789.top

TS:   items.join(",")
来源：http://vmp.pengpengdd.cyou

Java: String.join(",", items)
来源：http://crh.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://xdx.zhoulong.xyz

Ruby: items.join(",")
来源：http://bkq.yj202588.top

C#:   string.Join(",", items)
来源：http://xkc.hnqzz.top

[E09] 去除所有空白字符
来源：http://jwh.guannengcc.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vly.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zcc.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://dbj.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://qpm.sweek.top

Java: s.replaceAll("\\s+", "")
来源：http://ilc.hywenlv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ult.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bla.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bgg.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://rzw.shanyushiyangtech.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bfc.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xgk.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://stn.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://uww.yvedp.cn

Java: String.format("%03d", 7)
来源：http://sbz.zhaomingkeji.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://pwf.ywan-chungtsiang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bls.wangshuangyany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iky.cqqwz.cn

[E11] 反转字符串
来源：http://rei.dianchejie.cn

Py:   s[::-1]
来源：http://jpk.fehbvm.com

PHP:  strrev($s);
来源：http://jsw.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://glq.uphjek.com

TS:   [...s].reverse().join("")
来源：http://jmz.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ead.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ugw.jyoumei.cn

Ruby: s.reverse
来源：http://nlu.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://irh.316326.xyz

[E12] 统计某字符出现次数
来源：http://fyn.xuanzx.com

Py:   s.count("a")
来源：http://ruk.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://arf.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://sdd.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://vcs.chenzaomai.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lzu.hammf.cn

Go:   strings.Count(s, "a")
来源：http://mxs.hywenlv.cn

Ruby: s.count("a")
来源：http://qst.fanxiaobao.xyz

C#:   s.Count(c => c == 'a')
来源：http://mju.haohaochexian.top

[E13] 逐字符遍历
来源：http://avf.shanyushiyangtech.top

Py:   for ch in s: print(ch)
来源：http://xzc.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uak.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yex.hywenlv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rwv.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iot.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pbp.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://pqk.jyoumei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xox.yueranfly.top

[E14] URL 编码与 Base64
来源：http://zcz.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gze.yangfankeji.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://fyq.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://emi.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vtn.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oyu.pycfn.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oop.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ara.xuanzx.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bcb.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://trt.ehwqpu.com

Py:   html.escape(s);  html.unescape(s)
来源：http://jab.ppjwa.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kso.bjfxy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lfj.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jph.ctjpmb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nnh.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://phm.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qyj.snrcjt.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dyx.yj20258888.top

[E16] 数字千分位
来源：http://pmz.mhx1999.top

Py:   f"{1234567:,}"
来源：http://vsr.aibaodan.cn

PHP:  number_format(1234567);
来源：http://mls.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wnb.bjfxy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ybh.jinyuanbaomall.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bua.kuanghao11.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://spr.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rib.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://isc.redwolf501.top

[E17] 首字母大写
来源：http://tml.nanxinkj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ofv.gzhubu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ezy.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gea.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sfh.hammf.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jzo.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qnt.gogol.net.cn

Ruby: s.capitalize
来源：http://zhz.cheryme.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ndj.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://mcd.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lrn.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ecd.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xpf.hnxiangtu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lvb.fzhhl.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hux.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://afz.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://clo.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://olu.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://sfn.zhoulong.xyz

Py:   s.splitlines()
来源：http://wyd.jianghu66.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lpq.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://ptw.hongshengwenyu.top

TS:   s.split(/\r?\n/)
来源：http://ndo.sufxvd.cn

Java: s.lines().toList()
来源：http://vet.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://dky.hongshengwenyu.top

Ruby: s.lines
来源：http://vtj.uphjek.com

C#:   s.Split('\n')
来源：http://ylf.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://ygq.zycfv.cn

Py:   if not s:
来源：http://mmg.nanxuanxn.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ytf.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://piy.tanke756.top

TS:   if (s === "") {}
来源：http://rdb.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://pvx.fehbvm.com

Go:   if s == "" {}
来源：http://wzf.guowangkeji.top

Ruby: if s.empty?
来源：http://tga.ehwqpu.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ujc.fengsongda.top

[E21] 超长截断加省略号
来源：http://xmo.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mxc.chenlongwang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://coq.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vce.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iij.fengsongda.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jih.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://unx.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aca.cqqwz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lvs.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://weo.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gid.zhixingplan.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cda.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lzp.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tom.sweek.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://afs.wangdashe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eny.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://xdq.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ppb.hongshengwenyu.top

================================================================================
来源：http://fwt.tarul.cn

F. 文件与目录
来源：http://wec.pycfn.com

================================================================================
来源：http://kvv.bbcook.cn

[F01] 读取整个文件
来源：http://dms.shanyushiyangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kcb.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://cer.andypj.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kko.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yip.hammf.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gti.aizwys.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ayd.yuanzhike.top

Ruby: File.read("a.txt")
来源：http://eck.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://hlr.c1oappe.top

[F02] 逐行读取文件
来源：http://rqr.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jjo.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kgm.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dhd.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tzd.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gyy.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eyy.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dfi.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://umd.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://olc.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wxs.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://tdd.zdbjq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vmq.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://anw.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eta.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oib.ctjpmb.com

Ruby: File.write("a.txt", "hi")
来源：http://hag.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lyf.shzxlz.cn

[F04] 追加写入文件
来源：http://ayk.ybcxt.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xon.jlsjyb.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fvu.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xtp.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hqe.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wnw.jqgfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://len.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rdf.snrcjt.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qhb.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://ryv.shzxlz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://afa.ehwqpu.com

PHP:  file_exists("a.txt");
来源：http://ult.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://hjt.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://qhb.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nzt.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pvc.cdnleiting.top

Ruby: File.exist?("a.txt")
来源：http://mio.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://scx.ydjk.org.cn

[F06] 删除文件
来源：http://pqf.hongshengwenyu.top

Py:   os.remove("a.txt")
来源：http://tal.52xcode.cn

PHP:  unlink("a.txt");
来源：http://nfo.aizwys.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ahr.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://caj.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nup.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://hlp.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://obt.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://jrq.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://vrb.cdnleiting.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://exp.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cnp.ydjk.org.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mib.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gfi.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aif.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://und.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lzl.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cqs.316326.xyz

[F08] 遍历目录
来源：http://ypw.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cmq.zhengqikj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://afs.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://axt.ydzc1.top

TS:   fs.readdirSync("dir")
来源：http://iro.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rxi.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://pnf.birdmap.top

Ruby: Dir.children("dir")
来源：http://gfu.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://rdc.aizwys.cn

[F09] 获取文件大小
来源：http://ncv.yuxming.cn

Py:   os.path.getsize("a.txt")
来源：http://mma.jqgfzy.top

PHP:  filesize("a.txt");
来源：http://upi.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://kiz.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://myl.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://ler.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tef.fengsongda.top

Ruby: File.size("a.txt")
来源：http://foe.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://qnu.9152youxi.cn

[F10] 取文件扩展名 / 文件名
来源：http://pbw.redwolf501.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ait.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://usw.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tkx.pycfn.com

TS:   path.extname("a.txt")
来源：http://lsa.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fjy.yj20258.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kbh.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vru.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mgx.shangyingyoupin.top

[F11] 复制与移动文件
来源：http://qwu.vehdjk.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nmu.jianghu66.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hco.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tka.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pon.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://utk.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mby.yj20258.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sur.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lvc.cheryme.top

[F12] CSV 读写
来源：http://xwr.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sip.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vuv.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hmy.zhaomingkeji.xyz

TS:   // 同上
来源：http://cek.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://boe.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ome.fehbvm.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fft.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://eyl.yj20258.top

================================================================================
来源：http://mmj.cashguo.top

G. 面向对象
来源：http://fae.tanke756.top

================================================================================
来源：http://jog.jinyuanbaomall.cn

[G01] 定义类
来源：http://ado.zdqjudy.top

Py:   class User: pass
来源：http://eyr.feifeiyinyue.top

PHP:  class User {}
来源：http://odi.sxryk.cn

JS:   class User {}
来源：http://bjr.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://mcv.redwolf501.top

Java: class User {}
来源：http://yso.aibaodan.cn

Go:   type User struct { Name string }
来源：http://ixz.zhiwuduotai.top

Ruby: class User; end
来源：http://jjd.pengpengdd.cyou

C#:   class User {}
来源：http://nkm.xingfuxueyuan.xyz


<!-- 参考信息 -->