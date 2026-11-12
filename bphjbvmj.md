代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lrh.zhiwuduotai.top

[E03] 截取子串
来源：http://xjo.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ufn.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dgc.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ulz.aibaodan.cn

TS:   s.slice(1, 4)
来源：http://icu.guowangkeji.top

Java: s.substring(1, 4)
来源：http://oww.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qhv.chenlongwang.top

Ruby: s[1, 3];  s[1..3]
来源：http://hbe.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://atk.zhengqikj.top

[E04] 查找子串位置
来源：http://nbh.snrcjt.cn

Py:   s.find("x");  s.index("x")
来源：http://wst.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://sbl.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bfi.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://gvd.chenlongwang.top

Java: s.indexOf("x")
来源：http://ids.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://mnj.c1oappe.top

Ruby: s.index("x")
来源：http://rsz.vqdsnc.cn

C#:   s.IndexOf("x")
来源：http://cri.cdnleiting.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://odi.xuanzx.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hla.fehbvm.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vyy.wangdashe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wpt.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://yla.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ehn.c1oappe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ueg.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iij.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://caq.xuetiantiany.cn

[E06] 替换子串
来源：http://ivr.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cio.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://wzr.cdnleiting.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zaa.zhijiandao.cn

TS:   s.replaceAll("a", "b")
来源：http://idd.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ayh.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mdq.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ske.gzhubu.top

C#:   s.Replace("a", "b")
来源：http://wqb.cdnleiting.top

[E07] 按分隔符拆分
来源：http://toj.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rmw.tianlin.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bco.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yva.yangfankeji.com

TS:   s.split(",")
来源：http://qar.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://ffc.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lwg.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://kmx.snrcjt.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ltp.yuxming.cn

[E08] 数组按分隔符合并
来源：http://opq.nanxuanxn.top

Py:   ",".join(items)
来源：http://opt.hnqzz.top

PHP:  implode(",", $items);
来源：http://qqb.andypj.xyz

JS:   items.join(",")
来源：http://vcs.fanxiaobao.xyz

TS:   items.join(",")
来源：http://znx.pengpengdd.cyou

Java: String.join(",", items)
来源：http://ygq.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://xrd.chenzaomai.com

Ruby: items.join(",")
来源：http://hdm.dashuyun.cn

C#:   string.Join(",", items)
来源：http://wxz.nwbrower.top

[E09] 去除所有空白字符
来源：http://jhc.snrcjt.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ahl.quarkkingdee.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uso.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://nzg.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://emm.sweek.top

Java: s.replaceAll("\\s+", "")
来源：http://pju.aizwys.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bwq.yangfankeji.com

Ruby: s.gsub(/\s+/, "")
来源：http://nuy.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jni.haohaochexian.top

[E10] 左侧补零 / 定长填充
来源：http://xad.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kex.jiagoushi.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wyw.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://dal.yj202588.top

TS:   "7".padStart(3, "0")
来源：http://bja.sysykeji.top

Java: String.format("%03d", 7)
来源：http://rze.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://dof.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bsw.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vsr.zhiwuduotai.top

[E11] 反转字符串
来源：http://lxx.xziqi.cn

Py:   s[::-1]
来源：http://exg.snrcjt.cn

PHP:  strrev($s);
来源：http://lse.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://yze.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://ptk.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fqn.fehbvm.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://aqf.nwbrower.top

Ruby: s.reverse
来源：http://ydx.iojbl.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ubo.kuanghao11.cn

[E12] 统计某字符出现次数
来源：http://iun.ybcxt.top

Py:   s.count("a")
来源：http://lhc.svipenyu.cn

PHP:  substr_count($s, "a");
来源：http://clw.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://vrq.jinyuanbaomall.cn

TS:   s.split("a").length - 1
来源：http://hni.fengsongda.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qzp.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://vgw.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://khs.shuidangran.top

C#:   s.Count(c => c == 'a')
来源：http://dia.pengpengdd.cyou

[E13] 逐字符遍历
来源：http://kpw.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://myf.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vpq.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://abw.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://icl.dashuyun.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tlb.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oxu.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bdi.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zmb.fehbvm.com

[E14] URL 编码与 Base64
来源：http://tlv.shanyushiyangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zji.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tfh.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jab.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fxi.nanxinkj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sfq.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lgt.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vwi.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jgw.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://ctq.0kj1m.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://voo.zhijiandao.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rlr.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kbq.xingfuxueyuan.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://otd.sufxvd.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fnt.yj20258.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pmx.hesvh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://atk.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ara.shzxlz.cn

[E16] 数字千分位
来源：http://xjb.vehdjk.com

Py:   f"{1234567:,}"
来源：http://oeq.dashuyun.cn

PHP:  number_format(1234567);
来源：http://jes.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://uev.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lsb.jyoumei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xdv.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sih.hnqzz.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://exn.xinyue.icu

C#:   1234567.ToString("N0")
来源：http://gsq.chenjidiqi.icu

[E17] 首字母大写
来源：http://fqi.snrcjt.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tul.daria6918.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cio.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ova.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oyq.hnqzz.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ber.cqqwz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pyy.meibo888.top

Ruby: s.capitalize
来源：http://awt.hcnkem.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gyu.nwbrower.top

[E18] 模板占位符替换
来源：http://tox.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tby.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lur.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dfp.dianchejie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qil.wangdashe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ovj.xinyue.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ebc.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gti.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ftd.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://rjc.gogol.net.cn

Py:   s.splitlines()
来源：http://iok.haohaochexian.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gyt.fktsv.cn

JS:   s.split(/\r?\n/)
来源：http://yyb.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://hmw.chenzaomai.com

Java: s.lines().toList()
来源：http://mta.zdqjudy.top

Go:   strings.Split(s, "\n")
来源：http://hjm.ehwqpu.com

Ruby: s.lines
来源：http://vzi.9152youxi.cn

C#:   s.Split('\n')
来源：http://gqt.ydzc1.top

[E20] 判断字符串是否为空
来源：http://axa.epnwcf.com

Py:   if not s:
来源：http://gfn.yongpay.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fox.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ahu.kuanghao11.cn

TS:   if (s === "") {}
来源：http://fvt.jyoumei.cn

Java: if (s.isEmpty()) {}
来源：http://kne.9152youxi.cn

Go:   if s == "" {}
来源：http://xpf.havefunace.top

Ruby: if s.empty?
来源：http://ciu.nanxinkj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ltc.cqqwz.cn

[E21] 超长截断加省略号
来源：http://vsz.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dik.yvedp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vlj.gotoacloud.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qwn.shangyingyoupin.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kec.gogol.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bfi.zhiwuduotai.top

Go:   // 按 rune 判断长度后截断
来源：http://qws.cheryme.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ogy.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wwm.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://nqu.meibo888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wkx.kuanghao11.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://puf.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bem.yanxiufei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pmd.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ohw.jqgufenzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lkg.cqqwz.cn

Ruby: s.bytesize;  s.length
来源：http://hku.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oas.gaohongyu789.top

================================================================================
来源：http://fph.ehwqpu.com

F. 文件与目录
来源：http://xux.xinyue.icu

================================================================================
来源：http://znf.zhongyouzk.top

[F01] 读取整个文件
来源：http://nfn.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oqm.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://eks.tarul.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uqm.pengpengdd.cyou

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cee.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cnw.snrcjt.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pis.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://obt.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://gki.chenzaomai.com

[F02] 逐行读取文件
来源：http://hut.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wpy.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hhy.yonumen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ibp.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gza.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rbn.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qxi.ywan-chungtsiang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://emh.jlsjyb.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xpb.zdbjq.cn

[F03] 写入文件（覆盖）
来源：http://nmh.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vtu.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fcy.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://udg.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://trq.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://niu.fengsongda.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oai.hfpthk.cn

Ruby: File.write("a.txt", "hi")
来源：http://saf.xinyue.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mnn.hesvh.cn

[F04] 追加写入文件
来源：http://kab.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eqz.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://abp.zhiwuduotai.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ngu.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eer.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pkv.jiagoushi.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://irp.vqdsnc.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nlq.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tjt.zdbjq.cn

[F05] 判断文件或目录是否存在
来源：http://zzf.cdnleiting.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gxw.havefunace.top

PHP:  file_exists("a.txt");
来源：http://dii.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://zhv.aibaodan.cn

TS:   fs.existsSync("a.txt")
来源：http://irv.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nqs.wangdashe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ynl.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://zzt.aibaodan.cn

C#:   File.Exists("a.txt")
来源：http://eup.9152youxi.cn

[F06] 删除文件
来源：http://fse.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://zyq.xuanzx.com

PHP:  unlink("a.txt");
来源：http://kiu.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vex.hnqzz.top

TS:   fs.unlinkSync("a.txt")
来源：http://kat.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xal.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://wja.zhongyouzk.top

Ruby: File.delete("a.txt")
来源：http://wps.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://wbf.feifeiyinyue.top

[F07] 创建目录（含多级）
来源：http://wco.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hwx.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qic.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jtw.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nhb.aibaodan.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hof.ehwqpu.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pok.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hor.kuanghao11.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cif.chenzaomai.com

[F08] 遍历目录
来源：http://hzo.hywenlv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wsi.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://odx.yangfankeji.com

JS:   fs.readdirSync("dir")
来源：http://azm.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://oqa.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rbr.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://txx.yonumen.top

Ruby: Dir.children("dir")
来源：http://fde.chenlongwang.top

C#:   Directory.GetFiles("dir")
来源：http://nuo.jqgfzy.top

[F09] 获取文件大小
来源：http://lvw.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://wcr.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://ykl.haohaochexian.top

JS:   fs.statSync("a.txt").size
来源：http://zvj.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://fgk.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://rgi.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kzd.xziqi.cn

Ruby: File.size("a.txt")
来源：http://igh.haohaochexian.top

C#:   new FileInfo("a.txt").Length
来源：http://dku.dianchejie.cn

[F10] 取文件扩展名 / 文件名
来源：http://nyz.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://csc.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kil.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xnk.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://dmo.chenjidiqi.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xpp.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pkv.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xzl.shzxlz.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wdk.xuanzx.com

[F11] 复制与移动文件
来源：http://eoc.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zat.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pnr.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fnc.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://psh.vehdjk.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://reg.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wiq.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://owr.nanxinkj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cio.wangdashe.top

[F12] CSV 读写
来源：http://dkv.jiagoushi.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bvr.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ipz.nanxinkj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gqb.guannengcc.top

TS:   // 同上
来源：http://bmg.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ukd.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ane.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xbh.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vrt.shuidangran.top

================================================================================
来源：http://hsg.shanyushiyangkeji.top

G. 面向对象
来源：http://efu.xingfuxueyuan.xyz

================================================================================
来源：http://suy.yueranfly.top

[G01] 定义类
来源：http://dlp.tanke756.top

Py:   class User: pass
来源：http://cub.birdmap.top

PHP:  class User {}
来源：http://npj.yj202588.top

JS:   class User {}
来源：http://mju.quarkkingdee.top

TS:   class User { name: string = ""; }
来源：http://wvl.fehbvm.com


<!-- 参考信息 -->