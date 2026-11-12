代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hgn.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://zwn.aizwys.cn

Go:   // 手写循环
来源：http://wbj.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pqy.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bah.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://rkv.nanxinkj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wxd.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://duo.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vyv.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ppb.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pkc.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ojk.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lhh.c1oappe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rav.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://onf.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sxm.jyoumei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hkd.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hup.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nxs.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ted.ybcxt.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dug.yangfankeji.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dlf.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://glc.jiagoushi.top

[D26] 数组转字符串
来源：http://ykp.feifeiyinyue.top

Py:   ", ".join(map(str, arr))
来源：http://ygc.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://rse.zhoulong.xyz

JS:   arr.join(", ")
来源：http://pjc.redwolf501.top

TS:   arr.join(", ")
来源：http://lvw.havefunace.top

Java: String.join(", ", list)
来源：http://tnc.xziqi.cn

Go:   strings.Join(strs, ", ")
来源：http://hfl.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://smi.hesvh.cn

C#:   string.Join(", ", list)
来源：http://xki.hongshengwenyu.top

================================================================================
来源：http://gxr.xylfe.cn

E. 字符串处理
来源：http://qxj.birdmap.top

================================================================================
来源：http://yah.jlsjyb.cn

[E01] 拼接字符串
来源：http://jxx.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wqq.ybcxt.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kyn.yuanzhike.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://crk.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vdu.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nzk.pengpengdd.cyou

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://plz.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jhn.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iup.zhongyouzk.top

[E02] 重复字符串
来源：http://mxk.sysykeji.top

Py:   "ab" * 3
来源：http://efv.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://wds.haohaochexian.top

JS:   "ab".repeat(3)
来源：http://vpj.bjfxy.top

TS:   "ab".repeat(3)
来源：http://tba.xylfe.cn

Java: "ab".repeat(3)
来源：http://nha.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://xkw.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://vej.sweek.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jtl.chenjidiqi.icu

[E03] 截取子串
来源：http://yfj.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rju.bjfxy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ahl.daxiang520.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aya.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://cdd.cashguo.top

Java: s.substring(1, 4)
来源：http://nxk.yongpay.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hya.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://uhu.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://jbm.fktsv.cn

[E04] 查找子串位置
来源：http://ane.bbcook.cn

Py:   s.find("x");  s.index("x")
来源：http://hnr.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://cno.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uwu.yj20258.top

TS:   s.indexOf("x")
来源：http://akw.tian-w.cn

Java: s.indexOf("x")
来源：http://jdi.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://mge.9152youxi.cn

Ruby: s.index("x")
来源：http://ogj.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://skz.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ole.bjfxy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ohy.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hek.yonumen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dta.gogol.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rtd.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oie.daria6918.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qyi.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wol.yj20258888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ixu.yj202588.top

[E06] 替换子串
来源：http://jjw.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dkw.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://axc.vqdsnc.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://age.feifeiyinyue.top

TS:   s.replaceAll("a", "b")
来源：http://jyy.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pza.fktsv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hcs.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kip.tanke756.top

C#:   s.Replace("a", "b")
来源：http://vzl.gogol.net.cn

[E07] 按分隔符拆分
来源：http://ghg.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eus.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hzb.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://edh.fktsv.cn

TS:   s.split(",")
来源：http://azr.yuxming.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eif.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uqd.sxryk.cn

Ruby: s.split(",");  s.split
来源：http://mpz.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gge.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://snu.zhoulong.xyz

Py:   ",".join(items)
来源：http://ztj.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://nke.hfpthk.cn

JS:   items.join(",")
来源：http://dgv.tianlin.xyz

TS:   items.join(",")
来源：http://cux.jlsjyb.cn

Java: String.join(",", items)
来源：http://phb.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://dcb.yanxiufei.cn

Ruby: items.join(",")
来源：http://rnd.zhixingplan.top

C#:   string.Join(",", items)
来源：http://krl.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://hkh.guowangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fti.mhx1999.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aji.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://ftw.hnxiangtu.top

TS:   s.replace(/\s+/g, "")
来源：http://upc.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://luj.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fps.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://rcy.wangshuangyany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ots.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://tun.yj20258888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qbv.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://shc.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://pnf.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://qzm.yfazqb.com

Java: String.format("%03d", 7)
来源：http://zqd.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fec.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vja.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vpo.9152youxi.cn

[E11] 反转字符串
来源：http://pks.yj202588.top

Py:   s[::-1]
来源：http://fke.hfpthk.cn

PHP:  strrev($s);
来源：http://sni.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://oro.jinqigufen.top

TS:   [...s].reverse().join("")
来源：http://crc.zhijiandao.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qaa.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://gwq.yuanzhike.top

Ruby: s.reverse
来源：http://kqb.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://qxl.fengsongda.top

[E12] 统计某字符出现次数
来源：http://oxk.tian-w.cn

Py:   s.count("a")
来源：http://sfw.yongpay.top

PHP:  substr_count($s, "a");
来源：http://nyb.mhx1999.top

JS:   s.split("a").length - 1
来源：http://rrz.haohaochexian.top

TS:   s.split("a").length - 1
来源：http://uxe.hammf.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xxm.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://hux.yj20258.top

Ruby: s.count("a")
来源：http://wvz.yueranfly.top

C#:   s.Count(c => c == 'a')
来源：http://lhv.hesvh.cn

[E13] 逐字符遍历
来源：http://oee.havefunace.top

Py:   for ch in s: print(ch)
来源：http://dxe.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sue.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eaa.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lrr.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jzs.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dhc.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xsr.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zzp.ydzc1.top

[E14] URL 编码与 Base64
来源：http://dbp.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mov.zdqjudy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fuv.sxryk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://adp.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ufn.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xrr.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qjj.zhixingplan.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://omg.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://obz.yfazqb.com

[E15] HTML 转义 / 反转义
来源：http://yet.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yvh.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rlg.xylfe.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mdb.bjfxy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://iqs.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jkj.zhiwuduotai.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://btw.zdbjq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rql.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://beh.smart0.xyz

[E16] 数字千分位
来源：http://rnw.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://xbz.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://ymy.andypj.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://rha.cashguo.top

TS:   (1234567).toLocaleString("en-US")
来源：http://aye.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://icq.yuxming.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ccb.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pgl.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://rqp.epnwcf.com

[E17] 首字母大写
来源：http://ver.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qqb.hesvh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sfh.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xug.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://akq.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gga.daria6918.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zqx.yj20258.top

Ruby: s.capitalize
来源：http://dvy.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wia.shuidangran.top

[E18] 模板占位符替换
来源：http://vij.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fpd.zycfv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ukn.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xgo.chenlongwang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ipf.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aim.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://esk.cucudq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://glp.nwbrower.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eyq.c1oappe.top

[E19] 多行文本按行拆分
来源：http://afz.daria6918.cn

Py:   s.splitlines()
来源：http://avb.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zyl.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://pey.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://oua.dianchejie.cn

Java: s.lines().toList()
来源：http://mmf.cdnleiting.top

Go:   strings.Split(s, "\n")
来源：http://qes.yuanzhike.top

Ruby: s.lines
来源：http://ovk.uphjek.com

C#:   s.Split('\n')
来源：http://lbb.shuidangran.top

[E20] 判断字符串是否为空
来源：http://qml.shanyushiyangtech.top

Py:   if not s:
来源：http://uar.shangyingyoupin.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fon.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fos.dianchejie.cn

TS:   if (s === "") {}
来源：http://qzv.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://dve.tianlin.xyz

Go:   if s == "" {}
来源：http://jdm.feifeiyinyue.top

Ruby: if s.empty?
来源：http://xcl.bbcook.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://phb.9152youxi.cn

[E21] 超长截断加省略号
来源：http://qax.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cbq.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yoq.iojbl.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hwa.mhx1999.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uxe.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tba.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://nim.yonumen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://err.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kbe.yonumen.top

[E22] 字节长度与字符长度
来源：http://sqm.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yoe.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iay.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sqr.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gcr.aizwys.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lha.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rjm.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://elk.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qem.guannengcc.top

================================================================================
来源：http://wvv.hfpthk.cn

F. 文件与目录
来源：http://zvh.guannengcc.top

================================================================================
来源：http://zpm.nanxuanxn.top

[F01] 读取整个文件
来源：http://huh.zhixingplan.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xop.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://mms.sysykeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dpn.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ptz.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://zmc.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rio.aibaodan.cn

Ruby: File.read("a.txt")
来源：http://koo.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://iqd.meibo888.top

[F02] 逐行读取文件
来源：http://dar.hesvh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kcx.jqgfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wav.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wsc.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://get.andypj.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ljs.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://njf.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ojc.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hhs.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://cut.hongshengwenyu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wkp.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mxj.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://myu.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ehw.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gnw.vqdsnc.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://znl.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://fgt.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://myt.tian-w.cn

[F04] 追加写入文件
来源：http://gky.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ufn.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yoa.shangyingyoupin.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yar.nanxuanxn.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://shh.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dzr.smart0.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rhx.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zdy.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dgv.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://jdh.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://squ.zhiwuduotai.top

PHP:  file_exists("a.txt");
来源：http://swi.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://bya.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://wyj.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zkc.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rgb.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://kih.hammf.cn

C#:   File.Exists("a.txt")
来源：http://kch.cashguo.top

[F06] 删除文件
来源：http://hgb.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://gwi.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://kba.yonumen.top

JS:   fs.unlinkSync("a.txt")
来源：http://xyu.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wxt.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ryp.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://ztg.ctjpmb.com

Ruby: File.delete("a.txt")
来源：http://mkq.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://vzw.ydzc1.top

[F07] 创建目录（含多级）
来源：http://vbk.feifeiyinyue.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lhn.sufxvd.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mny.guowangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dzd.epnwcf.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rtb.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pfi.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dup.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://agr.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nde.hnxiangtu.top

[F08] 遍历目录
来源：http://jep.gotoacloud.top


<!-- 参考信息 -->