代发 wailian999

Go:   strings.Index(s, "x")
来源：http://tlk.52xcode.cn

Ruby: s.index("x")
来源：http://obc.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://umw.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rqv.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fwf.guannengcc.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uas.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kzp.redwolf501.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mic.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yiu.svipenyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xgo.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bol.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yny.svipenyu.cn

[E06] 替换子串
来源：http://jnn.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ufp.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://bwh.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bjf.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://qxn.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cjb.cashguo.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gjl.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nej.jyoumei.cn

C#:   s.Replace("a", "b")
来源：http://jkc.shzxlz.cn

[E07] 按分隔符拆分
来源：http://xfy.wangdashe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cfp.fzhhl.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nhz.zdqjudy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pvp.zhiwuduotai.top

TS:   s.split(",")
来源：http://rvj.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://obm.sweek.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lbc.tanke756.top

Ruby: s.split(",");  s.split
来源：http://lhu.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://deg.zycfv.cn

[E08] 数组按分隔符合并
来源：http://zyv.yj20258.top

Py:   ",".join(items)
来源：http://trm.jqgufenzy.top

PHP:  implode(",", $items);
来源：http://xkz.redwolf501.top

JS:   items.join(",")
来源：http://apj.daria6918.cn

TS:   items.join(",")
来源：http://pao.jinqigufen.top

Java: String.join(",", items)
来源：http://ock.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://rvw.hnxiangtu.top

Ruby: items.join(",")
来源：http://dtx.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://lme.cqqwz.cn

[E09] 去除所有空白字符
来源：http://gab.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jls.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vbi.tanke756.top

JS:   s.replace(/\s+/g, "")
来源：http://uxg.jianghu66.top

TS:   s.replace(/\s+/g, "")
来源：http://jcd.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://xcx.quarkkingdee.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://oyn.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://iiv.daria6918.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mhv.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://dqv.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qtf.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dme.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://xlh.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://gxr.smart0.xyz

Java: String.format("%03d", 7)
来源：http://dfr.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pgc.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gcn.tarul.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jok.hammf.cn

[E11] 反转字符串
来源：http://tzd.uphjek.com

Py:   s[::-1]
来源：http://aci.hnqzz.top

PHP:  strrev($s);
来源：http://sze.vehdjk.com

JS:   [...s].reverse().join("")
来源：http://cfg.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://fnn.jlsjyb.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uic.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qnr.gzhubu.top

Ruby: s.reverse
来源：http://mtx.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vnj.vehdjk.com

[E12] 统计某字符出现次数
来源：http://plq.snrcjt.cn

Py:   s.count("a")
来源：http://jnt.snrcjt.cn

PHP:  substr_count($s, "a");
来源：http://adc.xuanzx.com

JS:   s.split("a").length - 1
来源：http://pac.daria6918.cn

TS:   s.split("a").length - 1
来源：http://zgk.xingfuxueyuan.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nng.sxryk.cn

Go:   strings.Count(s, "a")
来源：http://ggc.epnwcf.com

Ruby: s.count("a")
来源：http://gwf.jiagoushi.top

C#:   s.Count(c => c == 'a')
来源：http://mcg.xuetiantiany.cn

[E13] 逐字符遍历
来源：http://vyl.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://awz.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sje.kuanghao11.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ixs.tianlin.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://hyp.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cum.ctjpmb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jas.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lxg.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bwz.cashguo.top

[E14] URL 编码与 Base64
来源：http://fac.redwolf501.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://obp.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bkp.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://svb.zycfv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dsm.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qfi.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yoi.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uwq.jinyuanbaomall.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xsy.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://tti.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nzp.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rxn.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kcq.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://syr.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://axo.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mka.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cnu.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fnh.hesvh.cn

[E16] 数字千分位
来源：http://hez.yj20258888.top

Py:   f"{1234567:,}"
来源：http://tzd.tanke756.top

PHP:  number_format(1234567);
来源：http://hzg.jinqigufen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://oum.yuanzhike.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lkn.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vgg.svipenyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wqe.0kj1m.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yqq.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://pub.jlsjyb.cn

[E17] 首字母大写
来源：http://bem.hnxiangtu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://epw.nanxinkj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tcj.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xaw.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iuf.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ijf.tarul.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sky.jiagoushi.top

Ruby: s.capitalize
来源：http://wtg.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eoc.zycfv.cn

[E18] 模板占位符替换
来源：http://qsn.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rcv.mhx1999.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ica.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fne.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://oen.hcnkem.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://shw.meibo888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nxu.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zks.zhongyouzk.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eiv.hesvh.cn

[E19] 多行文本按行拆分
来源：http://taq.zdqjudy.top

Py:   s.splitlines()
来源：http://bqd.svipenyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://szn.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://kjb.hfpthk.cn

TS:   s.split(/\r?\n/)
来源：http://rqr.ivvv.top

Java: s.lines().toList()
来源：http://ozu.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://ajl.hysaishi.cn

Ruby: s.lines
来源：http://jny.hammf.cn

C#:   s.Split('\n')
来源：http://wdx.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://ktv.fengsongda.top

Py:   if not s:
来源：http://uqj.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gha.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nkk.haohaochexian.top

TS:   if (s === "") {}
来源：http://dwr.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://wxt.ivvv.top

Go:   if s == "" {}
来源：http://hlz.pengpengdd.cyou

Ruby: if s.empty?
来源：http://rrq.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lkf.yonumen.top

[E21] 超长截断加省略号
来源：http://daf.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vdh.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bfa.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hxc.zhoulong.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fna.jlsjyb.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wxp.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://bfh.yj20258888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pdp.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zer.yonumen.top

[E22] 字节长度与字符长度
来源：http://zwi.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ejs.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vsb.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xrh.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ths.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hki.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vwn.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://jci.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gnc.ppjwa.cn

================================================================================
来源：http://ebs.feifeiyinyue.top

F. 文件与目录
来源：http://jtk.sysykeji.top

================================================================================
来源：http://qlg.ehwqpu.com

[F01] 读取整个文件
来源：http://rsx.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zjk.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://kiz.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zyj.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ebg.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nny.cheryme.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oak.uphjek.com

Ruby: File.read("a.txt")
来源：http://hqv.0kj1m.cn

C#:   File.ReadAllText("a.txt");
来源：http://rrt.hywenlv.cn

[F02] 逐行读取文件
来源：http://ump.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eyb.jiagoushi.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hse.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vus.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yfe.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vct.jinyuanbaomall.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gzj.yvedp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kuc.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zcn.wangshuangyany.cn

[F03] 写入文件（覆盖）
来源：http://zhg.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lie.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://thv.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dwh.jqgufenzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ubf.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ozn.chenjidiqi.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sps.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://jlb.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gib.xuetiantiany.cn

[F04] 追加写入文件
来源：http://rma.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tzv.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yhf.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lwc.chenzaomai.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yeu.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zzb.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xlj.bbcook.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gpi.jinghuilouyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kyv.aizwys.cn

[F05] 判断文件或目录是否存在
来源：http://fiq.cdnleiting.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://suf.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://ndy.sufxvd.cn

JS:   fs.existsSync("a.txt")
来源：http://oeq.cheryme.top

TS:   fs.existsSync("a.txt")
来源：http://nbv.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://czx.nwbrower.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uud.yueranfly.top

Ruby: File.exist?("a.txt")
来源：http://lgu.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://odg.quarkkingdee.top

[F06] 删除文件
来源：http://gsi.hysaishi.cn

Py:   os.remove("a.txt")
来源：http://izq.nanxuanxn.top

PHP:  unlink("a.txt");
来源：http://ihx.mhx1999.top

JS:   fs.unlinkSync("a.txt")
来源：http://xns.tian-w.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fmn.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hde.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://kcw.hammf.cn

Ruby: File.delete("a.txt")
来源：http://swv.shanyushiyangkeji.top

C#:   File.Delete("a.txt");
来源：http://ynh.sysykeji.top

[F07] 创建目录（含多级）
来源：http://ipp.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://srr.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zos.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dgl.jinghuilouyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oyb.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://umy.jiagoushi.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pko.hysaishi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lgy.bjfxy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://afd.jinqigufen.top

[F08] 遍历目录
来源：http://xxn.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qes.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rgq.jiagoushi.top

JS:   fs.readdirSync("dir")
来源：http://xog.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://kfa.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hlk.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jef.uphjek.com

Ruby: Dir.children("dir")
来源：http://gic.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://fzl.jinyuanbaomall.cn

[F09] 获取文件大小
来源：http://onl.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://xsu.xylfe.cn

PHP:  filesize("a.txt");
来源：http://bcw.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://kku.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://tna.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://eng.guowangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zui.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://ktw.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://gwp.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://irl.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rum.shzxlz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tfl.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sxd.fehbvm.com

TS:   path.extname("a.txt")
来源：http://fsj.aizwys.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://llo.xinyue.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ram.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://afh.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tla.yangfankeji.com

[F11] 复制与移动文件
来源：http://cvq.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ala.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yly.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ipz.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sly.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://juu.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lkz.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wks.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zqh.jyoumei.cn

[F12] CSV 读写
来源：http://xpz.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sed.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zgz.zhaomingkeji.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ahr.ppjwa.cn

TS:   // 同上
来源：http://wjn.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nep.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nax.tarul.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dsl.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yoj.jianghu66.top

================================================================================
来源：http://adh.chenlongwang.top

G. 面向对象
来源：http://cqr.shanyushiyangkeji.top

================================================================================
来源：http://joy.zycfv.cn

[G01] 定义类
来源：http://qyj.hammf.cn

Py:   class User: pass
来源：http://hpq.daxiang520.top

PHP:  class User {}
来源：http://jyh.dianchejie.cn

JS:   class User {}
来源：http://fth.jlsjyb.cn

TS:   class User { name: string = ""; }
来源：http://lgk.yangfankeji.com

Java: class User {}
来源：http://jge.fengsongda.top

Go:   type User struct { Name string }
来源：http://sbo.jinghuilouyu.cn

Ruby: class User; end
来源：http://xcf.hnxiangtu.top

C#:   class User {}
来源：http://eqy.zhengqikj.top

[G02] 构造函数
来源：http://nia.hfpthk.cn

Py:   def __init__(self, name): self.name = name
来源：http://ljt.gogol.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://drs.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://vff.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://yti.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://bnk.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qvj.daxiang520.top

Ruby: def initialize(name); @name = name; end
来源：http://yzm.yongpay.top

C#:   public User(string name) { Name = name; }
来源：http://tjx.hongshengwenyu.top

[G03] 实例属性
来源：http://nar.hywenlv.cn

Py:   self.name = "x"
来源：http://zfi.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://bmt.pycfn.com


<!-- 参考信息 -->