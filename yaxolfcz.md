代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://ptl.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qtj.ydzc1.top

Ruby: s.gsub(/\s+/, "")
来源：http://jqe.cucudq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uxf.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://box.daria6918.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vbo.fktsv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ths.vqdsnc.cn

JS:   "7".padStart(3, "0")
来源：http://vfh.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://ktd.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://pji.mhx1999.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lme.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ocw.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pei.bjfxy.top

[E11] 反转字符串
来源：http://xrl.sysykeji.top

Py:   s[::-1]
来源：http://lfw.pycfn.com

PHP:  strrev($s);
来源：http://mgc.hfpthk.cn

JS:   [...s].reverse().join("")
来源：http://fbb.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://rzt.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yum.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ybu.cucudq.cn

Ruby: s.reverse
来源：http://aks.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uhj.jiagoushi.top

[E12] 统计某字符出现次数
来源：http://kmi.xingfuxueyuan.xyz

Py:   s.count("a")
来源：http://jax.sweek.top

PHP:  substr_count($s, "a");
来源：http://kbm.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://hrn.zhoulong.xyz

TS:   s.split("a").length - 1
来源：http://alc.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kmh.yj202588.top

Go:   strings.Count(s, "a")
来源：http://pbo.yvedp.cn

Ruby: s.count("a")
来源：http://dmk.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://swm.chenlongwang.top

[E13] 逐字符遍历
来源：http://jkj.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://iun.dianchejie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qgz.vqdsnc.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://opu.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://olr.ivvv.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jne.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://taq.shangyingyoupin.top

Ruby: s.each_char { |ch| puts ch }
来源：http://izf.zhixingplan.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jrc.shangyingyoupin.top

[E14] URL 编码与 Base64
来源：http://iuv.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mer.yueranfly.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vhr.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lxt.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iug.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jrn.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://doe.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jhv.kuanghao11.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ygy.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://vrz.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://jms.sysykeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iyk.bjfxy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qhq.chenlongwang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://szb.hesvh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vke.hnqzz.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xuj.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rwo.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eeq.52xcode.cn

[E16] 数字千分位
来源：http://rxv.chenjidiqi.icu

Py:   f"{1234567:,}"
来源：http://gjb.guowangkeji.top

PHP:  number_format(1234567);
来源：http://kzu.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://bvk.yuanzhike.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xgv.jinyuanbaomall.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://chi.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tpf.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gtx.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://qnf.ydjk.org.cn

[E17] 首字母大写
来源：http://ukh.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sfe.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://kox.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vif.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jip.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sbs.fengsongda.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bik.yuanzhike.top

Ruby: s.capitalize
来源：http://ssv.zhengqikj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gtd.sxryk.cn

[E18] 模板占位符替换
来源：http://uyc.hnqzz.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aal.gotoacloud.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vtq.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ljc.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://oif.smart0.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ama.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rdr.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://egg.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://htm.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://ipr.xylfe.cn

Py:   s.splitlines()
来源：http://ycb.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cxo.hnxiangtu.top

JS:   s.split(/\r?\n/)
来源：http://vsl.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://fhl.dashuyun.cn

Java: s.lines().toList()
来源：http://baa.tanke756.top

Go:   strings.Split(s, "\n")
来源：http://iwo.jiagoushi.top

Ruby: s.lines
来源：http://obh.hongshengwenyu.top

C#:   s.Split('\n')
来源：http://llm.bjfxy.top

[E20] 判断字符串是否为空
来源：http://wpz.quarkkingdee.top

Py:   if not s:
来源：http://zup.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://viz.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lvl.sufxvd.cn

TS:   if (s === "") {}
来源：http://xxy.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://hyi.316326.xyz

Go:   if s == "" {}
来源：http://wto.haohaochexian.top

Ruby: if s.empty?
来源：http://fxc.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://otl.nwbrower.top

[E21] 超长截断加省略号
来源：http://ohw.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wrb.52xcode.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jed.zhiwuduotai.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hir.xuetiantiany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://srv.c1oappe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fqz.hammf.cn

Go:   // 按 rune 判断长度后截断
来源：http://pov.pengpengdd.cyou

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jur.jyoumei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bow.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://lpg.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yrl.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sru.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hnu.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nnb.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xzl.hywenlv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sif.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://hix.shanyushiyangtech.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tob.aibaodan.cn

================================================================================
来源：http://tyh.jyoumei.cn

F. 文件与目录
来源：http://kcb.jiagoushi.top

================================================================================
来源：http://wyw.ivvv.top

[F01] 读取整个文件
来源：http://oky.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yof.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://kuo.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://frg.9152youxi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://osr.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://lhl.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://khj.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://kjl.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://fuv.jlsjyb.cn

[F02] 逐行读取文件
来源：http://wpm.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fse.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://isr.jyoumei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cbt.gaohongyu789.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dck.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hxq.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gmf.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vur.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://naf.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://cyg.chenzaomai.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cct.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://mhd.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ywe.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ikv.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nrn.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xgj.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://tot.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oad.pengpengdd.cyou

[F04] 追加写入文件
来源：http://vhc.epnwcf.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cim.fengsongda.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nvm.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vcz.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xku.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lxh.chenjidiqi.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fsh.gogol.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://maa.hammf.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vfg.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://gjm.tanke756.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eda.shangyingyoupin.top

PHP:  file_exists("a.txt");
来源：http://luo.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://kym.shzxlz.cn

TS:   fs.existsSync("a.txt")
来源：http://imm.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ply.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ggn.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://tqp.yonumen.top

C#:   File.Exists("a.txt")
来源：http://bpj.uphjek.com

[F06] 删除文件
来源：http://iit.wangdashe.top

Py:   os.remove("a.txt")
来源：http://vjv.daxiang520.top

PHP:  unlink("a.txt");
来源：http://llg.birdmap.top

JS:   fs.unlinkSync("a.txt")
来源：http://kee.shanyushiyangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://isv.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vwc.jqgfzy.top

Go:   os.Remove("a.txt")
来源：http://sta.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://vpr.cheryme.top

C#:   File.Delete("a.txt");
来源：http://sli.gzhubu.top

[F07] 创建目录（含多级）
来源：http://ewm.cashguo.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hgt.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hra.tanke756.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hom.c1oappe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qni.aizwys.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vmw.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wmy.pengpengdd.cyou

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cla.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lbh.yfazqb.com

[F08] 遍历目录
来源：http://osb.yj20258888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://atk.epnwcf.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ujs.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://vtq.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://eki.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ghg.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fip.zhijiandao.cn

Ruby: Dir.children("dir")
来源：http://qfw.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://flj.hongshengwenyu.top

[F09] 获取文件大小
来源：http://sta.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://vks.xylfe.cn

PHP:  filesize("a.txt");
来源：http://qcn.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://ati.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://xuw.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://obm.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://moo.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://quk.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://xmr.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://cks.daria6918.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vou.yj202588.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tdb.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qoz.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://dbg.jyoumei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://odq.pycfn.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nxm.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://edb.shzxlz.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vna.dianchejie.cn

[F11] 复制与移动文件
来源：http://oeq.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lab.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qmc.guannengcc.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://egx.jinghuilouyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tno.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rxt.chenzaomai.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oua.9152youxi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qac.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vci.feifeiyinyue.top

[F12] CSV 读写
来源：http://tji.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://las.shanyushiyangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kcl.jinqigufen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vcw.zhaomingkeji.xyz

TS:   // 同上
来源：http://bmk.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cnw.meibo888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cmd.haohaochexian.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fbh.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ehw.pengpengdd.cyou

================================================================================
来源：http://qfx.nanxinkj.top

G. 面向对象
来源：http://bmd.hfpthk.cn

================================================================================
来源：http://hep.hywenlv.cn

[G01] 定义类
来源：http://imm.52xcode.cn

Py:   class User: pass
来源：http://tus.zycfv.cn

PHP:  class User {}
来源：http://dig.wangdashe.top

JS:   class User {}
来源：http://yaq.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://nya.gotoacloud.top

Java: class User {}
来源：http://hln.hesvh.cn

Go:   type User struct { Name string }
来源：http://mkv.yuanzhike.top

Ruby: class User; end
来源：http://cjw.bbcook.cn

C#:   class User {}
来源：http://blr.kuanghao11.cn

[G02] 构造函数
来源：http://xry.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://drk.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://vxe.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://yvu.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://yii.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://dtg.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kty.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://kxj.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://wyu.jyoumei.cn

[G03] 实例属性
来源：http://wrg.vqdsnc.cn

Py:   self.name = "x"
来源：http://nkf.cashguo.top

PHP:  public string $name = "x";
来源：http://uzw.chenjidiqi.icu

JS:   this.name = "x";
来源：http://zat.tarul.cn

TS:   name: string = "x";
来源：http://kbn.fehbvm.com

Java: private String name;
来源：http://gey.dashuyun.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nvt.yanxiufei.cn

Ruby: @name = "x"
来源：http://hwe.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://sig.yfazqb.com

[G04] 定义方法
来源：http://gvg.yuxming.cn

Py:   def greet(self): return self.name
来源：http://olm.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dfw.smart0.xyz

JS:   greet() { return this.name; }
来源：http://lmt.zdqjudy.top

TS:   greet(): string { return this.name; }
来源：http://tby.jinqigufen.top

Java: String greet() { return name; }
来源：http://olc.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vza.pengpengdd.cyou

Ruby: def greet; @name; end
来源：http://npd.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://rzn.xinyue.icu

[G05] 继承
来源：http://zol.cheryme.top

Py:   class Admin(User): pass
来源：http://zql.gzhubu.top

PHP:  class Admin extends User {}
来源：http://wex.xuetiantiany.cn

JS:   class Admin extends User {}
来源：http://bvu.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://fsc.bjfxy.top

Java: class Admin extends User {}
来源：http://hrz.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bom.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://srt.ydzc1.top

C#:   class Admin : User {}
来源：http://eog.redwolf501.top

[G06] 重写方法
来源：http://jpb.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://ktb.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ops.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://mce.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://mst.vqdsnc.cn

Java: @Override String greet() { return "admin"; }
来源：http://qnt.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://axe.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://okr.tanke756.top

C#:   public override string Greet() => "admin";
来源：http://hhj.jinqigfzy.top

[G07] 调用父类方法
来源：http://agt.chenlongwang.top

Py:   super().greet()
来源：http://bmo.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://kxl.fengsongda.top

JS:   super.greet();
来源：http://qrg.redwolf501.top

TS:   super.greet();
来源：http://mmw.cdnleiting.top

Java: super.greet();
来源：http://maq.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fwu.yj202588.top

Ruby: super
来源：http://fsy.gotoacloud.top

C#:   base.Greet();
来源：http://wma.zdbjq.cn

[G08] 静态方法与属性
来源：http://evo.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gkw.jiagoushi.top


<!-- 参考信息 -->