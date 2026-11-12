代发 wailian999

[E06] 替换子串
来源：http://uwz.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cep.jyoumei.cn

PHP:  str_replace("a", "b", $s);
来源：http://euo.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cqw.wangdashe.top

TS:   s.replaceAll("a", "b")
来源：http://oqm.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tev.xuetiantiany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://atj.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gdm.pycfn.com

C#:   s.Replace("a", "b")
来源：http://nik.aizwys.cn

[E07] 按分隔符拆分
来源：http://xfk.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zzw.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mai.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://tft.hcnkem.com

TS:   s.split(",")
来源：http://jqx.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://ylm.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uih.jinqigufen.top

Ruby: s.split(",");  s.split
来源：http://euu.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lpy.bbcook.cn

[E08] 数组按分隔符合并
来源：http://pqs.ivvv.top

Py:   ",".join(items)
来源：http://yhb.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://epj.yueranfly.top

JS:   items.join(",")
来源：http://pjk.yj202588.top

TS:   items.join(",")
来源：http://ntc.aizwys.cn

Java: String.join(",", items)
来源：http://qxg.yvedp.cn

Go:   strings.Join(items, ",")
来源：http://pyf.yanxiufei.cn

Ruby: items.join(",")
来源：http://oaw.xuetiantiany.cn

C#:   string.Join(",", items)
来源：http://bxj.aizwys.cn

[E09] 去除所有空白字符
来源：http://mye.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://isu.aizwys.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bdz.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://ppt.havefunace.top

TS:   s.replace(/\s+/g, "")
来源：http://kzj.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://vdp.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zap.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://doi.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://osf.yangfankeji.com

[E10] 左侧补零 / 定长填充
来源：http://nik.zhixingplan.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rds.dianchejie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mid.nwbrower.top

JS:   "7".padStart(3, "0")
来源：http://men.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://hjx.bbcook.cn

Java: String.format("%03d", 7)
来源：http://cpq.yj202588.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://clm.aizwys.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vsc.svipenyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ync.0kj1m.cn

[E11] 反转字符串
来源：http://eba.zdqjudy.top

Py:   s[::-1]
来源：http://del.jiagoushi.top

PHP:  strrev($s);
来源：http://xpc.xingfuxueyuan.xyz

JS:   [...s].reverse().join("")
来源：http://ith.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://wsv.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://agx.yj202588.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eka.ydjk.org.cn

Ruby: s.reverse
来源：http://xqu.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ifc.ivvv.top

[E12] 统计某字符出现次数
来源：http://sgo.ctjpmb.com

Py:   s.count("a")
来源：http://ijr.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://wpf.jianghu66.top

JS:   s.split("a").length - 1
来源：http://hyk.jiagoushi.top

TS:   s.split("a").length - 1
来源：http://dxl.nanxuanxn.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ltn.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://nge.cqqwz.cn

Ruby: s.count("a")
来源：http://bfg.shanyushiyangtech.top

C#:   s.Count(c => c == 'a')
来源：http://fkr.bjfxy.top

[E13] 逐字符遍历
来源：http://fwv.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://imy.jqgufenzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zgy.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://qbk.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sty.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ggo.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vcg.chenjidiqi.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://wlb.sufxvd.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vjf.tanke756.top

[E14] URL 编码与 Base64
来源：http://ehy.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://elt.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://xdu.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zxc.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tpm.zhiwuduotai.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fjw.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lua.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ima.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lxi.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://aid.gotoacloud.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tdd.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cit.xuetiantiany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zcw.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tds.bjfxy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ady.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pzq.yj20258888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://huk.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kvp.mhx1999.top

[E16] 数字千分位
来源：http://ixh.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://cpu.haohaochexian.top

PHP:  number_format(1234567);
来源：http://ygx.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gbj.redwolf501.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wrv.uphjek.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jhl.jqgufenzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yll.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ika.epnwcf.com

C#:   1234567.ToString("N0")
来源：http://vvf.xinyue.icu

[E17] 首字母大写
来源：http://gqh.cdnleiting.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yvl.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hcj.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zbc.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://how.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://utw.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pxd.birdmap.top

Ruby: s.capitalize
来源：http://xsb.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zsl.yj20258888.top

[E18] 模板占位符替换
来源：http://cke.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kfd.jiagoushi.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://art.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sxw.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zpi.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qnx.xuanzx.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qkc.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://obw.cqqwz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://otr.xziqi.cn

[E19] 多行文本按行拆分
来源：http://wkt.chenzaomai.com

Py:   s.splitlines()
来源：http://dtl.zdqjudy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rpf.tian-w.cn

JS:   s.split(/\r?\n/)
来源：http://ggc.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://gbt.yonumen.top

Java: s.lines().toList()
来源：http://ndr.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://wro.daria6918.cn

Ruby: s.lines
来源：http://osg.pycfn.com

C#:   s.Split('\n')
来源：http://qqg.fengsongda.top

[E20] 判断字符串是否为空
来源：http://lpx.jinqigufen.top

Py:   if not s:
来源：http://cpy.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hjx.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kit.uphjek.com

TS:   if (s === "") {}
来源：http://drf.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://vqg.daxiang520.top

Go:   if s == "" {}
来源：http://ezs.sufxvd.cn

Ruby: if s.empty?
来源：http://azh.bbcook.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vpe.ydzc1.top

[E21] 超长截断加省略号
来源：http://pfh.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hqb.sxryk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://suv.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vem.ctjpmb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fsm.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yla.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://ctp.yuxming.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dus.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hbj.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://zwl.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lze.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ndd.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fhu.zhoulong.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vej.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://emi.xingfuxueyuan.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://akw.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://ivq.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://afu.xylfe.cn

================================================================================
来源：http://jyt.cheryme.top

F. 文件与目录
来源：http://scv.chenlongwang.top

================================================================================
来源：http://vrv.fehbvm.com

[F01] 读取整个文件
来源：http://rgi.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://avx.hongshengwenyu.top

PHP:  file_get_contents("a.txt");
来源：http://lrs.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://riv.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yck.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gjv.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://shl.daria6918.cn

Ruby: File.read("a.txt")
来源：http://sho.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://soe.sweek.top

[F02] 逐行读取文件
来源：http://vgo.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ebo.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zbo.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gcl.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://odu.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wdy.shuidangran.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xhq.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tcd.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rpo.shanyushiyangkeji.top

[F03] 写入文件（覆盖）
来源：http://flt.c1oappe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://man.yanxiufei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hzb.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pkl.cheryme.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yyk.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wgz.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://luw.zhijiandao.cn

Ruby: File.write("a.txt", "hi")
来源：http://scg.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gxm.sufxvd.cn

[F04] 追加写入文件
来源：http://srf.epnwcf.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qww.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fqf.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://urg.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://igq.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hya.hesvh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://epu.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ihr.jinqigfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://obn.shzxlz.cn

[F05] 判断文件或目录是否存在
来源：http://pju.guowangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qkd.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://gdl.guannengcc.top

JS:   fs.existsSync("a.txt")
来源：http://qpj.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://gpt.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://czu.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://smy.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://frk.yongpay.top

C#:   File.Exists("a.txt")
来源：http://hfx.guannengcc.top

[F06] 删除文件
来源：http://kbx.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://exx.zhaomingkeji.xyz

PHP:  unlink("a.txt");
来源：http://ggc.fengsongda.top

JS:   fs.unlinkSync("a.txt")
来源：http://fqh.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://evb.cheryme.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mjb.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://vtz.gogol.net.cn

Ruby: File.delete("a.txt")
来源：http://adv.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://unp.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://oet.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ghm.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ojt.dianchejie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mmo.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vrf.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nxi.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hla.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://osu.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fsa.hysaishi.cn

[F08] 遍历目录
来源：http://fod.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iev.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yzu.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://axs.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://adf.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://irf.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gxm.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://gbv.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://nxi.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://dhb.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://ixg.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://lps.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://hxh.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://jvx.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://jcw.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rcf.tanke756.top

Ruby: File.size("a.txt")
来源：http://dzq.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://cio.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://evw.yuxming.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mta.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://opq.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gjl.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://sab.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://omn.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yvo.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lap.jiagoushi.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pjm.dianchejie.cn

[F11] 复制与移动文件
来源：http://ipp.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kgo.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nix.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nvm.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ewp.tanke756.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kxr.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xbc.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sjn.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ysm.jianghu66.top

[F12] CSV 读写
来源：http://rjr.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fiv.daxiang520.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qyy.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jxp.c1oappe.top

TS:   // 同上
来源：http://ias.tianlin.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://clb.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mvc.ehwqpu.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qqz.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nrw.sysykeji.top

================================================================================
来源：http://fqq.hongshengwenyu.top

G. 面向对象
来源：http://twu.bbcook.cn

================================================================================
来源：http://uah.ivvv.top

[G01] 定义类
来源：http://ewi.jiagoushi.top

Py:   class User: pass
来源：http://ohj.jqgufenzy.top

PHP:  class User {}
来源：http://sac.cheryme.top

JS:   class User {}
来源：http://qyf.cashguo.top

TS:   class User { name: string = ""; }
来源：http://zho.hysaishi.cn

Java: class User {}
来源：http://suc.pengpengdd.cyou

Go:   type User struct { Name string }
来源：http://dad.0kj1m.cn

Ruby: class User; end
来源：http://gwh.guannengcc.top

C#:   class User {}
来源：http://fpt.hfpthk.cn

[G02] 构造函数
来源：http://qma.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://bex.zdbjq.cn

PHP:  public function __construct(public string $name) {}
来源：http://niy.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://lab.quarkkingdee.top

TS:   constructor(public name: string) {}
来源：http://fim.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://pcs.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mxu.sufxvd.cn

Ruby: def initialize(name); @name = name; end
来源：http://nbw.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://boc.ppjwa.cn

[G03] 实例属性
来源：http://xrj.vehdjk.com

Py:   self.name = "x"
来源：http://osd.nanxuanxn.top

PHP:  public string $name = "x";
来源：http://uuu.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://gpm.pycfn.com

TS:   name: string = "x";
来源：http://pje.hysaishi.cn

Java: private String name;
来源：http://esg.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rpr.uphjek.com

Ruby: @name = "x"
来源：http://vmm.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://fme.hysaishi.cn

[G04] 定义方法
来源：http://nia.zhixingplan.top

Py:   def greet(self): return self.name
来源：http://pfi.ppjwa.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kux.ydzc1.top

JS:   greet() { return this.name; }
来源：http://bbl.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://qyp.fengsongda.top

Java: String greet() { return name; }
来源：http://kpt.c1oappe.top


<!-- 参考信息 -->