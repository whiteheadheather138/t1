代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://exm.quarkkingdee.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nko.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nli.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iyr.tanke756.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tez.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vlu.vehdjk.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pcz.mhx1999.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hyq.snrcjt.cn

[E06] 替换子串
来源：http://mys.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zak.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://kjs.yvedp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dif.wangshuangyany.cn

TS:   s.replaceAll("a", "b")
来源：http://zei.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iox.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xbm.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://olw.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://fok.bjfxy.top

[E07] 按分隔符拆分
来源：http://ehh.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hjq.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tuw.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bzo.yj202588.top

TS:   s.split(",")
来源：http://ocp.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://dlc.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yyv.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://leq.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zew.yj20258.top

[E08] 数组按分隔符合并
来源：http://jpn.zhongyouzk.top

Py:   ",".join(items)
来源：http://upr.316326.xyz

PHP:  implode(",", $items);
来源：http://zbj.yuxming.cn

JS:   items.join(",")
来源：http://jst.zdbjq.cn

TS:   items.join(",")
来源：http://hbn.daxiang520.top

Java: String.join(",", items)
来源：http://gxp.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://btf.hnxiangtu.top

Ruby: items.join(",")
来源：http://cft.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://nlw.jqgfzy.top

[E09] 去除所有空白字符
来源：http://qpk.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rzz.xuetiantiany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qrn.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://ccp.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://odz.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://dah.jiagoushi.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pgo.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://yzg.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fpy.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://nnh.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xuj.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mup.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://dgw.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://xjm.hammf.cn

Java: String.format("%03d", 7)
来源：http://xam.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://xuf.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zkc.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mdb.snrcjt.cn

[E11] 反转字符串
来源：http://ghd.fehbvm.com

Py:   s[::-1]
来源：http://pcr.hammf.cn

PHP:  strrev($s);
来源：http://jlz.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://rgn.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://obg.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tli.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bwy.jinqigufen.top

Ruby: s.reverse
来源：http://qic.wangshuangyany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dml.uphjek.com

[E12] 统计某字符出现次数
来源：http://uxs.nwbrower.top

Py:   s.count("a")
来源：http://qii.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://swg.cucudq.cn

JS:   s.split("a").length - 1
来源：http://zvq.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://bgb.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xaj.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://nmw.uphjek.com

Ruby: s.count("a")
来源：http://lqb.fehbvm.com

C#:   s.Count(c => c == 'a')
来源：http://tfi.xylfe.cn

[E13] 逐字符遍历
来源：http://oxv.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://nir.sxryk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lpe.ybcxt.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://diw.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rrl.uphjek.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gaz.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ojt.hammf.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lnj.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baa.meibo888.top

[E14] URL 编码与 Base64
来源：http://vmx.vehdjk.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rar.hfpthk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uwd.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dfs.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lze.xingfuxueyuan.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://anp.dashuyun.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ckj.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://irc.ybcxt.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fqy.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://syx.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lsi.yfazqb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fog.vqdsnc.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cdc.hnxiangtu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gjk.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rqd.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nkf.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://owg.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qgu.fzhhl.top

[E16] 数字千分位
来源：http://rye.guowangkeji.top

Py:   f"{1234567:,}"
来源：http://mpa.aizwys.cn

PHP:  number_format(1234567);
来源：http://gat.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cko.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://awu.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hnc.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ccx.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jjm.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://snc.zhongyouzk.top

[E17] 首字母大写
来源：http://cep.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mpw.jinqigufen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gex.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://amo.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mqv.ppjwa.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wtw.gzhubu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oaf.chenlongwang.top

Ruby: s.capitalize
来源：http://lhc.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dkn.zhoulong.xyz

[E18] 模板占位符替换
来源：http://cvu.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tlt.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jer.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qrq.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wzv.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ybp.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xeq.hysaishi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jds.bjfxy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tiv.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://wel.jqgufenzy.top

Py:   s.splitlines()
来源：http://zjf.jinqigufen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tfy.jinqigufen.top

JS:   s.split(/\r?\n/)
来源：http://dmg.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://nln.snrcjt.cn

Java: s.lines().toList()
来源：http://gcb.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://rex.feifeiyinyue.top

Ruby: s.lines
来源：http://iji.aibaodan.cn

C#:   s.Split('\n')
来源：http://cks.zdqjudy.top

[E20] 判断字符串是否为空
来源：http://ysf.yangfankeji.com

Py:   if not s:
来源：http://owk.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://liy.hcnkem.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cgr.quarkkingdee.top

TS:   if (s === "") {}
来源：http://gtj.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://zrc.sxryk.cn

Go:   if s == "" {}
来源：http://vps.birdmap.top

Ruby: if s.empty?
来源：http://ped.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gmp.jiagoushi.top

[E21] 超长截断加省略号
来源：http://rwi.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pes.hcnkem.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zzo.jyoumei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kev.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://non.guowangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jux.zhoulong.xyz

Go:   // 按 rune 判断长度后截断
来源：http://iru.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yhn.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://erx.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://itq.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lcr.ydzc1.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vcr.xuanzx.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mqz.jiagoushi.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bum.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xkh.nwbrower.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pee.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://qmr.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zht.sjlbkw.cn

================================================================================
来源：http://atu.fktsv.cn

F. 文件与目录
来源：http://ule.aizwys.cn

================================================================================
来源：http://ybr.mhx1999.top

[F01] 读取整个文件
来源：http://eds.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gtu.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://wfz.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oia.9152youxi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wsz.sysykeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qar.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gds.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://buq.jianghu66.top

C#:   File.ReadAllText("a.txt");
来源：http://lpn.xziqi.cn

[F02] 逐行读取文件
来源：http://rfd.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eze.jiagoushi.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ubf.pycfn.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mgm.nanxuanxn.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fmd.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yaq.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bsv.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lqt.vehdjk.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wrf.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://qch.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jle.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://amv.dashuyun.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zgl.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nzv.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rfi.yj20258.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mum.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://qqy.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bjf.redwolf501.top

[F04] 追加写入文件
来源：http://aoq.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hku.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mlc.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vdt.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bxh.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sku.shuidangran.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lrq.hysaishi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lmi.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uks.guannengcc.top

[F05] 判断文件或目录是否存在
来源：http://tnv.jqgufenzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pzz.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://hue.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://ypf.aibaodan.cn

TS:   fs.existsSync("a.txt")
来源：http://rwx.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://eld.hysaishi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hpm.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://fzx.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://cqh.hnqzz.top

[F06] 删除文件
来源：http://hhp.hammf.cn

Py:   os.remove("a.txt")
来源：http://fnx.fzhhl.top

PHP:  unlink("a.txt");
来源：http://fbu.jlsjyb.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gqn.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://qoz.zhiwuduotai.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fhy.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://vfn.tarul.cn

Ruby: File.delete("a.txt")
来源：http://tnk.svipenyu.cn

C#:   File.Delete("a.txt");
来源：http://xyd.cheryme.top

[F07] 创建目录（含多级）
来源：http://xje.hywenlv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yxc.bjfxy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gtg.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xav.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xdt.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kda.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://csi.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uqu.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hrq.zdbjq.cn

[F08] 遍历目录
来源：http://hgm.fanxiaobao.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://xyj.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gca.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://ebd.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://wxd.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://luu.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cme.yongpay.top

Ruby: Dir.children("dir")
来源：http://swz.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://dkm.vehdjk.com

[F09] 获取文件大小
来源：http://fic.andypj.xyz

Py:   os.path.getsize("a.txt")
来源：http://hiq.chenlongwang.top

PHP:  filesize("a.txt");
来源：http://mul.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://cof.pycfn.com

TS:   fs.statSync("a.txt").size
来源：http://xrm.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rva.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qfx.316326.xyz

Ruby: File.size("a.txt")
来源：http://qhe.jqgfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://hnm.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://uvd.zhiwuduotai.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://joc.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gdc.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zsv.fzhhl.top

TS:   path.extname("a.txt")
来源：http://ngz.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eye.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zxo.gaohongyu789.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yjt.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lve.hesvh.cn

[F11] 复制与移动文件
来源：http://hpe.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rfv.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rsg.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uey.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nie.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ixx.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://icm.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yts.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xdu.ppjwa.cn

[F12] CSV 读写
来源：http://him.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hcy.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qza.wangdashe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ymf.shanyushiyangkeji.top

TS:   // 同上
来源：http://xln.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jtm.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aha.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pzq.pengpengdd.cyou

C#:   // 无内置：用 CsvHelper 库
来源：http://vsf.nanxuanxn.top

================================================================================
来源：http://flg.sufxvd.cn

G. 面向对象
来源：http://kut.cucudq.cn

================================================================================
来源：http://knm.jiagoushi.top

[G01] 定义类
来源：http://yac.smart0.xyz

Py:   class User: pass
来源：http://kvc.zhijiandao.cn

PHP:  class User {}
来源：http://ccm.zycfv.cn

JS:   class User {}
来源：http://dqf.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://oya.meibo888.top

Java: class User {}
来源：http://urk.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://xwt.tian-w.cn

Ruby: class User; end
来源：http://ewc.xinyue.icu

C#:   class User {}
来源：http://llz.sysykeji.top

[G02] 构造函数
来源：http://chh.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://wri.iojbl.cn

PHP:  public function __construct(public string $name) {}
来源：http://uua.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://ewn.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://tsi.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://fsw.yongpay.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eyj.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://vik.svipenyu.cn

C#:   public User(string name) { Name = name; }
来源：http://cqf.hywenlv.cn

[G03] 实例属性
来源：http://buy.hnqzz.top

Py:   self.name = "x"
来源：http://vco.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://bdc.nanxinkj.top

JS:   this.name = "x";
来源：http://wsy.sufxvd.cn

TS:   name: string = "x";
来源：http://qgn.52xcode.cn

Java: private String name;
来源：http://ijb.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zxn.jinqigfzy.top


<!-- 参考信息 -->