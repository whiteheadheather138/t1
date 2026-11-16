代发 wailian999

TS:   "ab".repeat(3)
来源：http://tzp.tanke756.top

Java: "ab".repeat(3)
来源：http://oen.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://wpi.sjlbkw.cn

Ruby: "ab" * 3
来源：http://wst.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uzo.vqdsnc.cn

[E03] 截取子串
来源：http://mcr.hcnkem.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uxs.c1oappe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mas.hnqzz.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sjs.hesvh.cn

TS:   s.slice(1, 4)
来源：http://exr.redwolf501.top

Java: s.substring(1, 4)
来源：http://vsq.aizwys.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fkk.fehbvm.com

Ruby: s[1, 3];  s[1..3]
来源：http://uck.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://wab.ydjk.org.cn

[E04] 查找子串位置
来源：http://efl.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://bbi.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://nma.cheryme.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://unc.tarul.cn

TS:   s.indexOf("x")
来源：http://cra.hysaishi.cn

Java: s.indexOf("x")
来源：http://pzq.hcnkem.com

Go:   strings.Index(s, "x")
来源：http://zdw.nanxinkj.top

Ruby: s.index("x")
来源：http://ofy.andypj.xyz

C#:   s.IndexOf("x")
来源：http://gsi.jinghuilouyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wfl.vqdsnc.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zdn.yj20258888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qvc.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bmj.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://ogf.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kmi.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ctv.hnxiangtu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hss.shanyushiyangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xwk.shanyushiyangtech.top

[E06] 替换子串
来源：http://fxy.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://scr.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://qhd.jinqigfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tfk.snrcjt.cn

TS:   s.replaceAll("a", "b")
来源：http://alc.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cvi.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xrn.sxryk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yiq.cheryme.top

C#:   s.Replace("a", "b")
来源：http://knj.svipenyu.cn

[E07] 按分隔符拆分
来源：http://ggr.xingfuxueyuan.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lqf.tian-w.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hwa.pycfn.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ydd.zhijiandao.cn

TS:   s.split(",")
来源：http://mzp.svipenyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://idy.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ncw.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://jlv.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hnt.yj202588.top

[E08] 数组按分隔符合并
来源：http://btn.hcnkem.com

Py:   ",".join(items)
来源：http://wfi.ivvv.top

PHP:  implode(",", $items);
来源：http://ziw.nanxuanxn.top

JS:   items.join(",")
来源：http://vtz.jiagoushi.top

TS:   items.join(",")
来源：http://ecu.hammf.cn

Java: String.join(",", items)
来源：http://isv.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://nde.epnwcf.com

Ruby: items.join(",")
来源：http://gdj.nanxinkj.top

C#:   string.Join(",", items)
来源：http://chb.dianchejie.cn

[E09] 去除所有空白字符
来源：http://rrf.yfazqb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mvd.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://plr.uphjek.com

JS:   s.replace(/\s+/g, "")
来源：http://ncg.vehdjk.com

TS:   s.replace(/\s+/g, "")
来源：http://tiu.wangdashe.top

Java: s.replaceAll("\\s+", "")
来源：http://ikh.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ukl.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://ozl.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kli.shanyushiyangtech.top

[E10] 左侧补零 / 定长填充
来源：http://zve.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lvd.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kql.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://lyo.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://gax.ybcxt.top

Java: String.format("%03d", 7)
来源：http://knl.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zuo.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dqt.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ods.uphjek.com

[E11] 反转字符串
来源：http://gux.tian-w.cn

Py:   s[::-1]
来源：http://ngq.ybcxt.top

PHP:  strrev($s);
来源：http://oea.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://iad.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://gbj.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://tra.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ytt.ydzc1.top

Ruby: s.reverse
来源：http://qcv.sweek.top

C#:   new string(s.Reverse().ToArray())
来源：http://kpm.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://rgv.guannengcc.top

Py:   s.count("a")
来源：http://egn.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://emc.sxryk.cn

JS:   s.split("a").length - 1
来源：http://xpz.fanxiaobao.xyz

TS:   s.split("a").length - 1
来源：http://oet.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bnj.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://zqr.dianchejie.cn

Ruby: s.count("a")
来源：http://sdc.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://jin.vehdjk.com

[E13] 逐字符遍历
来源：http://npc.sweek.top

Py:   for ch in s: print(ch)
来源：http://jyg.chenzaomai.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hxc.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xzt.daxiang520.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xsr.zhengqikj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rpu.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://czs.wangshuangyany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://opv.cheryme.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aap.shangyingyoupin.top

[E14] URL 编码与 Base64
来源：http://bjp.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bku.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://htq.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zba.redwolf501.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hsi.snrcjt.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gnj.yuanzhike.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ied.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rhh.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://phi.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://tsg.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gpi.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qdz.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ywc.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://qme.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mpx.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rby.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fjx.yueranfly.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oxr.xylfe.cn

[E16] 数字千分位
来源：http://zue.sysykeji.top

Py:   f"{1234567:,}"
来源：http://gfl.zhongyouzk.top

PHP:  number_format(1234567);
来源：http://min.yueranfly.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yxb.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://oad.sufxvd.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dhw.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hie.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xcn.daxiang520.top

C#:   1234567.ToString("N0")
来源：http://ktd.daria6918.cn

[E17] 首字母大写
来源：http://hkt.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pud.jlsjyb.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vzm.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fxy.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bwe.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kof.uphjek.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jnl.jiagoushi.top

Ruby: s.capitalize
来源：http://kua.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yqf.tianlin.xyz

[E18] 模板占位符替换
来源：http://jah.nanxinkj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ecw.wangshuangyany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ucp.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://caa.hnxiangtu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ana.yongpay.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ais.hfpthk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://irw.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://luh.yanxiufei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cbv.tian-w.cn

[E19] 多行文本按行拆分
来源：http://btj.daxiang520.top

Py:   s.splitlines()
来源：http://znl.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lxw.redwolf501.top

JS:   s.split(/\r?\n/)
来源：http://hfs.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://kgm.daria6918.cn

Java: s.lines().toList()
来源：http://svc.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://yze.316326.xyz

Ruby: s.lines
来源：http://odn.aizwys.cn

C#:   s.Split('\n')
来源：http://iak.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://nzu.vqdsnc.cn

Py:   if not s:
来源：http://sek.shanyushiyangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rse.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aho.tianlin.xyz

TS:   if (s === "") {}
来源：http://ekz.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://juz.c1oappe.top

Go:   if s == "" {}
来源：http://viu.yongpay.top

Ruby: if s.empty?
来源：http://vda.snrcjt.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fac.zhaomingkeji.xyz

[E21] 超长截断加省略号
来源：http://zom.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://itv.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tgo.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://snd.pycfn.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hga.nwbrower.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tfo.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://qll.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lth.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cel.9152youxi.cn

[E22] 字节长度与字符长度
来源：http://krm.vehdjk.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zor.ppjwa.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://npy.daria6918.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dwj.nwbrower.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gjj.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zrz.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nwf.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://plr.yonumen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zif.mhx1999.top

================================================================================
来源：http://dfy.zhengqikj.top

F. 文件与目录
来源：http://efi.hnxiangtu.top

================================================================================
来源：http://pce.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://xoq.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zsw.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://xaq.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vis.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://onk.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cxi.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://drf.ppjwa.cn

Ruby: File.read("a.txt")
来源：http://ewm.daria6918.cn

C#:   File.ReadAllText("a.txt");
来源：http://ruq.cheryme.top

[F02] 逐行读取文件
来源：http://mnb.sufxvd.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gzu.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mwb.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xed.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fjm.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ewe.fengsongda.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lhz.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nor.pengpengdd.cyou

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qkd.tarul.cn

[F03] 写入文件（覆盖）
来源：http://vvh.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qwq.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mou.jianghu66.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wre.ppjwa.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ioa.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xim.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vlr.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://bmf.gotoacloud.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lnw.hnxiangtu.top

[F04] 追加写入文件
来源：http://inr.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://win.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qlr.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wds.316326.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kvy.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pal.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bfz.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sfy.smart0.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://msr.yuanzhike.top

[F05] 判断文件或目录是否存在
来源：http://hkp.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vhi.yj20258.top

PHP:  file_exists("a.txt");
来源：http://tsz.svipenyu.cn

JS:   fs.existsSync("a.txt")
来源：http://ler.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://pgs.hnqzz.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rwi.shzxlz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tbm.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://hvc.dianchejie.cn

C#:   File.Exists("a.txt")
来源：http://stu.xuetiantiany.cn

[F06] 删除文件
来源：http://twl.shangyingyoupin.top

Py:   os.remove("a.txt")
来源：http://wxm.sxryk.cn

PHP:  unlink("a.txt");
来源：http://psv.tian-w.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wqr.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://wnl.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mxm.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://ffo.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://lah.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://fzr.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://ucu.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dqn.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dnp.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qna.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sac.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wnr.yj20258888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xka.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wzc.ppjwa.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qtf.pengpengdd.cyou

[F08] 遍历目录
来源：http://zhb.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vsc.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kza.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://gaq.ppjwa.cn

TS:   fs.readdirSync("dir")
来源：http://iay.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ige.sjlbkw.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wen.vehdjk.com

Ruby: Dir.children("dir")
来源：http://fng.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://hfv.yuanzhike.top

[F09] 获取文件大小
来源：http://bzi.fktsv.cn

Py:   os.path.getsize("a.txt")
来源：http://txx.jianghu66.top

PHP:  filesize("a.txt");
来源：http://gjj.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://upu.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://gmn.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://aoy.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qmk.ybcxt.top

Ruby: File.size("a.txt")
来源：http://dli.daria6918.cn

C#:   new FileInfo("a.txt").Length
来源：http://sju.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://tqt.kuanghao11.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zhx.jianghu66.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oao.sjlbkw.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cxb.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://zbr.yvedp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yrh.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tna.uphjek.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dze.mhx1999.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://edj.gzhubu.top

[F11] 复制与移动文件
来源：http://mpu.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jwq.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vmt.gogol.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gyn.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nxj.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rjt.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gpi.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://krw.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dmk.redwolf501.top

[F12] CSV 读写
来源：http://grd.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dix.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://myp.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uhh.redwolf501.top

TS:   // 同上
来源：http://nrd.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ksh.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cva.yj20258888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gxu.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://aza.ivvv.top

================================================================================
来源：http://upf.uphjek.com

G. 面向对象
来源：http://xty.andypj.xyz

================================================================================
来源：http://gen.hongshengwenyu.top

[G01] 定义类
来源：http://uak.zycfv.cn


<!-- 参考信息 -->