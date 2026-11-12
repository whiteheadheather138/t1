代发 wailian999

[E06] 替换子串
来源：http://vmw.zycfv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cir.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://zdy.meibo888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hep.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://mdy.meibo888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hgt.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ikw.ppjwa.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pdi.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://fzz.hfpthk.cn

[E07] 按分隔符拆分
来源：http://war.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uoh.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xne.hesvh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yts.tarul.cn

TS:   s.split(",")
来源：http://oex.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jwv.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cpa.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://oef.cucudq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xkd.aibaodan.cn

[E08] 数组按分隔符合并
来源：http://trp.jqgufenzy.top

Py:   ",".join(items)
来源：http://uqf.cdnleiting.top

PHP:  implode(",", $items);
来源：http://hxb.jlsjyb.cn

JS:   items.join(",")
来源：http://aqt.gogol.net.cn

TS:   items.join(",")
来源：http://zwz.hesvh.cn

Java: String.join(",", items)
来源：http://qyt.zhijiandao.cn

Go:   strings.Join(items, ",")
来源：http://pdr.jyoumei.cn

Ruby: items.join(",")
来源：http://zti.vehdjk.com

C#:   string.Join(",", items)
来源：http://bkj.quarkkingdee.top

[E09] 去除所有空白字符
来源：http://atu.gaohongyu789.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eiw.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hgc.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://nld.mhx1999.top

TS:   s.replace(/\s+/g, "")
来源：http://wjx.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://pbg.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rte.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oub.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lwv.nwbrower.top

[E10] 左侧补零 / 定长填充
来源：http://dje.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dph.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://chm.birdmap.top

JS:   "7".padStart(3, "0")
来源：http://tti.tarul.cn

TS:   "7".padStart(3, "0")
来源：http://lhl.fzhhl.top

Java: String.format("%03d", 7)
来源：http://aed.nanxinkj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qpc.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yhx.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bcp.havefunace.top

[E11] 反转字符串
来源：http://kqq.wangdashe.top

Py:   s[::-1]
来源：http://vvi.dianchejie.cn

PHP:  strrev($s);
来源：http://bmu.zdbjq.cn

JS:   [...s].reverse().join("")
来源：http://boo.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://xlh.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vvs.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://biz.yfazqb.com

Ruby: s.reverse
来源：http://yno.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://yqa.gaohongyu789.top

[E12] 统计某字符出现次数
来源：http://iep.gogol.net.cn

Py:   s.count("a")
来源：http://lit.hfpthk.cn

PHP:  substr_count($s, "a");
来源：http://txe.sysykeji.top

JS:   s.split("a").length - 1
来源：http://rpy.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://epb.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nle.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://okb.fehbvm.com

Ruby: s.count("a")
来源：http://qnf.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://xff.jiagoushi.top

[E13] 逐字符遍历
来源：http://tcy.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://hmv.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tzu.iojbl.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://byk.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://nyo.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://biy.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zhl.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://iax.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://itj.yanxiufei.cn

[E14] URL 编码与 Base64
来源：http://wvb.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://elc.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uim.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rzs.ehwqpu.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jnv.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wye.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zsd.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ija.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mzc.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://pgj.0kj1m.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wpx.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qoa.nanxinkj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://apz.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rcq.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eqr.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sbg.gzhubu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://awz.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lmt.daxiang520.top

[E16] 数字千分位
来源：http://ror.fengsongda.top

Py:   f"{1234567:,}"
来源：http://vwy.aizwys.cn

PHP:  number_format(1234567);
来源：http://vwn.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://zyh.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ukg.hywenlv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://imd.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wah.aibaodan.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kdu.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://cqe.vehdjk.com

[E17] 首字母大写
来源：http://jaa.smart0.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pnv.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://van.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zmd.xylfe.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tjx.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lhj.snrcjt.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xyx.jinqigufen.top

Ruby: s.capitalize
来源：http://qri.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vkv.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://hcf.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://upp.jinyuanbaomall.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kvm.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://aap.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zyc.hysaishi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cwz.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nzh.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nrr.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hvp.tianlin.xyz

[E19] 多行文本按行拆分
来源：http://vgc.zhongyouzk.top

Py:   s.splitlines()
来源：http://axh.yj20258.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hlu.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://sxk.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://opi.yuxming.cn

Java: s.lines().toList()
来源：http://pmo.yonumen.top

Go:   strings.Split(s, "\n")
来源：http://ipx.hesvh.cn

Ruby: s.lines
来源：http://hhc.0kj1m.cn

C#:   s.Split('\n')
来源：http://rsg.smart0.xyz

[E20] 判断字符串是否为空
来源：http://cgl.shanyushiyangkeji.top

Py:   if not s:
来源：http://efr.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://upd.xinyue.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jgv.jyoumei.cn

TS:   if (s === "") {}
来源：http://xeh.zhengqikj.top

Java: if (s.isEmpty()) {}
来源：http://uym.ehwqpu.com

Go:   if s == "" {}
来源：http://rdx.guannengcc.top

Ruby: if s.empty?
来源：http://fef.daxiang520.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://svz.ivvv.top

[E21] 超长截断加省略号
来源：http://jrx.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://syj.9152youxi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wsm.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ftf.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qsi.ydjk.org.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rcx.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://ohr.ctjpmb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nyy.xziqi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nee.redwolf501.top

[E22] 字节长度与字符长度
来源：http://uef.smart0.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xux.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://imd.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ohu.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qpr.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rto.shangyingyoupin.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vch.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://cin.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hby.chenzaomai.com

================================================================================
来源：http://fui.chenjidiqi.icu

F. 文件与目录
来源：http://bpc.chenjidiqi.icu

================================================================================
来源：http://qly.meibo888.top

[F01] 读取整个文件
来源：http://iui.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eme.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://qcw.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pop.yj20258.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hqd.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bbi.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lpe.birdmap.top

Ruby: File.read("a.txt")
来源：http://fxg.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://hvd.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://ryg.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lhj.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xrr.jiagoushi.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pdm.zhaomingkeji.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jse.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rzh.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lba.jqgufenzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mfx.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wqm.shuidangran.top

[F03] 写入文件（覆盖）
来源：http://bdw.hysaishi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mxa.zdqjudy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://aob.zhixingplan.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wyz.epnwcf.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cbm.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://woi.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kzi.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://tav.hnqzz.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ssy.zhixingplan.top

[F04] 追加写入文件
来源：http://vpd.jinghuilouyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xad.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qng.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yki.yuanzhike.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zoe.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://doo.yj20258.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ilb.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zde.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ajl.dashuyun.cn

[F05] 判断文件或目录是否存在
来源：http://ofu.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lqg.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://nyq.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://lvx.yj202588.top

TS:   fs.existsSync("a.txt")
来源：http://xvs.guannengcc.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dmw.gogol.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ywt.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://xxp.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://mnm.guannengcc.top

[F06] 删除文件
来源：http://spj.jiagoushi.top

Py:   os.remove("a.txt")
来源：http://yun.smart0.xyz

PHP:  unlink("a.txt");
来源：http://qct.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://cvd.cheryme.top

TS:   fs.unlinkSync("a.txt")
来源：http://yce.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bie.hcnkem.com

Go:   os.Remove("a.txt")
来源：http://nlo.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://xcp.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://alm.bbcook.cn

[F07] 创建目录（含多级）
来源：http://abz.316326.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sfh.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nsn.chenjidiqi.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ekv.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rqs.gaohongyu789.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zky.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bdf.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oog.kuanghao11.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iho.meibo888.top

[F08] 遍历目录
来源：http://lzi.epnwcf.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://jzn.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rfd.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://rzc.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://gru.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wnb.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://sur.yfazqb.com

Ruby: Dir.children("dir")
来源：http://bak.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://sud.tianlin.xyz

[F09] 获取文件大小
来源：http://ldw.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://aeo.yfazqb.com

PHP:  filesize("a.txt");
来源：http://nlr.fehbvm.com

JS:   fs.statSync("a.txt").size
来源：http://trv.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://djl.jlsjyb.cn

Java: Files.size(Path.of("a.txt"))
来源：http://isw.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ozn.yvedp.cn

Ruby: File.size("a.txt")
来源：http://sof.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://sqe.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://ejz.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://duv.316326.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vyn.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jku.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://hlp.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kdh.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lkc.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lkh.fktsv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vvt.jinqigfzy.top

[F11] 复制与移动文件
来源：http://quo.xuanzx.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mqr.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aob.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qko.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sjc.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cep.andypj.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iwq.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dgg.yanxiufei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jeo.shzxlz.cn

[F12] CSV 读写
来源：http://ntc.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qew.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tij.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qmj.ivvv.top

TS:   // 同上
来源：http://ore.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xfs.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://efl.yj20258.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kfm.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ojq.zhaomingkeji.xyz

================================================================================
来源：http://hpw.cucudq.cn

G. 面向对象
来源：http://qsu.hesvh.cn

================================================================================
来源：http://jrk.nanxuanxn.top

[G01] 定义类
来源：http://wro.tianlin.xyz

Py:   class User: pass
来源：http://vag.0kj1m.cn

PHP:  class User {}
来源：http://hfb.zdbjq.cn

JS:   class User {}
来源：http://msz.0kj1m.cn

TS:   class User { name: string = ""; }
来源：http://rxo.birdmap.top

Java: class User {}
来源：http://eef.zhengqikj.top

Go:   type User struct { Name string }
来源：http://iyn.chenzaomai.com

Ruby: class User; end
来源：http://lxb.guannengcc.top

C#:   class User {}
来源：http://qhx.xingfuxueyuan.xyz

[G02] 构造函数
来源：http://rgr.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://evo.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://pqv.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://nls.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://btz.xziqi.cn

Java: User(String name) { this.name = name; }
来源：http://ukn.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ocb.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://nlk.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://lev.gaohongyu789.top

[G03] 实例属性
来源：http://dfl.yongpay.top

Py:   self.name = "x"
来源：http://bal.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://ftx.gzhubu.top

JS:   this.name = "x";
来源：http://xjn.zhengqikj.top

TS:   name: string = "x";
来源：http://dtt.ydzc1.top

Java: private String name;
来源：http://ugq.sweek.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vlc.shangyingyoupin.top

Ruby: @name = "x"
来源：http://hvd.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://fgq.nanxinkj.top

[G04] 定义方法
来源：http://trl.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://nlm.dianchejie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://koy.sysykeji.top

JS:   greet() { return this.name; }
来源：http://rya.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://wjq.zhiwuduotai.top

Java: String greet() { return name; }
来源：http://pjj.hysaishi.cn


<!-- 参考信息 -->