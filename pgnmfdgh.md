代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://syj.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://nbe.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vmq.feifeiyinyue.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nbv.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://otu.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bes.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cda.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bnx.uphjek.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dki.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ikl.iojbl.cn

[D25] Set 集合去重与交并差
来源：http://bbb.zhengqikj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jxa.xuanzx.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vxp.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qhv.sweek.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ilh.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qeh.andypj.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nbr.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hvm.shanyushiyangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kgh.dianchejie.cn

[D26] 数组转字符串
来源：http://jvv.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://cap.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://mrg.cqqwz.cn

JS:   arr.join(", ")
来源：http://grd.chenzaomai.com

TS:   arr.join(", ")
来源：http://syw.tian-w.cn

Java: String.join(", ", list)
来源：http://ixq.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://ypj.mhx1999.top

Ruby: arr.join(", ")
来源：http://klb.daxiang520.top

C#:   string.Join(", ", list)
来源：http://gfj.jqgfzy.top

================================================================================
来源：http://aak.jinqigufen.top

E. 字符串处理
来源：http://dbn.gogol.net.cn

================================================================================
来源：http://gnb.xinyue.icu

[E01] 拼接字符串
来源：http://sbw.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lhp.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ijx.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qiz.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tit.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uwe.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qqu.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lmq.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bfb.guowangkeji.top

[E02] 重复字符串
来源：http://juh.ivvv.top

Py:   "ab" * 3
来源：http://mfv.zhongyouzk.top

PHP:  str_repeat("ab", 3);
来源：http://uit.hesvh.cn

JS:   "ab".repeat(3)
来源：http://itq.ydzc1.top

TS:   "ab".repeat(3)
来源：http://voz.hammf.cn

Java: "ab".repeat(3)
来源：http://zpz.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://owy.quarkkingdee.top

Ruby: "ab" * 3
来源：http://vnq.yangfankeji.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eok.yj202588.top

[E03] 截取子串
来源：http://zju.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hms.ehwqpu.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://weg.jinqigufen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hrn.havefunace.top

TS:   s.slice(1, 4)
来源：http://wam.iojbl.cn

Java: s.substring(1, 4)
来源：http://qdi.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://znl.zhiwuduotai.top

Ruby: s[1, 3];  s[1..3]
来源：http://njf.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://otf.jlsjyb.cn

[E04] 查找子串位置
来源：http://ikq.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://gvc.andypj.xyz

PHP:  strpos($s, "x");
来源：http://fqf.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oqd.jiagoushi.top

TS:   s.indexOf("x")
来源：http://qur.vehdjk.com

Java: s.indexOf("x")
来源：http://iqy.yuxming.cn

Go:   strings.Index(s, "x")
来源：http://wmr.uphjek.com

Ruby: s.index("x")
来源：http://gni.ppjwa.cn

C#:   s.IndexOf("x")
来源：http://kwv.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rhk.hysaishi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kdc.cheryme.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mln.tanke756.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://len.shanyushiyangtech.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pfq.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jlp.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bxi.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bdp.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ohq.316326.xyz

[E06] 替换子串
来源：http://rul.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nzg.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://yus.jyoumei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ntr.yueranfly.top

TS:   s.replaceAll("a", "b")
来源：http://ahl.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ycb.hnxiangtu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tuz.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iro.nanxinkj.top

C#:   s.Replace("a", "b")
来源：http://app.gzhubu.top

[E07] 按分隔符拆分
来源：http://glw.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zte.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vhv.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dmf.haohaochexian.top

TS:   s.split(",")
来源：http://caz.uphjek.com

Java: s.split(",");  s.split("\\s+")
来源：http://bfu.jinqigfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://msp.chenlongwang.top

Ruby: s.split(",");  s.split
来源：http://hvl.yj202588.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fii.ybcxt.top

[E08] 数组按分隔符合并
来源：http://fmf.yj20258888.top

Py:   ",".join(items)
来源：http://pyi.xziqi.cn

PHP:  implode(",", $items);
来源：http://kfi.vqdsnc.cn

JS:   items.join(",")
来源：http://gxt.shuidangran.top

TS:   items.join(",")
来源：http://zqf.sufxvd.cn

Java: String.join(",", items)
来源：http://rbo.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://kwy.nanxuanxn.top

Ruby: items.join(",")
来源：http://pni.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://coh.iojbl.cn

[E09] 去除所有空白字符
来源：http://xiq.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mwu.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nag.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://tph.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://idh.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://wsi.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://yla.ybcxt.top

Ruby: s.gsub(/\s+/, "")
来源：http://est.gotoacloud.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rcf.zdqjudy.top

[E10] 左侧补零 / 定长填充
来源：http://tfx.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mgz.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kpt.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://wbn.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://ryg.hnxiangtu.top

Java: String.format("%03d", 7)
来源：http://leb.gotoacloud.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hdc.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://akp.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kdp.snrcjt.cn

[E11] 反转字符串
来源：http://otm.cashguo.top

Py:   s[::-1]
来源：http://hbx.zhengqikj.top

PHP:  strrev($s);
来源：http://lem.yvedp.cn

JS:   [...s].reverse().join("")
来源：http://siy.yj20258888.top

TS:   [...s].reverse().join("")
来源：http://tup.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qzs.hysaishi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ait.shuidangran.top

Ruby: s.reverse
来源：http://ffi.yj202588.top

C#:   new string(s.Reverse().ToArray())
来源：http://qpr.fengsongda.top

[E12] 统计某字符出现次数
来源：http://rif.zycfv.cn

Py:   s.count("a")
来源：http://uos.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://kka.fktsv.cn

JS:   s.split("a").length - 1
来源：http://uus.xziqi.cn

TS:   s.split("a").length - 1
来源：http://msr.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qtk.jyoumei.cn

Go:   strings.Count(s, "a")
来源：http://kic.andypj.xyz

Ruby: s.count("a")
来源：http://zvw.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://rjm.ydjk.org.cn

[E13] 逐字符遍历
来源：http://rhy.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://uld.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://isi.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://odc.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lya.ydzc1.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qmz.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ulh.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://izc.316326.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://idv.daxiang520.top

[E14] URL 编码与 Base64
来源：http://odr.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tma.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hpy.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hce.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qmn.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zmk.zdbjq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mix.guannengcc.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pbg.nwbrower.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wco.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://xfn.shanyushiyangtech.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mio.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yfk.smart0.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eri.jianghu66.top

TS:   // 同上，务必做 XSS 过滤
来源：http://klk.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://chl.guowangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wyq.aibaodan.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kna.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uyx.vqdsnc.cn

[E16] 数字千分位
来源：http://vkm.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://wtg.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://vri.snrcjt.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zss.kuanghao11.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://aly.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yzj.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eht.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ndb.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://htb.cqqwz.cn

[E17] 首字母大写
来源：http://cin.fengsongda.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pkz.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://wjl.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lnn.zhaomingkeji.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://epl.ehwqpu.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jor.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://frp.yj20258.top

Ruby: s.capitalize
来源：http://mhf.sufxvd.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://let.jyoumei.cn

[E18] 模板占位符替换
来源：http://hju.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pau.wangshuangyany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qlo.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://asn.yj20258888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jov.chenzaomai.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://egq.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ikr.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xnq.jinqigufen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pkg.meibo888.top

[E19] 多行文本按行拆分
来源：http://qjy.birdmap.top

Py:   s.splitlines()
来源：http://zjc.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fpd.shangyingyoupin.top

JS:   s.split(/\r?\n/)
来源：http://esp.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://kfu.jqgfzy.top

Java: s.lines().toList()
来源：http://wvw.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://rhs.hfpthk.cn

Ruby: s.lines
来源：http://qbp.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://nye.vehdjk.com

[E20] 判断字符串是否为空
来源：http://bdj.daxiang520.top

Py:   if not s:
来源：http://irr.nanxinkj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://brm.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qbp.quarkkingdee.top

TS:   if (s === "") {}
来源：http://nzn.xziqi.cn

Java: if (s.isEmpty()) {}
来源：http://isf.ppjwa.cn

Go:   if s == "" {}
来源：http://rsd.hysaishi.cn

Ruby: if s.empty?
来源：http://gkw.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://csu.jianghu66.top

[E21] 超长截断加省略号
来源：http://fjg.iojbl.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eat.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kvj.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iqw.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iso.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wbd.pengpengdd.cyou

Go:   // 按 rune 判断长度后截断
来源：http://fuu.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iac.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ium.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://eaa.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zdp.c1oappe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bod.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uvm.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fpz.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lwm.zdbjq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rdp.yj202588.top

Ruby: s.bytesize;  s.length
来源：http://lsk.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zhk.hcnkem.com

================================================================================
来源：http://awc.yueranfly.top

F. 文件与目录
来源：http://zdm.yfazqb.com

================================================================================
来源：http://fka.fktsv.cn

[F01] 读取整个文件
来源：http://xox.xylfe.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wvc.jinqigufen.top

PHP:  file_get_contents("a.txt");
来源：http://tbw.ywan-chungtsiang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gei.andypj.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mnx.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mmz.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://liw.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://sms.quarkkingdee.top

C#:   File.ReadAllText("a.txt");
来源：http://kct.daxiang520.top

[F02] 逐行读取文件
来源：http://sjt.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jyv.ehwqpu.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://woc.aizwys.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fyz.havefunace.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yco.aibaodan.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tyv.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xwu.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mju.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qdw.fehbvm.com

[F03] 写入文件（覆盖）
来源：http://ced.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kzi.smart0.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://gjy.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blr.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qqv.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lrh.zycfv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jbl.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://nkk.zhiwuduotai.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://myx.jiagoushi.top

[F04] 追加写入文件
来源：http://xko.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mnw.ehwqpu.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://juk.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ykv.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ctz.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rpl.ydjk.org.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yej.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fnr.chenzaomai.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ffy.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://bvi.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uxx.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://otr.sjlbkw.cn

JS:   fs.existsSync("a.txt")
来源：http://jmd.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://ivw.jlsjyb.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bsz.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ioi.meibo888.top

Ruby: File.exist?("a.txt")
来源：http://bpq.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://upv.nanxuanxn.top

[F06] 删除文件
来源：http://kns.andypj.xyz

Py:   os.remove("a.txt")
来源：http://khh.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://osw.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://iri.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mmb.ppjwa.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://odf.pengpengdd.cyou

Go:   os.Remove("a.txt")
来源：http://oxl.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://lvo.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://lgn.yvedp.cn

[F07] 创建目录（含多级）
来源：http://zyv.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://izj.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cbg.tanke756.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cst.dashuyun.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mww.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xmr.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qoo.gotoacloud.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zqo.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://odz.sxryk.cn

[F08] 遍历目录
来源：http://fiz.hcnkem.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://uiv.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mbq.gotoacloud.top

JS:   fs.readdirSync("dir")
来源：http://ulr.yfazqb.com

TS:   fs.readdirSync("dir")
来源：http://rbn.daria6918.cn


<!-- 参考信息 -->