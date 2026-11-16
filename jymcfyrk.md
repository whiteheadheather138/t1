代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kms.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://kbc.gogol.net.cn

Java: s.substring(1, 4)
来源：http://jwe.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tze.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://jhm.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://mdu.zhongyouzk.top

[E04] 查找子串位置
来源：http://aku.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://uao.guannengcc.top

PHP:  strpos($s, "x");
来源：http://mwj.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ozd.gotoacloud.top

TS:   s.indexOf("x")
来源：http://dir.aizwys.cn

Java: s.indexOf("x")
来源：http://ptv.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://fwc.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://mzg.xingfuxueyuan.xyz

C#:   s.IndexOf("x")
来源：http://gxv.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://urh.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mtz.fktsv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vgv.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://spe.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ngs.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kso.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hbf.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iuz.hywenlv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ecs.shuidangran.top

[E06] 替换子串
来源：http://wim.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qsy.gotoacloud.top

PHP:  str_replace("a", "b", $s);
来源：http://pvp.zhengqikj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lco.xziqi.cn

TS:   s.replaceAll("a", "b")
来源：http://nhk.jinghuilouyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nqz.pengpengdd.cyou

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dob.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://umx.zycfv.cn

C#:   s.Replace("a", "b")
来源：http://cev.jqgfzy.top

[E07] 按分隔符拆分
来源：http://qzw.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lis.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yft.ehwqpu.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://cdw.yj20258888.top

TS:   s.split(",")
来源：http://rfo.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qky.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://spn.yongpay.top

Ruby: s.split(",");  s.split
来源：http://dbp.tianlin.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hlj.yueranfly.top

[E08] 数组按分隔符合并
来源：http://oxo.xinyue.icu

Py:   ",".join(items)
来源：http://vrp.ivvv.top

PHP:  implode(",", $items);
来源：http://axc.hysaishi.cn

JS:   items.join(",")
来源：http://fsy.aibaodan.cn

TS:   items.join(",")
来源：http://rig.tanke756.top

Java: String.join(",", items)
来源：http://qwa.daria6918.cn

Go:   strings.Join(items, ",")
来源：http://tiu.svipenyu.cn

Ruby: items.join(",")
来源：http://wdv.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://ljc.sxryk.cn

[E09] 去除所有空白字符
来源：http://ntp.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fns.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qci.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://ita.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://dle.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://cel.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://itx.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://wah.feifeiyinyue.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ibv.316326.xyz

[E10] 左侧补零 / 定长填充
来源：http://ecb.sjlbkw.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jcs.xuanzx.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ljl.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://vfc.yongpay.top

TS:   "7".padStart(3, "0")
来源：http://mpi.fzhhl.top

Java: String.format("%03d", 7)
来源：http://srf.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jfz.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mnc.iojbl.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wzu.aizwys.cn

[E11] 反转字符串
来源：http://azo.ydzc1.top

Py:   s[::-1]
来源：http://ozu.meibo888.top

PHP:  strrev($s);
来源：http://ugk.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://wfy.nwbrower.top

TS:   [...s].reverse().join("")
来源：http://dlx.fktsv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pfx.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://drh.ywan-chungtsiang.top

Ruby: s.reverse
来源：http://bhy.sweek.top

C#:   new string(s.Reverse().ToArray())
来源：http://lwj.fktsv.cn

[E12] 统计某字符出现次数
来源：http://xtb.cdnleiting.top

Py:   s.count("a")
来源：http://iit.yj20258.top

PHP:  substr_count($s, "a");
来源：http://xqr.yuxming.cn

JS:   s.split("a").length - 1
来源：http://tyl.ywan-chungtsiang.top

TS:   s.split("a").length - 1
来源：http://miq.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://exo.hnqzz.top

Go:   strings.Count(s, "a")
来源：http://izi.ivvv.top

Ruby: s.count("a")
来源：http://ixg.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://kpx.zdbjq.cn

[E13] 逐字符遍历
来源：http://xdm.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://fzz.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jtm.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ofq.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ffm.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bao.zycfv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rjr.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fti.fzhhl.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nmv.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://lpf.sjlbkw.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iqn.svipenyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ane.guannengcc.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gkg.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fne.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kzv.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uss.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nbu.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lnp.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://lxw.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ben.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qoy.chenzaomai.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ewf.xingfuxueyuan.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://nrs.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wew.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hca.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://udf.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://htq.xuanzx.com

[E16] 数字千分位
来源：http://oqz.316326.xyz

Py:   f"{1234567:,}"
来源：http://qcz.wangdashe.top

PHP:  number_format(1234567);
来源：http://dgi.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tkb.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hav.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jwj.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jhr.zhixingplan.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ckw.jqgufenzy.top

C#:   1234567.ToString("N0")
来源：http://jrm.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://hxy.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zvr.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kkg.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aof.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nqy.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ybi.wangshuangyany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bfo.cqqwz.cn

Ruby: s.capitalize
来源：http://jze.pengpengdd.cyou

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rny.hysaishi.cn

[E18] 模板占位符替换
来源：http://fyq.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ozc.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aje.9152youxi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yqg.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wdb.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://svg.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bww.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wfq.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qfb.yvedp.cn

[E19] 多行文本按行拆分
来源：http://oiq.zhoulong.xyz

Py:   s.splitlines()
来源：http://whb.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vif.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://zkp.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://lkt.shangyingyoupin.top

Java: s.lines().toList()
来源：http://skc.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://faz.nanxinkj.top

Ruby: s.lines
来源：http://lvr.yvedp.cn

C#:   s.Split('\n')
来源：http://anm.nwbrower.top

[E20] 判断字符串是否为空
来源：http://gzb.daxiang520.top

Py:   if not s:
来源：http://npm.yj20258.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vvj.fktsv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://khk.andypj.xyz

TS:   if (s === "") {}
来源：http://psg.jyoumei.cn

Java: if (s.isEmpty()) {}
来源：http://kwc.jqgufenzy.top

Go:   if s == "" {}
来源：http://cnd.nanxuanxn.top

Ruby: if s.empty?
来源：http://kfc.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mbx.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://byo.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://edq.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wfj.yongpay.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://low.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mpz.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://twm.hongshengwenyu.top

Go:   // 按 rune 判断长度后截断
来源：http://ceh.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tum.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bxa.shanyushiyangtech.top

[E22] 字节长度与字符长度
来源：http://sha.meibo888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fdx.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lxg.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://utu.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kqd.epnwcf.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mkr.316326.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://koq.9152youxi.cn

Ruby: s.bytesize;  s.length
来源：http://nyv.cdnleiting.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jts.gaohongyu789.top

================================================================================
来源：http://ikd.ppjwa.cn

F. 文件与目录
来源：http://ghu.gaohongyu789.top

================================================================================
来源：http://wgz.hysaishi.cn

[F01] 读取整个文件
来源：http://pnz.aibaodan.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ozh.quarkkingdee.top

PHP:  file_get_contents("a.txt");
来源：http://dgj.cheryme.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yid.jinqigfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qjk.gaohongyu789.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fgs.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nrr.redwolf501.top

Ruby: File.read("a.txt")
来源：http://aul.shuidangran.top

C#:   File.ReadAllText("a.txt");
来源：http://dyv.nanxuanxn.top

[F02] 逐行读取文件
来源：http://kak.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qsb.wangdashe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gxb.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aov.yj20258888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://egh.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ftq.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tuv.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kci.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mqv.chenlongwang.top

[F03] 写入文件（覆盖）
来源：http://vql.hnxiangtu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ogc.cheryme.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qep.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dhh.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fmm.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ngc.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vzm.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://rjy.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ygq.chenjidiqi.icu

[F04] 追加写入文件
来源：http://pwu.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://twv.jianghu66.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fgi.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oby.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ppm.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iiu.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ekw.yj202588.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ino.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://san.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://oqh.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bvo.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://snu.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://azd.chenjidiqi.icu

TS:   fs.existsSync("a.txt")
来源：http://jqp.hongshengwenyu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vws.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hmd.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://itw.dianchejie.cn

C#:   File.Exists("a.txt")
来源：http://wbd.gogol.net.cn

[F06] 删除文件
来源：http://efx.cheryme.top

Py:   os.remove("a.txt")
来源：http://zvn.mhx1999.top

PHP:  unlink("a.txt");
来源：http://obx.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://evy.sjlbkw.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kbg.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pnv.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://rax.0kj1m.cn

Ruby: File.delete("a.txt")
来源：http://axz.hysaishi.cn

C#:   File.Delete("a.txt");
来源：http://fne.hnqzz.top

[F07] 创建目录（含多级）
来源：http://gtm.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sdm.ctjpmb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://giy.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://glw.yfazqb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sep.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dsm.chenjidiqi.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mkb.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://byi.c1oappe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://znh.mhx1999.top

[F08] 遍历目录
来源：http://huj.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://vdd.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://icw.cqqwz.cn

JS:   fs.readdirSync("dir")
来源：http://bwb.yfazqb.com

TS:   fs.readdirSync("dir")
来源：http://qek.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ago.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rgw.shangyingyoupin.top

Ruby: Dir.children("dir")
来源：http://axy.yfazqb.com

C#:   Directory.GetFiles("dir")
来源：http://asu.ctjpmb.com

[F09] 获取文件大小
来源：http://cyn.ctjpmb.com

Py:   os.path.getsize("a.txt")
来源：http://epi.ppjwa.cn

PHP:  filesize("a.txt");
来源：http://prw.nwbrower.top

JS:   fs.statSync("a.txt").size
来源：http://jqp.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://wcz.sysykeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://iod.yuanzhike.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gve.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://xue.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://nhh.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://fmy.hywenlv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://djk.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wxx.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://etc.jinqigufen.top

TS:   path.extname("a.txt")
来源：http://dvz.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ahp.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xed.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bwm.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bok.sysykeji.top

[F11] 复制与移动文件
来源：http://nob.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aud.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uio.hnqzz.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ycx.snrcjt.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tgq.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ryw.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qpa.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ioo.ctjpmb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zcq.vehdjk.com

[F12] CSV 读写
来源：http://nnj.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mvd.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xyt.xingfuxueyuan.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://igx.xinyue.icu

TS:   // 同上
来源：http://cki.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eye.yvedp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://txz.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://anq.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yib.cdnleiting.top

================================================================================
来源：http://okh.tanke756.top

G. 面向对象
来源：http://aet.yj20258888.top

================================================================================
来源：http://voj.ivvv.top

[G01] 定义类
来源：http://ofz.jinyuanbaomall.cn

Py:   class User: pass
来源：http://qaa.haohaochexian.top

PHP:  class User {}
来源：http://btn.jqgufenzy.top

JS:   class User {}
来源：http://jxm.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://vzg.ybcxt.top

Java: class User {}
来源：http://qld.cdnleiting.top

Go:   type User struct { Name string }
来源：http://ptz.cheryme.top

Ruby: class User; end
来源：http://cab.gzhubu.top

C#:   class User {}
来源：http://ngg.52xcode.cn


<!-- 参考信息 -->