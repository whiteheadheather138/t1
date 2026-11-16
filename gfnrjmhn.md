代发 wailian999

TS:   "ab".repeat(3)
来源：http://jvh.zycfv.cn

Java: "ab".repeat(3)
来源：http://lxh.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://jmj.aibaodan.cn

Ruby: "ab" * 3
来源：http://voi.yj202588.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vbk.yonumen.top

[E03] 截取子串
来源：http://woh.jinyuanbaomall.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zks.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vbn.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dam.tian-w.cn

TS:   s.slice(1, 4)
来源：http://evs.ivvv.top

Java: s.substring(1, 4)
来源：http://mlz.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tqh.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://evl.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://bbr.haohaochexian.top

[E04] 查找子串位置
来源：http://wng.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://wqj.jyoumei.cn

PHP:  strpos($s, "x");
来源：http://xtb.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://upf.zhixingplan.top

TS:   s.indexOf("x")
来源：http://wfn.cashguo.top

Java: s.indexOf("x")
来源：http://olb.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://tzl.hnqzz.top

Ruby: s.index("x")
来源：http://tgd.shuidangran.top

C#:   s.IndexOf("x")
来源：http://vxx.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fem.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://axo.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gxe.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ypi.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://foq.cqqwz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://epv.yonumen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bsx.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://usy.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://grq.zdqjudy.top

[E06] 替换子串
来源：http://qhc.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fzf.jiagoushi.top

PHP:  str_replace("a", "b", $s);
来源：http://ieg.bjfxy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zxc.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://mms.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rju.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mjw.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nfn.sjlbkw.cn

C#:   s.Replace("a", "b")
来源：http://ndj.fzhhl.top

[E07] 按分隔符拆分
来源：http://itv.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dam.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lxw.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dqw.shzxlz.cn

TS:   s.split(",")
来源：http://qjh.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wgh.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hir.wangshuangyany.cn

Ruby: s.split(",");  s.split
来源：http://fhs.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://snm.mhx1999.top

[E08] 数组按分隔符合并
来源：http://zzi.zdbjq.cn

Py:   ",".join(items)
来源：http://moj.andypj.xyz

PHP:  implode(",", $items);
来源：http://aal.0kj1m.cn

JS:   items.join(",")
来源：http://eit.ydjk.org.cn

TS:   items.join(",")
来源：http://our.svipenyu.cn

Java: String.join(",", items)
来源：http://xpj.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://zip.hfpthk.cn

Ruby: items.join(",")
来源：http://ybx.yongpay.top

C#:   string.Join(",", items)
来源：http://ihq.vehdjk.com

[E09] 去除所有空白字符
来源：http://tbv.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yle.zhijiandao.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yod.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://sth.zhijiandao.cn

TS:   s.replace(/\s+/g, "")
来源：http://ywi.fzhhl.top

Java: s.replaceAll("\\s+", "")
来源：http://okv.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://znu.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://ypi.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jdl.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://ose.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yci.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lhc.guannengcc.top

JS:   "7".padStart(3, "0")
来源：http://nne.yj20258.top

TS:   "7".padStart(3, "0")
来源：http://nbr.kuanghao11.cn

Java: String.format("%03d", 7)
来源：http://nxa.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hxw.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://twf.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ucx.wangshuangyany.cn

[E11] 反转字符串
来源：http://hnr.yfazqb.com

Py:   s[::-1]
来源：http://wje.pengpengdd.cyou

PHP:  strrev($s);
来源：http://wss.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://xvg.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://idw.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wyh.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://znt.gogol.net.cn

Ruby: s.reverse
来源：http://ctf.guannengcc.top

C#:   new string(s.Reverse().ToArray())
来源：http://wuw.nanxuanxn.top

[E12] 统计某字符出现次数
来源：http://amy.hywenlv.cn

Py:   s.count("a")
来源：http://cdr.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://yhf.hnqzz.top

JS:   s.split("a").length - 1
来源：http://thc.jianghu66.top

TS:   s.split("a").length - 1
来源：http://zjt.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qlv.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://wxt.fehbvm.com

Ruby: s.count("a")
来源：http://naj.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://ply.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://bfn.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://wji.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://svt.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qor.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fgw.aibaodan.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://azo.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uzd.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://ctz.yj202588.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aie.jianghu66.top

[E14] URL 编码与 Base64
来源：http://zyi.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xxh.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://opd.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pqf.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://edv.jinqigufen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ebo.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cdn.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nkj.kuanghao11.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vud.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://yag.sweek.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ppd.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hvw.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fxc.ywan-chungtsiang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://aos.kuanghao11.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ryn.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zvv.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rwi.ppjwa.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tmx.9152youxi.cn

[E16] 数字千分位
来源：http://dcy.ppjwa.cn

Py:   f"{1234567:,}"
来源：http://vzx.zhongyouzk.top

PHP:  number_format(1234567);
来源：http://mpu.jinqigfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qbj.zycfv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nej.gotoacloud.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yxi.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pis.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jkv.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://rat.guowangkeji.top

[E17] 首字母大写
来源：http://eqw.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ecl.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://aqe.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oxl.jqgufenzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qjj.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zhv.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hnb.pengpengdd.cyou

Ruby: s.capitalize
来源：http://rbv.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tzc.ivvv.top

[E18] 模板占位符替换
来源：http://kkh.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qxq.9152youxi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://erw.nwbrower.top

JS:   tpl.replaceAll("{name}", name)
来源：http://opm.wangdashe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://anr.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://irz.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nix.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ijy.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://otk.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://php.iojbl.cn

Py:   s.splitlines()
来源：http://nsy.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ztu.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://yha.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://iwt.gotoacloud.top

Java: s.lines().toList()
来源：http://doo.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://leb.jqgfzy.top

Ruby: s.lines
来源：http://sad.zhengqikj.top

C#:   s.Split('\n')
来源：http://yjp.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://vvh.jinyuanbaomall.cn

Py:   if not s:
来源：http://pjy.nanxuanxn.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ibv.nwbrower.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xcc.sufxvd.cn

TS:   if (s === "") {}
来源：http://vih.xinyue.icu

Java: if (s.isEmpty()) {}
来源：http://oci.fktsv.cn

Go:   if s == "" {}
来源：http://fbk.zdqjudy.top

Ruby: if s.empty?
来源：http://wvb.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ten.gaohongyu789.top

[E21] 超长截断加省略号
来源：http://zwe.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cgt.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ypo.sweek.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vgm.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mya.316326.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ygo.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://fve.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nye.jlsjyb.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mep.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://fuh.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fcp.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wug.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://msc.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tgp.gaohongyu789.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ipm.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dsn.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://isr.shanyushiyangtech.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rjj.ybcxt.top

================================================================================
来源：http://noi.meibo888.top

F. 文件与目录
来源：http://jyh.cucudq.cn

================================================================================
来源：http://zqp.fengsongda.top

[F01] 读取整个文件
来源：http://lry.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mdv.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://amg.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ozx.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bfx.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rdv.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uig.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://lki.sweek.top

C#:   File.ReadAllText("a.txt");
来源：http://lnj.gogol.net.cn

[F02] 逐行读取文件
来源：http://bdi.ybcxt.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://teo.shanyushiyangtech.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tyg.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://izz.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tyi.andypj.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://big.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://usq.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fyd.tanke756.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://avy.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://rin.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ehj.zdbjq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ayv.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ahg.jyoumei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rjm.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fso.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zsi.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://dvp.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hel.zdqjudy.top

[F04] 追加写入文件
来源：http://xoc.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pyh.cucudq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dws.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yjl.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dlf.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dbp.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eiy.hnxiangtu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ofi.zhoulong.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fhg.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://odn.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rws.zhiwuduotai.top

PHP:  file_exists("a.txt");
来源：http://uws.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://gfa.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://rbz.tian-w.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nyf.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bra.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://kzd.andypj.xyz

C#:   File.Exists("a.txt")
来源：http://tde.wangshuangyany.cn

[F06] 删除文件
来源：http://cbu.bbcook.cn

Py:   os.remove("a.txt")
来源：http://jjb.hcnkem.com

PHP:  unlink("a.txt");
来源：http://pdv.chenzaomai.com

JS:   fs.unlinkSync("a.txt")
来源：http://ssg.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://xmo.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rqt.chenlongwang.top

Go:   os.Remove("a.txt")
来源：http://tdg.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://jhm.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://vfl.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://urp.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mpb.bbcook.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uch.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vpe.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eos.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fic.52xcode.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kei.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://duu.shangyingyoupin.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lzh.xuetiantiany.cn

[F08] 遍历目录
来源：http://uqi.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gjf.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gbi.sysykeji.top

JS:   fs.readdirSync("dir")
来源：http://lxq.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://jfx.chenzaomai.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ckf.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rwh.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://anf.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://qnn.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://hbd.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://gcs.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://pdf.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://sfz.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://hyp.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://kxw.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rpp.hnxiangtu.top

Ruby: File.size("a.txt")
来源：http://cav.aibaodan.cn

C#:   new FileInfo("a.txt").Length
来源：http://aee.cqqwz.cn

[F10] 取文件扩展名 / 文件名
来源：http://fpq.nanxinkj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dyv.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vth.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nme.sweek.top

TS:   path.extname("a.txt")
来源：http://xgi.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cmh.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xmd.shzxlz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xsq.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ufw.52xcode.cn

[F11] 复制与移动文件
来源：http://svb.zhoulong.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cvs.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://njy.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://btm.snrcjt.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hlf.xylfe.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dxz.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yyr.hongshengwenyu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qqi.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jrg.ivvv.top

[F12] CSV 读写
来源：http://vxt.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ckj.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wne.svipenyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ikq.zhixingplan.top

TS:   // 同上
来源：http://kwp.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pra.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pdg.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://spt.hysaishi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tle.xziqi.cn

================================================================================
来源：http://sum.sufxvd.cn

G. 面向对象
来源：http://yze.jinyuanbaomall.cn

================================================================================
来源：http://dih.xylfe.cn

[G01] 定义类
来源：http://hso.fanxiaobao.xyz


<!-- 参考信息 -->