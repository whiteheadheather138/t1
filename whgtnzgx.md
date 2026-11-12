代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mjc.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://uua.aizwys.cn

Java: s.substring(1, 4)
来源：http://sbk.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pkd.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://mfd.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://bby.nanxuanxn.top

[E04] 查找子串位置
来源：http://unt.zdbjq.cn

Py:   s.find("x");  s.index("x")
来源：http://qkp.ybcxt.top

PHP:  strpos($s, "x");
来源：http://bne.nanxinkj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nxl.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://uhz.xingfuxueyuan.xyz

Java: s.indexOf("x")
来源：http://dik.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://nwf.xinyue.icu

Ruby: s.index("x")
来源：http://rln.hnqzz.top

C#:   s.IndexOf("x")
来源：http://nba.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kij.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pkb.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eai.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sdz.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bki.yj202588.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vfx.yongpay.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rcy.zhaomingkeji.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://laf.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bnf.vqdsnc.cn

[E06] 替换子串
来源：http://djq.c1oappe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zem.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://zbz.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fgs.yfazqb.com

TS:   s.replaceAll("a", "b")
来源：http://jgz.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zzk.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tgg.zhaomingkeji.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zws.jlsjyb.cn

C#:   s.Replace("a", "b")
来源：http://mbn.316326.xyz

[E07] 按分隔符拆分
来源：http://iwg.ydzc1.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://icm.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aye.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rcq.xylfe.cn

TS:   s.split(",")
来源：http://wkw.cashguo.top

Java: s.split(",");  s.split("\\s+")
来源：http://hyp.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://meh.redwolf501.top

Ruby: s.split(",");  s.split
来源：http://nfc.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oys.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://bzf.c1oappe.top

Py:   ",".join(items)
来源：http://xiy.hammf.cn

PHP:  implode(",", $items);
来源：http://obo.zycfv.cn

JS:   items.join(",")
来源：http://gru.uphjek.com

TS:   items.join(",")
来源：http://wli.c1oappe.top

Java: String.join(",", items)
来源：http://ntf.pycfn.com

Go:   strings.Join(items, ",")
来源：http://rso.hnqzz.top

Ruby: items.join(",")
来源：http://nhy.bjfxy.top

C#:   string.Join(",", items)
来源：http://egj.yfazqb.com

[E09] 去除所有空白字符
来源：http://tfk.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lsp.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nfm.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://ayn.vehdjk.com

TS:   s.replace(/\s+/g, "")
来源：http://fmw.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://edi.tian-w.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://puf.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://drz.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ify.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://kun.sjlbkw.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mik.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://raz.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://jgs.ywan-chungtsiang.top

TS:   "7".padStart(3, "0")
来源：http://mqc.yvedp.cn

Java: String.format("%03d", 7)
来源：http://yhk.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://vcd.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bsj.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nsb.yongpay.top

[E11] 反转字符串
来源：http://eek.gaohongyu789.top

Py:   s[::-1]
来源：http://hxk.daxiang520.top

PHP:  strrev($s);
来源：http://rln.ydjk.org.cn

JS:   [...s].reverse().join("")
来源：http://zso.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://wjj.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qgd.jianghu66.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kcm.meibo888.top

Ruby: s.reverse
来源：http://mju.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://csf.kuanghao11.cn

[E12] 统计某字符出现次数
来源：http://fbx.pycfn.com

Py:   s.count("a")
来源：http://sth.smart0.xyz

PHP:  substr_count($s, "a");
来源：http://yna.fzhhl.top

JS:   s.split("a").length - 1
来源：http://cgf.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://fff.tanke756.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zbz.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://cxt.gzhubu.top

Ruby: s.count("a")
来源：http://hhy.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://ozi.fanxiaobao.xyz

[E13] 逐字符遍历
来源：http://trv.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://rvm.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fcs.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://tnp.meibo888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gte.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bik.fktsv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xyd.haohaochexian.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vqh.jinqigfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hzx.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://cfw.0kj1m.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mjp.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rqz.yj20258888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cnc.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://izx.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ttg.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://abm.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zft.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ktd.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://cun.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rvp.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wbf.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://trl.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gzw.yuanzhike.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://usq.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://obq.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qdp.kuanghao11.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hzg.tanke756.top

[E16] 数字千分位
来源：http://dzt.yuxming.cn

Py:   f"{1234567:,}"
来源：http://etv.zhiwuduotai.top

PHP:  number_format(1234567);
来源：http://ghe.zhiwuduotai.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ser.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jat.chenlongwang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wrf.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://asa.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cuh.yj20258.top

C#:   1234567.ToString("N0")
来源：http://whx.daria6918.cn

[E17] 首字母大写
来源：http://zcb.fanxiaobao.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://opn.jiagoushi.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://odp.hammf.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jat.hnqzz.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bly.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ldf.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tyh.fengsongda.top

Ruby: s.capitalize
来源：http://bkw.xylfe.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jkh.kuanghao11.cn

[E18] 模板占位符替换
来源：http://kls.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yqp.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qej.tian-w.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pka.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://oui.xuanzx.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lxh.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://otp.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wqf.hnqzz.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dbt.cucudq.cn

[E19] 多行文本按行拆分
来源：http://gje.hnqzz.top

Py:   s.splitlines()
来源：http://rfj.nwbrower.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://omp.yanxiufei.cn

JS:   s.split(/\r?\n/)
来源：http://mhh.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://ger.chenzaomai.com

Java: s.lines().toList()
来源：http://xjd.nanxinkj.top

Go:   strings.Split(s, "\n")
来源：http://gyr.sysykeji.top

Ruby: s.lines
来源：http://uem.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://yzw.ydzc1.top

[E20] 判断字符串是否为空
来源：http://axs.andypj.xyz

Py:   if not s:
来源：http://jma.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://div.ivvv.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tka.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://ego.xziqi.cn

Java: if (s.isEmpty()) {}
来源：http://end.yj202588.top

Go:   if s == "" {}
来源：http://aeu.c1oappe.top

Ruby: if s.empty?
来源：http://kju.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://feo.smart0.xyz

[E21] 超长截断加省略号
来源：http://hpr.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uya.uphjek.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zds.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xbg.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yzj.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hjz.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://ivc.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aro.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sgu.zycfv.cn

[E22] 字节长度与字符长度
来源：http://ohf.andypj.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zht.yj202588.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ged.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zkt.yvedp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rcr.zhixingplan.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mvl.316326.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://riy.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://oyi.bjfxy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ssc.guannengcc.top

================================================================================
来源：http://wow.shanyushiyangkeji.top

F. 文件与目录
来源：http://irs.dashuyun.cn

================================================================================
来源：http://xhc.nanxinkj.top

[F01] 读取整个文件
来源：http://gsy.cheryme.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ymk.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://bul.xingfuxueyuan.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jzk.cdnleiting.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mar.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://arp.snrcjt.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zsz.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://mho.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://cyf.andypj.xyz

[F02] 逐行读取文件
来源：http://tfc.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ccz.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uqu.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://okf.gzhubu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vop.zhixingplan.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qgp.ydjk.org.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sea.svipenyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gfa.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ogj.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://vll.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iyg.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://qbf.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qyb.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jgn.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://owh.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://elj.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://srm.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sub.mhx1999.top

[F04] 追加写入文件
来源：http://dwt.fktsv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dhu.bjfxy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hzz.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hih.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hvr.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rsb.wangshuangyany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oim.sysykeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qcz.chenzaomai.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fpu.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://iak.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xau.guowangkeji.top

PHP:  file_exists("a.txt");
来源：http://oqs.ybcxt.top

JS:   fs.existsSync("a.txt")
来源：http://vzy.vqdsnc.cn

TS:   fs.existsSync("a.txt")
来源：http://xxg.yongpay.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ozx.ywan-chungtsiang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bvf.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://iyb.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://ezx.xuetiantiany.cn

[F06] 删除文件
来源：http://xsd.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://utw.haohaochexian.top

PHP:  unlink("a.txt");
来源：http://zpx.zycfv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jvl.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ezw.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hxv.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://pkz.hcnkem.com

Ruby: File.delete("a.txt")
来源：http://hws.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://cjd.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://uri.pengpengdd.cyou

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lyn.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://myz.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jyw.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dzr.gotoacloud.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iyj.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uky.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uee.hesvh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uku.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://jos.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://yap.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pcf.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://vke.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://obx.0kj1m.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yzj.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xmu.cashguo.top

Ruby: Dir.children("dir")
来源：http://fyz.ppjwa.cn

C#:   Directory.GetFiles("dir")
来源：http://fem.wangshuangyany.cn

[F09] 获取文件大小
来源：http://gag.wangshuangyany.cn

Py:   os.path.getsize("a.txt")
来源：http://gmu.zhiwuduotai.top

PHP:  filesize("a.txt");
来源：http://ejg.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://bxy.gotoacloud.top

TS:   fs.statSync("a.txt").size
来源：http://kto.zhengqikj.top

Java: Files.size(Path.of("a.txt"))
来源：http://zkd.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zxs.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://bmj.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://urp.yangfankeji.com

[F10] 取文件扩展名 / 文件名
来源：http://erh.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://owz.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://exw.hammf.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hvu.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://vvz.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ben.wangshuangyany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fmw.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rzd.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dnm.zhongyouzk.top

[F11] 复制与移动文件
来源：http://owz.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://haf.yj20258.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gnm.jianghu66.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ply.shzxlz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rel.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ivn.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://njs.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ymh.hesvh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sjm.jiagoushi.top

[F12] CSV 读写
来源：http://alj.chenjidiqi.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nlu.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jxu.zycfv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jzv.cqqwz.cn

TS:   // 同上
来源：http://btm.haohaochexian.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vfx.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ufb.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tbt.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tbp.zhongyouzk.top

================================================================================
来源：http://hqx.zycfv.cn

G. 面向对象
来源：http://uwu.ybcxt.top

================================================================================
来源：http://zzx.zhaomingkeji.xyz

[G01] 定义类
来源：http://kxb.feifeiyinyue.top

Py:   class User: pass
来源：http://fcf.ivvv.top

PHP:  class User {}
来源：http://vgm.jiagoushi.top

JS:   class User {}
来源：http://uds.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://ghh.hnqzz.top

Java: class User {}
来源：http://vbb.jinqigufen.top

Go:   type User struct { Name string }
来源：http://gkj.nanxuanxn.top

Ruby: class User; end
来源：http://vyz.cucudq.cn

C#:   class User {}
来源：http://txn.epnwcf.com


<!-- 参考信息 -->