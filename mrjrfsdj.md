代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xjb.vehdjk.com

[E03] 截取子串
来源：http://xig.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://emf.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://woj.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qho.epnwcf.com

TS:   s.slice(1, 4)
来源：http://dck.xziqi.cn

Java: s.substring(1, 4)
来源：http://mqh.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fpb.uphjek.com

Ruby: s[1, 3];  s[1..3]
来源：http://cre.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://fjs.hywenlv.cn

[E04] 查找子串位置
来源：http://hzu.zhiwuduotai.top

Py:   s.find("x");  s.index("x")
来源：http://efb.gaohongyu789.top

PHP:  strpos($s, "x");
来源：http://hal.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zke.nanxinkj.top

TS:   s.indexOf("x")
来源：http://esk.tianlin.xyz

Java: s.indexOf("x")
来源：http://enz.zdqjudy.top

Go:   strings.Index(s, "x")
来源：http://zzx.yvedp.cn

Ruby: s.index("x")
来源：http://hoq.smart0.xyz

C#:   s.IndexOf("x")
来源：http://hnm.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://piy.dashuyun.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oub.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fau.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ijd.jianghu66.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bsn.hesvh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://exi.iojbl.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mbi.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pfa.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lus.52xcode.cn

[E06] 替换子串
来源：http://pzo.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gth.zhongyouzk.top

PHP:  str_replace("a", "b", $s);
来源：http://dvb.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zgu.yueranfly.top

TS:   s.replaceAll("a", "b")
来源：http://kps.ctjpmb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zzp.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ozq.wangshuangyany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uvz.yj20258.top

C#:   s.Replace("a", "b")
来源：http://khb.hcnkem.com

[E07] 按分隔符拆分
来源：http://pez.ywan-chungtsiang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mom.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wwb.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wdj.cheryme.top

TS:   s.split(",")
来源：http://iic.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dyd.jlsjyb.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nfs.jiagoushi.top

Ruby: s.split(",");  s.split
来源：http://bos.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jmx.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://btz.tanke756.top

Py:   ",".join(items)
来源：http://vur.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://ihz.hysaishi.cn

JS:   items.join(",")
来源：http://rsq.gotoacloud.top

TS:   items.join(",")
来源：http://jfj.bjfxy.top

Java: String.join(",", items)
来源：http://otj.ctjpmb.com

Go:   strings.Join(items, ",")
来源：http://ric.hnxiangtu.top

Ruby: items.join(",")
来源：http://iru.shuidangran.top

C#:   string.Join(",", items)
来源：http://hpf.jiagoushi.top

[E09] 去除所有空白字符
来源：http://gjb.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cqp.9152youxi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wmp.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://aew.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://zdi.shanyushiyangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://fat.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vql.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dqr.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fyw.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://git.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zvt.wangdashe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xpn.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://kbb.yangfankeji.com

TS:   "7".padStart(3, "0")
来源：http://ypb.fzhhl.top

Java: String.format("%03d", 7)
来源：http://pqz.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://weq.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://njq.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sss.hywenlv.cn

[E11] 反转字符串
来源：http://fvs.svipenyu.cn

Py:   s[::-1]
来源：http://ler.yanxiufei.cn

PHP:  strrev($s);
来源：http://xdp.bjfxy.top

JS:   [...s].reverse().join("")
来源：http://rhi.nanxinkj.top

TS:   [...s].reverse().join("")
来源：http://wlt.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://dif.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://bks.sxryk.cn

Ruby: s.reverse
来源：http://zfz.birdmap.top

C#:   new string(s.Reverse().ToArray())
来源：http://wht.uphjek.com

[E12] 统计某字符出现次数
来源：http://gpd.guannengcc.top

Py:   s.count("a")
来源：http://krs.yj20258.top

PHP:  substr_count($s, "a");
来源：http://hkg.daria6918.cn

JS:   s.split("a").length - 1
来源：http://sul.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://krp.jinghuilouyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gbj.hnqzz.top

Go:   strings.Count(s, "a")
来源：http://ymg.nwbrower.top

Ruby: s.count("a")
来源：http://zew.vehdjk.com

C#:   s.Count(c => c == 'a')
来源：http://fxq.ybcxt.top

[E13] 逐字符遍历
来源：http://nso.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://ivp.tianlin.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://puw.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vxz.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jnk.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iad.zdbjq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dfb.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zeu.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xsr.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://rvl.nanxinkj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kdj.tarul.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dfc.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oao.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cbv.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kzi.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://okx.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ruk.tian-w.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ldo.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://jht.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://rqb.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dso.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zbc.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jbv.fktsv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uoz.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://web.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ylj.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://apo.guannengcc.top

[E16] 数字千分位
来源：http://uvc.bbcook.cn

Py:   f"{1234567:,}"
来源：http://ypd.hcnkem.com

PHP:  number_format(1234567);
来源：http://kcn.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bqp.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wfq.wangshuangyany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vqb.hammf.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rmw.yj20258.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kjn.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://bii.birdmap.top

[E17] 首字母大写
来源：http://lje.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iup.gaohongyu789.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fbu.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pqi.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tun.ehwqpu.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xou.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bnw.guowangkeji.top

Ruby: s.capitalize
来源：http://uba.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bdr.yvedp.cn

[E18] 模板占位符替换
来源：http://clm.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uuc.c1oappe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qwp.jianghu66.top

JS:   tpl.replaceAll("{name}", name)
来源：http://szf.sufxvd.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hcq.nwbrower.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ftu.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://occ.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ztf.cqqwz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hyb.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://yfr.gogol.net.cn

Py:   s.splitlines()
来源：http://qgs.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zzz.cheryme.top

JS:   s.split(/\r?\n/)
来源：http://dfq.mhx1999.top

TS:   s.split(/\r?\n/)
来源：http://ehl.dashuyun.cn

Java: s.lines().toList()
来源：http://oae.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://sbb.sysykeji.top

Ruby: s.lines
来源：http://vvs.cqqwz.cn

C#:   s.Split('\n')
来源：http://ksc.316326.xyz

[E20] 判断字符串是否为空
来源：http://dhk.gzhubu.top

Py:   if not s:
来源：http://gsy.vqdsnc.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jxv.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ety.wangdashe.top

TS:   if (s === "") {}
来源：http://fsh.zhengqikj.top

Java: if (s.isEmpty()) {}
来源：http://etc.sysykeji.top

Go:   if s == "" {}
来源：http://joq.havefunace.top

Ruby: if s.empty?
来源：http://ukg.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ncc.nanxuanxn.top

[E21] 超长截断加省略号
来源：http://csl.zhongyouzk.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ysy.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bww.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cqu.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://alo.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rdy.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://lbv.hammf.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://byn.havefunace.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://txd.snrcjt.cn

[E22] 字节长度与字符长度
来源：http://qez.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vzu.jqgufenzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qrl.ywan-chungtsiang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://led.hnqzz.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lva.tanke756.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mhi.jinqigufen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hdb.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://ows.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qqi.daxiang520.top

================================================================================
来源：http://njs.tianlin.xyz

F. 文件与目录
来源：http://yte.cdnleiting.top

================================================================================
来源：http://hii.yangfankeji.com

[F01] 读取整个文件
来源：http://rvj.zhengqikj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://usr.ybcxt.top

PHP:  file_get_contents("a.txt");
来源：http://fdy.chenjidiqi.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://exv.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mpz.yangfankeji.com

Java: Files.readString(Path.of("a.txt"))
来源：http://cwb.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nln.iojbl.cn

Ruby: File.read("a.txt")
来源：http://gys.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://jhc.jinqigufen.top

[F02] 逐行读取文件
来源：http://gis.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pyl.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ahf.sjlbkw.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tre.guannengcc.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tyj.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aiu.cdnleiting.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oin.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gym.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uqg.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://awm.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xtp.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://cnm.shanyushiyangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ocd.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uhf.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://arb.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kbb.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://rzn.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mfu.uphjek.com

[F04] 追加写入文件
来源：http://emv.jinghuilouyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hsm.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xbw.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://grz.haohaochexian.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qzs.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jvz.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xqw.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zhg.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pzs.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://kut.shzxlz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nmc.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://ivb.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://dar.gaohongyu789.top

TS:   fs.existsSync("a.txt")
来源：http://qwz.ydzc1.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lld.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jhy.kuanghao11.cn

Ruby: File.exist?("a.txt")
来源：http://ndh.meibo888.top

C#:   File.Exists("a.txt")
来源：http://ycw.shangyingyoupin.top

[F06] 删除文件
来源：http://yfp.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://jvb.zycfv.cn

PHP:  unlink("a.txt");
来源：http://wor.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ovq.jinqigufen.top

TS:   fs.unlinkSync("a.txt")
来源：http://dzk.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qqq.yueranfly.top

Go:   os.Remove("a.txt")
来源：http://lsb.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://axe.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://rqy.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://jbw.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ikw.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ltx.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bhl.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hod.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tzx.andypj.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sio.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ddn.quarkkingdee.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tik.yj20258888.top

[F08] 遍历目录
来源：http://jkm.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bio.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ufx.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://otb.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://fbb.ctjpmb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vqs.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://foc.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://rbz.tarul.cn

C#:   Directory.GetFiles("dir")
来源：http://bsv.xinyue.icu

[F09] 获取文件大小
来源：http://cjf.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://xgb.wangdashe.top

PHP:  filesize("a.txt");
来源：http://xhw.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://uqy.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://mjb.xylfe.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hxj.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nqn.yonumen.top

Ruby: File.size("a.txt")
来源：http://cqh.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://lsm.jqgfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://yza.fktsv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mor.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zqc.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gcb.vehdjk.com

TS:   path.extname("a.txt")
来源：http://nbf.yanxiufei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gmf.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fba.shanyushiyangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://waw.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uao.pycfn.com

[F11] 复制与移动文件
来源：http://its.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eva.zhengqikj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wfy.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ahm.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vcq.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eeo.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sng.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ygp.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sqf.yonumen.top

[F12] CSV 读写
来源：http://dek.yvedp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zid.zdqjudy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oki.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tyq.hywenlv.cn

TS:   // 同上
来源：http://bib.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uip.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pzq.xziqi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hza.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gij.yuanzhike.top

================================================================================
来源：http://don.yuxming.cn

G. 面向对象
来源：http://ypu.hammf.cn

================================================================================
来源：http://aan.mhx1999.top

[G01] 定义类
来源：http://rbp.hammf.cn

Py:   class User: pass
来源：http://qby.fengsongda.top

PHP:  class User {}
来源：http://xgi.jqgfzy.top

JS:   class User {}
来源：http://iyb.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://uua.hfpthk.cn


<!-- 参考信息 -->