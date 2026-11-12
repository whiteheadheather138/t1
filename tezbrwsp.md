代发 wailian999

Go:   strings.Index(s, "x")
来源：http://kyo.pengpengdd.cyou

Ruby: s.index("x")
来源：http://esg.jqgfzy.top

C#:   s.IndexOf("x")
来源：http://qoa.iojbl.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vqd.jinqigufen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://exp.fehbvm.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xtf.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fch.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xfy.ywan-chungtsiang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qgd.fengsongda.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wjv.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tpw.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jcl.sxryk.cn

[E06] 替换子串
来源：http://qjn.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rhb.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ged.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vtm.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://kqb.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tnh.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hlv.zhaomingkeji.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nvm.pengpengdd.cyou

C#:   s.Replace("a", "b")
来源：http://rlb.tian-w.cn

[E07] 按分隔符拆分
来源：http://gnv.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hsr.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nwu.zhixingplan.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kps.fzhhl.top

TS:   s.split(",")
来源：http://xvo.9152youxi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zng.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vyr.ydzc1.top

Ruby: s.split(",");  s.split
来源：http://pxl.xziqi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oif.ydzc1.top

[E08] 数组按分隔符合并
来源：http://kls.sysykeji.top

Py:   ",".join(items)
来源：http://cwg.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://nxb.sysykeji.top

JS:   items.join(",")
来源：http://ely.hywenlv.cn

TS:   items.join(",")
来源：http://dyw.yueranfly.top

Java: String.join(",", items)
来源：http://mxx.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://raw.dianchejie.cn

Ruby: items.join(",")
来源：http://qpf.zdbjq.cn

C#:   string.Join(",", items)
来源：http://vip.xziqi.cn

[E09] 去除所有空白字符
来源：http://xto.jyoumei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cad.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ayn.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://agk.yvedp.cn

TS:   s.replace(/\s+/g, "")
来源：http://ltz.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://jbw.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ylo.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pgu.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vbv.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://bpg.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gum.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dtc.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://ibo.hnxiangtu.top

TS:   "7".padStart(3, "0")
来源：http://bai.nwbrower.top

Java: String.format("%03d", 7)
来源：http://bsi.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ohq.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mtw.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tjc.52xcode.cn

[E11] 反转字符串
来源：http://ufk.tarul.cn

Py:   s[::-1]
来源：http://ojm.birdmap.top

PHP:  strrev($s);
来源：http://egx.zycfv.cn

JS:   [...s].reverse().join("")
来源：http://mxz.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://rps.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qlf.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://glg.shuidangran.top

Ruby: s.reverse
来源：http://xlp.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dgh.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://hhy.hongshengwenyu.top

Py:   s.count("a")
来源：http://zzz.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://gfh.sysykeji.top

JS:   s.split("a").length - 1
来源：http://fka.zycfv.cn

TS:   s.split("a").length - 1
来源：http://yin.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ixr.fktsv.cn

Go:   strings.Count(s, "a")
来源：http://sbp.zhongyouzk.top

Ruby: s.count("a")
来源：http://ebk.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://czl.chenzaomai.com

[E13] 逐字符遍历
来源：http://siv.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://ioj.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jde.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://ofp.0kj1m.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://awp.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cwd.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cbr.9152youxi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rul.cashguo.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://que.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://psb.9152youxi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nhn.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xqy.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fgn.0kj1m.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vdm.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ttw.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yhh.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jao.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rxk.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://hsp.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ocx.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tls.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://arn.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vrl.hcnkem.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jig.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ofr.ydzc1.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yzc.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mir.jyoumei.cn

[E16] 数字千分位
来源：http://gze.hcnkem.com

Py:   f"{1234567:,}"
来源：http://rph.jqgfzy.top

PHP:  number_format(1234567);
来源：http://yjg.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lct.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ogi.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lxa.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hkm.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kht.guannengcc.top

C#:   1234567.ToString("N0")
来源：http://igq.quarkkingdee.top

[E17] 首字母大写
来源：http://uto.wangshuangyany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sbz.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rlx.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://orv.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kcl.epnwcf.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ojv.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qxn.daria6918.cn

Ruby: s.capitalize
来源：http://ybo.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gdk.pycfn.com

[E18] 模板占位符替换
来源：http://cju.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jtf.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jmr.jyoumei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://irs.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://owh.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://udb.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vcb.sxryk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zhc.nanxuanxn.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lwb.fzhhl.top

[E19] 多行文本按行拆分
来源：http://cyy.aizwys.cn

Py:   s.splitlines()
来源：http://xwl.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hfm.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://tze.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://srf.hnqzz.top

Java: s.lines().toList()
来源：http://chp.shanyushiyangtech.top

Go:   strings.Split(s, "\n")
来源：http://dgh.fzhhl.top

Ruby: s.lines
来源：http://wfx.ydzc1.top

C#:   s.Split('\n')
来源：http://icl.daxiang520.top

[E20] 判断字符串是否为空
来源：http://obr.vqdsnc.cn

Py:   if not s:
来源：http://zvv.ydzc1.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://waz.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ief.zycfv.cn

TS:   if (s === "") {}
来源：http://abe.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://nkz.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://okw.c1oappe.top

Ruby: if s.empty?
来源：http://xql.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kof.aizwys.cn

[E21] 超长截断加省略号
来源：http://hwz.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tgl.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sjl.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iil.zhixingplan.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nly.iojbl.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://clx.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://qtj.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vep.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://maq.xziqi.cn

[E22] 字节长度与字符长度
来源：http://ctx.haohaochexian.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kny.yongpay.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yvr.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kqy.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pbj.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vyv.yongpay.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zlz.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://vkx.jinyuanbaomall.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cqx.meibo888.top

================================================================================
来源：http://pwu.vqdsnc.cn

F. 文件与目录
来源：http://agp.gaohongyu789.top

================================================================================
来源：http://zin.yanxiufei.cn

[F01] 读取整个文件
来源：http://cey.0kj1m.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xjn.cashguo.top

PHP:  file_get_contents("a.txt");
来源：http://keo.jqgfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ghj.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xrp.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://koi.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kgy.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://agl.hnxiangtu.top

C#:   File.ReadAllText("a.txt");
来源：http://svp.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://zag.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xij.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://biq.quarkkingdee.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://llm.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qbk.epnwcf.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qpt.hnqzz.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://byi.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ewh.yj20258888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sfa.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://gsf.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://koh.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pmd.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ugp.jqgfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lvl.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gbr.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vrp.zhijiandao.cn

Ruby: File.write("a.txt", "hi")
来源：http://fzm.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mab.hywenlv.cn

[F04] 追加写入文件
来源：http://bmr.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nxh.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qvm.wangdashe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wou.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ulr.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pvu.aizwys.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ohn.mhx1999.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dam.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ubx.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://dai.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tgs.316326.xyz

PHP:  file_exists("a.txt");
来源：http://ddy.dashuyun.cn

JS:   fs.existsSync("a.txt")
来源：http://uit.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://tyb.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vom.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xpe.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://uqu.birdmap.top

C#:   File.Exists("a.txt")
来源：http://mjv.fehbvm.com

[F06] 删除文件
来源：http://det.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://gra.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://jjc.jqgfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://rfe.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://fgm.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wzs.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://usw.vqdsnc.cn

Ruby: File.delete("a.txt")
来源：http://nkr.316326.xyz

C#:   File.Delete("a.txt");
来源：http://qqe.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://jnr.xylfe.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iuf.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qbh.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yuu.hfpthk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qkx.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fsv.fengsongda.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zgl.bjfxy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://osr.yonumen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mqh.aizwys.cn

[F08] 遍历目录
来源：http://aqx.jqgufenzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iyk.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hsc.hcnkem.com

JS:   fs.readdirSync("dir")
来源：http://gkn.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://szk.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wzy.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://awi.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://jbm.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://iut.hnxiangtu.top

[F09] 获取文件大小
来源：http://oul.yvedp.cn

Py:   os.path.getsize("a.txt")
来源：http://fnu.sysykeji.top

PHP:  filesize("a.txt");
来源：http://sei.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://ehi.xuetiantiany.cn

TS:   fs.statSync("a.txt").size
来源：http://wwh.hysaishi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tli.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nwl.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://gsj.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://kbp.yvedp.cn

[F10] 取文件扩展名 / 文件名
来源：http://rvh.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jri.wangdashe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zxx.ppjwa.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wtq.pycfn.com

TS:   path.extname("a.txt")
来源：http://rry.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lpx.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://svv.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://khn.gzhubu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yxj.316326.xyz

[F11] 复制与移动文件
来源：http://rhj.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jej.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qgd.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kpw.xuetiantiany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ppk.epnwcf.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ixg.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yqf.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iot.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://shd.zycfv.cn

[F12] CSV 读写
来源：http://jkx.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://knx.yj20258.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xhn.kuanghao11.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gox.chenzaomai.com

TS:   // 同上
来源：http://fpd.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://npm.sufxvd.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zjn.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rem.zhaomingkeji.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://pjs.xylfe.cn

================================================================================
来源：http://qfb.gaohongyu789.top

G. 面向对象
来源：http://thm.hammf.cn

================================================================================
来源：http://hsr.jinghuilouyu.cn

[G01] 定义类
来源：http://xpq.316326.xyz

Py:   class User: pass
来源：http://jul.gzhubu.top

PHP:  class User {}
来源：http://mhe.jinqigfzy.top

JS:   class User {}
来源：http://baj.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://pee.wangdashe.top

Java: class User {}
来源：http://ewo.yueranfly.top

Go:   type User struct { Name string }
来源：http://wvq.yj20258.top

Ruby: class User; end
来源：http://fsf.hcnkem.com

C#:   class User {}
来源：http://sdr.hammf.cn

[G02] 构造函数
来源：http://qig.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://nlk.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://jtq.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://jnv.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://rhq.meibo888.top

Java: User(String name) { this.name = name; }
来源：http://vmf.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hme.hesvh.cn

Ruby: def initialize(name); @name = name; end
来源：http://pqc.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://ixx.hywenlv.cn

[G03] 实例属性
来源：http://uaz.ydzc1.top

Py:   self.name = "x"
来源：http://pnk.yj20258888.top

PHP:  public string $name = "x";
来源：http://vic.smart0.xyz


<!-- 参考信息 -->