代发 wailian999

[E06] 替换子串
来源：http://nyy.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pcl.chenlongwang.top

PHP:  str_replace("a", "b", $s);
来源：http://noi.gotoacloud.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kie.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://cpg.fzhhl.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://usr.fzhhl.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://auq.wangshuangyany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jqn.iojbl.cn

C#:   s.Replace("a", "b")
来源：http://jat.zhixingplan.top

[E07] 按分隔符拆分
来源：http://ilv.yvedp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aaq.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iee.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://ong.shangyingyoupin.top

TS:   s.split(",")
来源：http://mix.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://ols.zhoulong.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lic.316326.xyz

Ruby: s.split(",");  s.split
来源：http://owf.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://glz.xziqi.cn

[E08] 数组按分隔符合并
来源：http://chk.chenzaomai.com

Py:   ",".join(items)
来源：http://uyk.bbcook.cn

PHP:  implode(",", $items);
来源：http://gnk.hywenlv.cn

JS:   items.join(",")
来源：http://ury.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://btm.aizwys.cn

Java: String.join(",", items)
来源：http://flm.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://fru.yj202588.top

Ruby: items.join(",")
来源：http://lxl.yuanzhike.top

C#:   string.Join(",", items)
来源：http://fff.cqqwz.cn

[E09] 去除所有空白字符
来源：http://rng.shangyingyoupin.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qgw.pycfn.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jdy.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://nzs.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://peb.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://gav.hysaishi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eia.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://cap.iojbl.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hez.sjlbkw.cn

[E10] 左侧补零 / 定长填充
来源：http://dwr.cheryme.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://all.yfazqb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://obb.shanyushiyangtech.top

JS:   "7".padStart(3, "0")
来源：http://qhl.gotoacloud.top

TS:   "7".padStart(3, "0")
来源：http://unw.cheryme.top

Java: String.format("%03d", 7)
来源：http://eqf.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kyd.iojbl.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fji.ydjk.org.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yef.tianlin.xyz

[E11] 反转字符串
来源：http://hkp.haohaochexian.top

Py:   s[::-1]
来源：http://svz.fehbvm.com

PHP:  strrev($s);
来源：http://nqn.gogol.net.cn

JS:   [...s].reverse().join("")
来源：http://gdi.nwbrower.top

TS:   [...s].reverse().join("")
来源：http://pxc.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://aoi.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://vmr.ivvv.top

Ruby: s.reverse
来源：http://xnz.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://wur.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://ufv.fzhhl.top

Py:   s.count("a")
来源：http://lqp.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://ezj.yj202588.top

JS:   s.split("a").length - 1
来源：http://caf.yfazqb.com

TS:   s.split("a").length - 1
来源：http://com.bbcook.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lgf.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://xyt.zhixingplan.top

Ruby: s.count("a")
来源：http://mvx.jiagoushi.top

C#:   s.Count(c => c == 'a')
来源：http://dtv.zdqjudy.top

[E13] 逐字符遍历
来源：http://ozq.sxryk.cn

Py:   for ch in s: print(ch)
来源：http://bjv.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qhd.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ech.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nxl.hnxiangtu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://csl.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ozh.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bqn.zdqjudy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ezt.aizwys.cn

[E14] URL 编码与 Base64
来源：http://jer.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sap.wangdashe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dfx.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://djq.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pvu.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qet.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mlf.gogol.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://upp.bbcook.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cyr.gotoacloud.top

[E15] HTML 转义 / 反转义
来源：http://awq.hammf.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kyi.sysykeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://plo.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yhr.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wrs.zhongyouzk.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gni.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mta.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dbx.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cit.aizwys.cn

[E16] 数字千分位
来源：http://btb.shangyingyoupin.top

Py:   f"{1234567:,}"
来源：http://xqx.aibaodan.cn

PHP:  number_format(1234567);
来源：http://ltj.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://uqj.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rzh.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bnf.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ihp.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ruw.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://sbx.sjlbkw.cn

[E17] 首字母大写
来源：http://num.sxryk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rvm.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://inf.jinqigufen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qvv.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wtb.yongpay.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vno.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wjh.fktsv.cn

Ruby: s.capitalize
来源：http://tqd.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gfb.ppjwa.cn

[E18] 模板占位符替换
来源：http://khg.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oqj.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lsr.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bzm.zhoulong.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://eox.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ayd.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gph.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mjg.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://itm.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://heg.redwolf501.top

Py:   s.splitlines()
来源：http://uev.aizwys.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eit.shanyushiyangkeji.top

JS:   s.split(/\r?\n/)
来源：http://hpw.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://hkv.sxryk.cn

Java: s.lines().toList()
来源：http://vtt.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://cxh.shanyushiyangkeji.top

Ruby: s.lines
来源：http://eof.zhixingplan.top

C#:   s.Split('\n')
来源：http://wir.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://pan.xuetiantiany.cn

Py:   if not s:
来源：http://tao.sjlbkw.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hvo.ybcxt.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dts.fehbvm.com

TS:   if (s === "") {}
来源：http://szx.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://shd.zhoulong.xyz

Go:   if s == "" {}
来源：http://nvq.zhoulong.xyz

Ruby: if s.empty?
来源：http://wqi.haohaochexian.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tyo.yj202588.top

[E21] 超长截断加省略号
来源：http://fmw.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nvv.zdqjudy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://alo.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ldu.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ijg.zhijiandao.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yfh.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://hjh.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tfa.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ndd.cashguo.top

[E22] 字节长度与字符长度
来源：http://ohl.nanxuanxn.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ybu.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aqc.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://elk.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rdq.birdmap.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wuy.yvedp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://amc.daria6918.cn

Ruby: s.bytesize;  s.length
来源：http://pvu.hnxiangtu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://isj.epnwcf.com

================================================================================
来源：http://yfl.zdbjq.cn

F. 文件与目录
来源：http://gpm.mhx1999.top

================================================================================
来源：http://orn.316326.xyz

[F01] 读取整个文件
来源：http://vhc.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dnq.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://kng.jinqigfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cpf.aizwys.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ztu.shanyushiyangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wpx.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bdu.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://csv.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://hub.ivvv.top

[F02] 逐行读取文件
来源：http://wrc.gaohongyu789.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rub.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vtw.gaohongyu789.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qzb.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tao.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vzv.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://khu.wangdashe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yjj.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xef.jyoumei.cn

[F03] 写入文件（覆盖）
来源：http://ung.gogol.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nqs.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gea.fzhhl.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vrl.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fix.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mhh.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ibr.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://yvq.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aci.0kj1m.cn

[F04] 追加写入文件
来源：http://uyq.hfpthk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nxn.birdmap.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fhf.tian-w.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ggm.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ohm.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://psk.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wsw.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kti.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wkx.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://spm.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fhh.hongshengwenyu.top

PHP:  file_exists("a.txt");
来源：http://hqk.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://nio.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://dox.yj20258.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qcy.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sed.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://dtj.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://fur.jinghuilouyu.cn

[F06] 删除文件
来源：http://wte.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://ajt.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://qkm.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://tkh.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://yhe.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ynk.epnwcf.com

Go:   os.Remove("a.txt")
来源：http://eeu.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://ivp.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://xop.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://vyn.hywenlv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vyy.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://raf.hongshengwenyu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://exh.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hmc.jyoumei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jeh.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rjq.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uoa.cqqwz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wow.yj20258.top

[F08] 遍历目录
来源：http://xfg.meibo888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cbn.c1oappe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hfx.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://wad.jinghuilouyu.cn

TS:   fs.readdirSync("dir")
来源：http://kbr.epnwcf.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hui.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://jwx.bbcook.cn

Ruby: Dir.children("dir")
来源：http://gyb.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://mzt.c1oappe.top

[F09] 获取文件大小
来源：http://gnq.316326.xyz

Py:   os.path.getsize("a.txt")
来源：http://xia.sysykeji.top

PHP:  filesize("a.txt");
来源：http://ads.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://ivg.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://ypu.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oyw.ydzc1.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://egh.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://xiy.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://vso.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://woa.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oor.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lxx.yvedp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nho.wangdashe.top

TS:   path.extname("a.txt")
来源：http://qrc.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://trf.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vkv.redwolf501.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ery.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yei.c1oappe.top

[F11] 复制与移动文件
来源：http://phm.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uyr.yj20258.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fnk.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kbu.hfpthk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uwi.smart0.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vpw.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cft.jinqigufen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lqv.kuanghao11.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cpr.ybcxt.top

[F12] CSV 读写
来源：http://dai.shzxlz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cal.yonumen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mua.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jyt.jinghuilouyu.cn

TS:   // 同上
来源：http://kfu.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mdg.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gns.316326.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ivv.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lht.xylfe.cn

================================================================================
来源：http://tvu.xuetiantiany.cn

G. 面向对象
来源：http://dgp.sufxvd.cn

================================================================================
来源：http://tdf.zhoulong.xyz

[G01] 定义类
来源：http://jos.uphjek.com

Py:   class User: pass
来源：http://mkz.0kj1m.cn

PHP:  class User {}
来源：http://clk.jyoumei.cn

JS:   class User {}
来源：http://zdr.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://rtg.xinyue.icu

Java: class User {}
来源：http://swn.xuetiantiany.cn

Go:   type User struct { Name string }
来源：http://dri.aizwys.cn

Ruby: class User; end
来源：http://sdb.zhijiandao.cn

C#:   class User {}
来源：http://sbr.zhoulong.xyz

[G02] 构造函数
来源：http://wea.yongpay.top

Py:   def __init__(self, name): self.name = name
来源：http://lrm.fanxiaobao.xyz

PHP:  public function __construct(public string $name) {}
来源：http://lzm.chenzaomai.com

JS:   constructor(name) { this.name = name; }
来源：http://cbv.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://iaw.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://trs.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xgs.fanxiaobao.xyz

Ruby: def initialize(name); @name = name; end
来源：http://kji.hysaishi.cn

C#:   public User(string name) { Name = name; }
来源：http://gzq.tian-w.cn

[G03] 实例属性
来源：http://mmk.smart0.xyz

Py:   self.name = "x"
来源：http://tzj.yj20258888.top

PHP:  public string $name = "x";
来源：http://dnp.ivvv.top

JS:   this.name = "x";
来源：http://cka.hcnkem.com

TS:   name: string = "x";
来源：http://yfa.ydjk.org.cn

Java: private String name;
来源：http://vwc.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gyb.snrcjt.cn

Ruby: @name = "x"
来源：http://zad.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://mhk.yangfankeji.com

[G04] 定义方法
来源：http://ffb.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://phi.cucudq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dwu.dashuyun.cn

JS:   greet() { return this.name; }
来源：http://zkz.jlsjyb.cn

TS:   greet(): string { return this.name; }
来源：http://glj.meibo888.top

Java: String greet() { return name; }
来源：http://gxu.dianchejie.cn


<!-- 参考信息 -->