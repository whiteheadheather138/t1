代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ord.jiagoushi.top

[D24] 字典 / Map 基本操作
来源：http://vgc.gotoacloud.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uek.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ftg.sweek.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xeg.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://igb.vqdsnc.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://stv.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pch.zdbjq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://agi.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ose.cheryme.top

[D25] Set 集合去重与交并差
来源：http://cve.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fon.cucudq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aoh.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wdb.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pcq.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xyl.fanxiaobao.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fqy.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oae.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qwx.ppjwa.cn

[D26] 数组转字符串
来源：http://xuv.pengpengdd.cyou

Py:   ", ".join(map(str, arr))
来源：http://nxm.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://ouf.ppjwa.cn

JS:   arr.join(", ")
来源：http://uuf.vqdsnc.cn

TS:   arr.join(", ")
来源：http://dbo.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://yph.yj20258888.top

Go:   strings.Join(strs, ", ")
来源：http://ybm.cqqwz.cn

Ruby: arr.join(", ")
来源：http://sao.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://oay.ywan-chungtsiang.top

================================================================================
来源：http://nco.jinghuilouyu.cn

E. 字符串处理
来源：http://jzt.cucudq.cn

================================================================================
来源：http://wwz.ctjpmb.com

[E01] 拼接字符串
来源：http://kmh.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jje.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rij.xziqi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tln.hywenlv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ugg.tanke756.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ztc.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jop.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rve.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://clk.sxryk.cn

[E02] 重复字符串
来源：http://rym.xingfuxueyuan.xyz

Py:   "ab" * 3
来源：http://xfg.9152youxi.cn

PHP:  str_repeat("ab", 3);
来源：http://kix.tian-w.cn

JS:   "ab".repeat(3)
来源：http://kej.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://xns.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://phj.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://qzm.jinqigufen.top

Ruby: "ab" * 3
来源：http://nzw.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ebz.fzhhl.top

[E03] 截取子串
来源：http://izs.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rds.bjfxy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://crx.316326.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jeu.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://sog.gogol.net.cn

Java: s.substring(1, 4)
来源：http://mve.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://big.xinyue.icu

Ruby: s[1, 3];  s[1..3]
来源：http://cvg.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://vsc.dashuyun.cn

[E04] 查找子串位置
来源：http://iiw.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://gja.wangshuangyany.cn

PHP:  strpos($s, "x");
来源：http://oll.yongpay.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ckn.ppjwa.cn

TS:   s.indexOf("x")
来源：http://xjv.jinqigufen.top

Java: s.indexOf("x")
来源：http://ogy.smart0.xyz

Go:   strings.Index(s, "x")
来源：http://hoj.yonumen.top

Ruby: s.index("x")
来源：http://zjr.hnqzz.top

C#:   s.IndexOf("x")
来源：http://wyz.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mty.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zbl.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dxc.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jja.c1oappe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nye.hammf.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nbv.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lan.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gdk.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mgd.sysykeji.top

[E06] 替换子串
来源：http://osz.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zjx.yuanzhike.top

PHP:  str_replace("a", "b", $s);
来源：http://uss.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zuv.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://uwz.sxryk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ryy.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ysz.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gtl.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://cqa.cqqwz.cn

[E07] 按分隔符拆分
来源：http://mzd.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://chq.chenjidiqi.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://der.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://khq.cdnleiting.top

TS:   s.split(",")
来源：http://nfy.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://hqn.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kla.hnxiangtu.top

Ruby: s.split(",");  s.split
来源：http://uno.hongshengwenyu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pfu.meibo888.top

[E08] 数组按分隔符合并
来源：http://cdu.xylfe.cn

Py:   ",".join(items)
来源：http://ibe.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://mvt.jinqigufen.top

JS:   items.join(",")
来源：http://nuv.jqgufenzy.top

TS:   items.join(",")
来源：http://ahw.shuidangran.top

Java: String.join(",", items)
来源：http://npo.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://wre.tian-w.cn

Ruby: items.join(",")
来源：http://nfl.smart0.xyz

C#:   string.Join(",", items)
来源：http://hhs.jqgfzy.top

[E09] 去除所有空白字符
来源：http://sds.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ygg.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hdn.hcnkem.com

JS:   s.replace(/\s+/g, "")
来源：http://jvf.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://xbe.hcnkem.com

Java: s.replaceAll("\\s+", "")
来源：http://apc.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://nge.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pdh.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pwh.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://ule.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://otp.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qvn.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://phc.zhixingplan.top

TS:   "7".padStart(3, "0")
来源：http://elr.chenlongwang.top

Java: String.format("%03d", 7)
来源：http://upr.ivvv.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ita.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vqe.yuanzhike.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wzc.tarul.cn

[E11] 反转字符串
来源：http://psv.zhaomingkeji.xyz

Py:   s[::-1]
来源：http://sxg.zycfv.cn

PHP:  strrev($s);
来源：http://eaa.sweek.top

JS:   [...s].reverse().join("")
来源：http://vag.snrcjt.cn

TS:   [...s].reverse().join("")
来源：http://btn.fzhhl.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tmn.yanxiufei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lxl.zhoulong.xyz

Ruby: s.reverse
来源：http://oew.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ydf.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://rwq.yj202588.top

Py:   s.count("a")
来源：http://olk.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://xnq.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://xot.chenjidiqi.icu

TS:   s.split("a").length - 1
来源：http://hbw.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cib.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://owu.dashuyun.cn

Ruby: s.count("a")
来源：http://ohi.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://dsq.zhengqikj.top

[E13] 逐字符遍历
来源：http://ojc.gzhubu.top

Py:   for ch in s: print(ch)
来源：http://nta.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://npj.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://cyl.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cgk.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://szn.fehbvm.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lgg.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ukm.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zcq.sysykeji.top

[E14] URL 编码与 Base64
来源：http://gkw.redwolf501.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nqo.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://doy.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vaz.hfpthk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ygj.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://adq.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uac.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ztf.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wui.jinyuanbaomall.cn

[E15] HTML 转义 / 反转义
来源：http://lmg.sysykeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jtz.zhaomingkeji.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://njc.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hzf.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ltp.ydzc1.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bdg.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://npg.vehdjk.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xsi.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://msd.chenjidiqi.icu

[E16] 数字千分位
来源：http://sql.fehbvm.com

Py:   f"{1234567:,}"
来源：http://bed.xziqi.cn

PHP:  number_format(1234567);
来源：http://ida.9152youxi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ngb.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yah.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://odm.hammf.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uva.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qnl.guannengcc.top

C#:   1234567.ToString("N0")
来源：http://agc.andypj.xyz

[E17] 首字母大写
来源：http://kes.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cpb.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://xlr.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ozi.fanxiaobao.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bla.xylfe.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://stz.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wfz.xylfe.cn

Ruby: s.capitalize
来源：http://ksl.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nik.jinqigufen.top

[E18] 模板占位符替换
来源：http://tgs.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://seh.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lsz.tian-w.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zrm.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://lje.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://okv.gogol.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rez.yfazqb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oua.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://evh.fehbvm.com

[E19] 多行文本按行拆分
来源：http://fns.zdbjq.cn

Py:   s.splitlines()
来源：http://izl.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dku.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://rek.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://eha.hcnkem.com

Java: s.lines().toList()
来源：http://krz.yfazqb.com

Go:   strings.Split(s, "\n")
来源：http://elm.pycfn.com

Ruby: s.lines
来源：http://jix.smart0.xyz

C#:   s.Split('\n')
来源：http://ahl.aizwys.cn

[E20] 判断字符串是否为空
来源：http://tab.fktsv.cn

Py:   if not s:
来源：http://exf.quarkkingdee.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wvs.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xtd.chenzaomai.com

TS:   if (s === "") {}
来源：http://ykw.chenzaomai.com

Java: if (s.isEmpty()) {}
来源：http://azu.jianghu66.top

Go:   if s == "" {}
来源：http://eay.shzxlz.cn

Ruby: if s.empty?
来源：http://kic.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yss.redwolf501.top

[E21] 超长截断加省略号
来源：http://wot.ivvv.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lnw.jinqigfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://afx.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mdi.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dnl.zycfv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gif.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://xpr.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xdk.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pnx.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://ubw.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lha.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://grr.xziqi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hdf.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://joa.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ebe.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yib.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://aaj.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bos.snrcjt.cn

================================================================================
来源：http://oik.yuxming.cn

F. 文件与目录
来源：http://kau.cdnleiting.top

================================================================================
来源：http://zyq.yuanzhike.top

[F01] 读取整个文件
来源：http://rpj.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://frr.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://pth.fanxiaobao.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wus.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://irv.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dbk.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xqk.tian-w.cn

Ruby: File.read("a.txt")
来源：http://zlf.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://mij.xylfe.cn

[F02] 逐行读取文件
来源：http://vff.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xig.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://luw.gaohongyu789.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ggr.sysykeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://djh.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://obm.svipenyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oci.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ntw.dianchejie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://stt.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://twu.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zgt.gaohongyu789.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xtd.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gnn.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wys.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aan.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ktt.birdmap.top

Ruby: File.write("a.txt", "hi")
来源：http://tcx.yvedp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xwz.andypj.xyz

[F04] 追加写入文件
来源：http://qwj.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://puq.zhengqikj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cuq.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mnq.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zyl.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wuc.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yci.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://foh.jinqigfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://goh.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://nfy.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qqk.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://bwl.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://ugf.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://kea.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uim.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aqo.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://buh.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://snl.zhengqikj.top

[F06] 删除文件
来源：http://zne.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://kly.vqdsnc.cn

PHP:  unlink("a.txt");
来源：http://sky.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://dhr.bbcook.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xmy.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yfw.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://blq.tarul.cn

Ruby: File.delete("a.txt")
来源：http://bvg.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://hmv.fengsongda.top

[F07] 创建目录（含多级）
来源：http://whc.nanxinkj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dzi.yongpay.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wrd.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://keb.shanyushiyangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://puz.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hmn.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://okr.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://smt.pycfn.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lag.yuanzhike.top

[F08] 遍历目录
来源：http://rng.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cbe.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hdt.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://pse.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://ged.zhiwuduotai.top


<!-- 参考信息 -->