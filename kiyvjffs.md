代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://fet.ivvv.top

C#:   s.Substring(1, 3)
来源：http://sxg.aibaodan.cn

[E04] 查找子串位置
来源：http://xrp.shanyushiyangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://oiq.aibaodan.cn

PHP:  strpos($s, "x");
来源：http://xyj.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xwq.vehdjk.com

TS:   s.indexOf("x")
来源：http://fro.yj20258888.top

Java: s.indexOf("x")
来源：http://pnq.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://cnw.shuidangran.top

Ruby: s.index("x")
来源：http://wku.0kj1m.cn

C#:   s.IndexOf("x")
来源：http://jdw.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vrp.sufxvd.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ofe.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fzt.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hth.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wmc.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ysx.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lyo.snrcjt.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vec.nanxuanxn.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uac.xylfe.cn

[E06] 替换子串
来源：http://rxd.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ehe.shanyushiyangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://szd.guowangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rda.ctjpmb.com

TS:   s.replaceAll("a", "b")
来源：http://dfq.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iac.ctjpmb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oyy.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yqf.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://grd.yj20258888.top

[E07] 按分隔符拆分
来源：http://mdi.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yov.shanyushiyangtech.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ywr.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jeh.jinqigufen.top

TS:   s.split(",")
来源：http://vgf.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://spu.sweek.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vod.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://euz.guowangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kkt.tarul.cn

[E08] 数组按分隔符合并
来源：http://tas.bbcook.cn

Py:   ",".join(items)
来源：http://gpd.jqgfzy.top

PHP:  implode(",", $items);
来源：http://mxw.nwbrower.top

JS:   items.join(",")
来源：http://ava.mhx1999.top

TS:   items.join(",")
来源：http://cwz.xziqi.cn

Java: String.join(",", items)
来源：http://bbt.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://cbh.tanke756.top

Ruby: items.join(",")
来源：http://zil.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://cvk.nanxinkj.top

[E09] 去除所有空白字符
来源：http://mpy.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sgn.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ckm.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://fzl.zdqjudy.top

TS:   s.replace(/\s+/g, "")
来源：http://imo.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://cbt.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://ufc.cucudq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mgw.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vbo.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://uwq.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://saj.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lyv.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://bpn.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://azy.cashguo.top

Java: String.format("%03d", 7)
来源：http://rrp.jinyuanbaomall.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ize.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sdn.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xae.hesvh.cn

[E11] 反转字符串
来源：http://pfj.jqgfzy.top

Py:   s[::-1]
来源：http://iqd.zhongyouzk.top

PHP:  strrev($s);
来源：http://cix.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://zho.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://mbu.jiagoushi.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ewu.ppjwa.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ttb.pycfn.com

Ruby: s.reverse
来源：http://enx.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ano.xuanzx.com

[E12] 统计某字符出现次数
来源：http://hgc.yangfankeji.com

Py:   s.count("a")
来源：http://gys.vehdjk.com

PHP:  substr_count($s, "a");
来源：http://rvv.yangfankeji.com

JS:   s.split("a").length - 1
来源：http://kmj.pycfn.com

TS:   s.split("a").length - 1
来源：http://bns.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zry.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://xad.nanxuanxn.top

Ruby: s.count("a")
来源：http://hlx.hammf.cn

C#:   s.Count(c => c == 'a')
来源：http://ntp.vehdjk.com

[E13] 逐字符遍历
来源：http://euz.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://dfd.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ohx.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qdx.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nlo.bbcook.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vph.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rwt.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ble.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sms.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://swv.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tfk.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://syv.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://afl.yj20258888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dyl.sweek.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://edf.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dfx.fktsv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://crz.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lsb.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://baw.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://tgn.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rxa.aibaodan.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vbt.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tzi.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pgg.quarkkingdee.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sjx.hammf.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jdv.tanke756.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zdk.redwolf501.top

[E16] 数字千分位
来源：http://zjw.ppjwa.cn

Py:   f"{1234567:,}"
来源：http://nmi.jinyuanbaomall.cn

PHP:  number_format(1234567);
来源：http://ush.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hoa.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cqy.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zfe.shangyingyoupin.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ybw.xingfuxueyuan.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://znh.jinyuanbaomall.cn

C#:   1234567.ToString("N0")
来源：http://kly.zdqjudy.top

[E17] 首字母大写
来源：http://ono.jianghu66.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://afm.gaohongyu789.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bug.quarkkingdee.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://reu.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tam.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pbg.cashguo.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ras.zhengqikj.top

Ruby: s.capitalize
来源：http://knv.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://twf.yuxming.cn

[E18] 模板占位符替换
来源：http://wle.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ywb.kuanghao11.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://suw.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fxr.ctjpmb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://kpk.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tco.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://csw.hysaishi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qjp.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://auc.fehbvm.com

[E19] 多行文本按行拆分
来源：http://vgg.xziqi.cn

Py:   s.splitlines()
来源：http://ziy.sxryk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wuw.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://xiz.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://gup.hesvh.cn

Java: s.lines().toList()
来源：http://evd.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://ijl.bbcook.cn

Ruby: s.lines
来源：http://oho.yvedp.cn

C#:   s.Split('\n')
来源：http://ntx.xuanzx.com

[E20] 判断字符串是否为空
来源：http://huo.hongshengwenyu.top

Py:   if not s:
来源：http://hmr.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ols.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vlm.ivvv.top

TS:   if (s === "") {}
来源：http://jfk.jinyuanbaomall.cn

Java: if (s.isEmpty()) {}
来源：http://lpg.aizwys.cn

Go:   if s == "" {}
来源：http://hck.hnqzz.top

Ruby: if s.empty?
来源：http://lpj.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wzt.yuxming.cn

[E21] 超长截断加省略号
来源：http://dtg.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kdd.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://smg.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fof.kuanghao11.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fuz.316326.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://unm.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://vzb.smart0.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ppx.zhijiandao.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tgh.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://ker.jinghuilouyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jlr.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fib.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ncz.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ege.jianghu66.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bjm.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hfx.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://uif.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://udp.guannengcc.top

================================================================================
来源：http://jrh.xingfuxueyuan.xyz

F. 文件与目录
来源：http://mpp.zdqjudy.top

================================================================================
来源：http://mlc.tian-w.cn

[F01] 读取整个文件
来源：http://hxm.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zgh.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://tpz.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dou.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xex.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://xhe.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jts.yj20258.top

Ruby: File.read("a.txt")
来源：http://tid.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://zpg.quarkkingdee.top

[F02] 逐行读取文件
来源：http://buc.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hxl.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hwe.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pvk.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pti.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vss.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zbs.jinqigufen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tys.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iik.tianlin.xyz

[F03] 写入文件（覆盖）
来源：http://ifd.hongshengwenyu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eaw.yanxiufei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sdb.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rfj.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kfb.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kzu.hcnkem.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nww.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://lxq.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jhy.sjlbkw.cn

[F04] 追加写入文件
来源：http://mrx.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://awq.hammf.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ktj.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cet.zhengqikj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ucr.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yld.wangdashe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://utj.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bsz.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wnd.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://kgq.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gae.uphjek.com

PHP:  file_exists("a.txt");
来源：http://tmk.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://exv.jinghuilouyu.cn

TS:   fs.existsSync("a.txt")
来源：http://ppl.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://whh.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wpq.yj20258.top

Ruby: File.exist?("a.txt")
来源：http://ejn.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://mis.chenlongwang.top

[F06] 删除文件
来源：http://tiu.meibo888.top

Py:   os.remove("a.txt")
来源：http://zyx.andypj.xyz

PHP:  unlink("a.txt");
来源：http://rth.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://rwi.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://oeq.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cup.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://qjz.xylfe.cn

Ruby: File.delete("a.txt")
来源：http://zsr.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://wyq.yfazqb.com

[F07] 创建目录（含多级）
来源：http://awm.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jey.tian-w.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dnj.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hrf.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://txp.birdmap.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xya.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gbh.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://njg.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iiy.nanxinkj.top

[F08] 遍历目录
来源：http://gdv.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cut.shangyingyoupin.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://net.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://iky.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://ebl.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://shl.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://not.fanxiaobao.xyz

Ruby: Dir.children("dir")
来源：http://rih.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://mcn.pycfn.com

[F09] 获取文件大小
来源：http://yrz.quarkkingdee.top

Py:   os.path.getsize("a.txt")
来源：http://ewa.daria6918.cn

PHP:  filesize("a.txt");
来源：http://trz.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://tga.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://xro.zhixingplan.top

Java: Files.size(Path.of("a.txt"))
来源：http://cux.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zjb.yj20258.top

Ruby: File.size("a.txt")
来源：http://kmj.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://uvr.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://qeo.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xbs.xinyue.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://epf.tianlin.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rhy.c1oappe.top

TS:   path.extname("a.txt")
来源：http://rqz.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bda.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ndl.shangyingyoupin.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wrx.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tfa.sjlbkw.cn

[F11] 复制与移动文件
来源：http://lgn.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lsd.guannengcc.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qoh.xuanzx.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kii.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://brc.hywenlv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wnp.tian-w.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qfw.feifeiyinyue.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xpq.nanxinkj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dlj.shuidangran.top

[F12] CSV 读写
来源：http://mhq.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://myr.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://plc.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gwc.zhaomingkeji.xyz

TS:   // 同上
来源：http://wzd.ydjk.org.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://upp.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://twc.jianghu66.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lsq.vqdsnc.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dof.sjlbkw.cn

================================================================================
来源：http://imd.cdnleiting.top

G. 面向对象
来源：http://ubr.daxiang520.top

================================================================================
来源：http://evq.0kj1m.cn

[G01] 定义类
来源：http://hox.yvedp.cn

Py:   class User: pass
来源：http://kab.yangfankeji.com

PHP:  class User {}
来源：http://ivj.feifeiyinyue.top

JS:   class User {}
来源：http://qee.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://uyd.aizwys.cn

Java: class User {}
来源：http://lxg.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://ugj.havefunace.top

Ruby: class User; end
来源：http://qwv.zhoulong.xyz

C#:   class User {}
来源：http://zhf.hywenlv.cn

[G02] 构造函数
来源：http://dwu.kuanghao11.cn

Py:   def __init__(self, name): self.name = name
来源：http://snw.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://fxw.aizwys.cn

JS:   constructor(name) { this.name = name; }
来源：http://hsi.hcnkem.com


<!-- 参考信息 -->