代发 wailian999

[E02] 重复字符串
来源：http://yeo.jqgfzy.top

Py:   "ab" * 3
来源：http://noc.cqqwz.cn

PHP:  str_repeat("ab", 3);
来源：http://tmn.yfazqb.com

JS:   "ab".repeat(3)
来源：http://cpe.ehwqpu.com

TS:   "ab".repeat(3)
来源：http://oxb.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://ubs.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://fjq.guowangkeji.top

Ruby: "ab" * 3
来源：http://nqg.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qrh.jqgufenzy.top

[E03] 截取子串
来源：http://wwr.hnxiangtu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lts.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kev.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ewy.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://xra.jianghu66.top

Java: s.substring(1, 4)
来源：http://bpl.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iwv.zdbjq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pdc.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://tuo.fengsongda.top

[E04] 查找子串位置
来源：http://ovb.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://gbu.birdmap.top

PHP:  strpos($s, "x");
来源：http://bxb.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lsy.ybcxt.top

TS:   s.indexOf("x")
来源：http://hqv.bjfxy.top

Java: s.indexOf("x")
来源：http://bud.jinqigfzy.top

Go:   strings.Index(s, "x")
来源：http://rbj.xuanzx.com

Ruby: s.index("x")
来源：http://dus.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://rhw.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zwh.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hbl.dianchejie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hun.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nrd.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lzw.meibo888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eoq.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lhi.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zfo.hysaishi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ppj.ivvv.top

[E06] 替换子串
来源：http://mkg.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://itv.cucudq.cn

PHP:  str_replace("a", "b", $s);
来源：http://cje.hongshengwenyu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://smf.guowangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://flt.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yoo.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://scx.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yri.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://zhw.ppjwa.cn

[E07] 按分隔符拆分
来源：http://uah.aizwys.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tht.dashuyun.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nqb.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mst.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://whs.dianchejie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lgg.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pda.sysykeji.top

Ruby: s.split(",");  s.split
来源：http://kfn.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qdz.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://tfw.yonumen.top

Py:   ",".join(items)
来源：http://blp.fanxiaobao.xyz

PHP:  implode(",", $items);
来源：http://jhp.yanxiufei.cn

JS:   items.join(",")
来源：http://nec.hongshengwenyu.top

TS:   items.join(",")
来源：http://ayw.ppjwa.cn

Java: String.join(",", items)
来源：http://qhq.yj202588.top

Go:   strings.Join(items, ",")
来源：http://htm.yvedp.cn

Ruby: items.join(",")
来源：http://edc.gotoacloud.top

C#:   string.Join(",", items)
来源：http://jjj.meibo888.top

[E09] 去除所有空白字符
来源：http://gzq.yj20258888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nzo.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://acn.yj202588.top

JS:   s.replace(/\s+/g, "")
来源：http://eyg.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://yup.iojbl.cn

Java: s.replaceAll("\\s+", "")
来源：http://bor.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xdw.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://kft.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xdk.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://equ.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wqb.chenlongwang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ulf.tarul.cn

JS:   "7".padStart(3, "0")
来源：http://ilj.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://pud.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://lwi.zhaomingkeji.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://csp.quarkkingdee.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://exc.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nic.shzxlz.cn

[E11] 反转字符串
来源：http://jkm.sjlbkw.cn

Py:   s[::-1]
来源：http://bda.chenjidiqi.icu

PHP:  strrev($s);
来源：http://wrh.jinghuilouyu.cn

JS:   [...s].reverse().join("")
来源：http://nbk.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://pzp.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jch.meibo888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ekb.cashguo.top

Ruby: s.reverse
来源：http://lxd.mhx1999.top

C#:   new string(s.Reverse().ToArray())
来源：http://bqf.hesvh.cn

[E12] 统计某字符出现次数
来源：http://thx.shuidangran.top

Py:   s.count("a")
来源：http://elp.jinqigfzy.top

PHP:  substr_count($s, "a");
来源：http://shw.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://yue.52xcode.cn

TS:   s.split("a").length - 1
来源：http://sqc.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nod.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://gnn.yanxiufei.cn

Ruby: s.count("a")
来源：http://qpe.ybcxt.top

C#:   s.Count(c => c == 'a')
来源：http://bgp.0kj1m.cn

[E13] 逐字符遍历
来源：http://cyb.yj20258888.top

Py:   for ch in s: print(ch)
来源：http://zmq.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bkf.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fsb.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://meb.yanxiufei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://btl.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kjp.xuanzx.com

Ruby: s.each_char { |ch| puts ch }
来源：http://tuy.fzhhl.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xes.iojbl.cn

[E14] URL 编码与 Base64
来源：http://vcl.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://enu.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tqw.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ehq.epnwcf.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jcp.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ihx.sjlbkw.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kud.vehdjk.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qiy.jiagoushi.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://awk.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://hrw.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uei.sjlbkw.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kov.9152youxi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xyq.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fli.ivvv.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ars.hfpthk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bti.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://man.yanxiufei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wqq.chenzaomai.com

[E16] 数字千分位
来源：http://fon.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://xau.xuanzx.com

PHP:  number_format(1234567);
来源：http://ocy.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://nge.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wtv.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mug.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://isn.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zap.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://ynh.tarul.cn

[E17] 首字母大写
来源：http://jnx.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ppx.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://inw.feifeiyinyue.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://epl.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cva.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gnv.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fuf.hammf.cn

Ruby: s.capitalize
来源：http://ytg.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fxy.sxryk.cn

[E18] 模板占位符替换
来源：http://ben.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oct.birdmap.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bye.316326.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://woa.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nsd.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aju.ydzc1.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zni.jinghuilouyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mat.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://maz.gaohongyu789.top

[E19] 多行文本按行拆分
来源：http://ieh.bjfxy.top

Py:   s.splitlines()
来源：http://mnr.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qfq.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://aoo.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://jbm.smart0.xyz

Java: s.lines().toList()
来源：http://thw.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://ddu.iojbl.cn

Ruby: s.lines
来源：http://sdy.havefunace.top

C#:   s.Split('\n')
来源：http://sem.zhijiandao.cn

[E20] 判断字符串是否为空
来源：http://dog.gogol.net.cn

Py:   if not s:
来源：http://zso.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sey.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jqg.gogol.net.cn

TS:   if (s === "") {}
来源：http://jko.zhengqikj.top

Java: if (s.isEmpty()) {}
来源：http://bdi.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://jmr.cdnleiting.top

Ruby: if s.empty?
来源：http://zfc.chenlongwang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hss.sysykeji.top

[E21] 超长截断加省略号
来源：http://jdb.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://clb.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zsk.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bmc.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hbp.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nrh.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://bat.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://odc.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jom.zycfv.cn

[E22] 字节长度与字符长度
来源：http://zku.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ing.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mgu.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kfk.jianghu66.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cnz.fehbvm.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://npl.sweek.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fju.zhengqikj.top

Ruby: s.bytesize;  s.length
来源：http://qfn.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xtv.dianchejie.cn

================================================================================
来源：http://dcf.tianlin.xyz

F. 文件与目录
来源：http://oid.jianghu66.top

================================================================================
来源：http://xbf.zhaomingkeji.xyz

[F01] 读取整个文件
来源：http://syw.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://suz.chenzaomai.com

PHP:  file_get_contents("a.txt");
来源：http://gfq.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nyd.sjlbkw.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fnb.feifeiyinyue.top

Java: Files.readString(Path.of("a.txt"))
来源：http://clx.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wra.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://jzb.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://kwy.guowangkeji.top

[F02] 逐行读取文件
来源：http://khc.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vyk.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ygq.svipenyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://avs.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uvm.quarkkingdee.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kge.hnqzz.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vhw.shuidangran.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bzy.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fwn.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://vui.dianchejie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zan.hysaishi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zzh.zdqjudy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://urq.cucudq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vtt.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fmt.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sqd.epnwcf.com

Ruby: File.write("a.txt", "hi")
来源：http://mpj.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kcn.tanke756.top

[F04] 追加写入文件
来源：http://pla.gzhubu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uyy.vehdjk.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://phg.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yeo.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wqm.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uor.wangshuangyany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tiv.hnxiangtu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jdu.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://knl.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://izk.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hnr.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://hku.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://jgj.pengpengdd.cyou

TS:   fs.existsSync("a.txt")
来源：http://yjm.shuidangran.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jgc.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zyu.aizwys.cn

Ruby: File.exist?("a.txt")
来源：http://nne.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://eng.fanxiaobao.xyz

[F06] 删除文件
来源：http://zou.yfazqb.com

Py:   os.remove("a.txt")
来源：http://soo.jlsjyb.cn

PHP:  unlink("a.txt");
来源：http://jrf.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://ryu.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://ice.zhongyouzk.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ykn.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://pcx.cqqwz.cn

Ruby: File.delete("a.txt")
来源：http://dxb.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://uka.aibaodan.cn

[F07] 创建目录（含多级）
来源：http://nlc.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kob.jyoumei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qol.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tnw.0kj1m.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rzg.gotoacloud.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qtz.wangshuangyany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://swy.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nfb.jinqigfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://drk.jinghuilouyu.cn

[F08] 遍历目录
来源：http://rcw.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://csd.kuanghao11.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ccg.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://ujd.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://xdo.pengpengdd.cyou

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ywq.ppjwa.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://smz.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://gcj.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://jbo.guannengcc.top

[F09] 获取文件大小
来源：http://ilg.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://jhg.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://lid.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://ylq.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://zin.xylfe.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mpq.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uxm.dianchejie.cn

Ruby: File.size("a.txt")
来源：http://frn.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://jzm.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://gxr.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xwx.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bty.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://itp.snrcjt.cn

TS:   path.extname("a.txt")
来源：http://rqn.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dwe.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ews.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dmx.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nhg.aibaodan.cn

[F11] 复制与移动文件
来源：http://xeo.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hgi.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ezk.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tda.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lit.cqqwz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://plc.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ysp.9152youxi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gmp.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://epw.sjlbkw.cn

[F12] CSV 读写
来源：http://vlh.xingfuxueyuan.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lcy.redwolf501.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://myu.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gqu.quarkkingdee.top

TS:   // 同上
来源：http://hmj.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ylb.yanxiufei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aoi.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://euz.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://afv.andypj.xyz


<!-- 参考信息 -->