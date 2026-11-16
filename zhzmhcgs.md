代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qdw.uphjek.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://hqh.yj20258.top

Go:   // 手写循环
来源：http://vvn.epnwcf.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ygc.sjlbkw.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://agc.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://nfm.jyoumei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tnd.zycfv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://foj.yvedp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tnu.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lcr.gaohongyu789.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ugr.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jtr.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yso.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wjx.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://yaf.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lbc.jinqigfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://azl.aibaodan.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nrj.shanyushiyangtech.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://akz.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ass.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xzv.mhx1999.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mch.cheryme.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jxf.zhongyouzk.top

[D26] 数组转字符串
来源：http://lde.jinghuilouyu.cn

Py:   ", ".join(map(str, arr))
来源：http://rol.pengpengdd.cyou

PHP:  implode(", ", $arr);
来源：http://rbu.shanyushiyangtech.top

JS:   arr.join(", ")
来源：http://juc.zhoulong.xyz

TS:   arr.join(", ")
来源：http://ceo.yj202588.top

Java: String.join(", ", list)
来源：http://qka.zhoulong.xyz

Go:   strings.Join(strs, ", ")
来源：http://cyl.fehbvm.com

Ruby: arr.join(", ")
来源：http://jgk.fehbvm.com

C#:   string.Join(", ", list)
来源：http://xmm.jinqigufen.top

================================================================================
来源：http://vfs.snrcjt.cn

E. 字符串处理
来源：http://hkv.yfazqb.com

================================================================================
来源：http://rnr.guannengcc.top

[E01] 拼接字符串
来源：http://ogq.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gaq.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ngh.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vvj.havefunace.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mgv.tarul.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yba.c1oappe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xxz.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qqh.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wfm.fzhhl.top

[E02] 重复字符串
来源：http://mqn.nanxinkj.top

Py:   "ab" * 3
来源：http://zrw.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://nla.wangdashe.top

JS:   "ab".repeat(3)
来源：http://rfa.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://zga.fktsv.cn

Java: "ab".repeat(3)
来源：http://dwf.zhoulong.xyz

Go:   strings.Repeat("ab", 3)
来源：http://acm.jianghu66.top

Ruby: "ab" * 3
来源：http://uhm.0kj1m.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qvh.yanxiufei.cn

[E03] 截取子串
来源：http://emh.zycfv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tfr.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gis.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hwo.snrcjt.cn

TS:   s.slice(1, 4)
来源：http://ojk.shuidangran.top

Java: s.substring(1, 4)
来源：http://vwu.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iso.yonumen.top

Ruby: s[1, 3];  s[1..3]
来源：http://tud.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://cif.jyoumei.cn

[E04] 查找子串位置
来源：http://ynk.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://kxe.xingfuxueyuan.xyz

PHP:  strpos($s, "x");
来源：http://neu.gotoacloud.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://shu.yangfankeji.com

TS:   s.indexOf("x")
来源：http://bks.xziqi.cn

Java: s.indexOf("x")
来源：http://sge.316326.xyz

Go:   strings.Index(s, "x")
来源：http://wwl.aibaodan.cn

Ruby: s.index("x")
来源：http://zoy.havefunace.top

C#:   s.IndexOf("x")
来源：http://eax.zhaomingkeji.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://kzx.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wmv.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qar.andypj.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yqz.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rye.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fuf.hesvh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://upc.svipenyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kqt.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cdz.jinyuanbaomall.cn

[E06] 替换子串
来源：http://sgp.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rqt.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://nfh.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qhr.mhx1999.top

TS:   s.replaceAll("a", "b")
来源：http://wno.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zwf.cashguo.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ijp.xuanzx.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eei.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://lob.andypj.xyz

[E07] 按分隔符拆分
来源：http://gnk.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hkt.shangyingyoupin.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lvy.nanxuanxn.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vth.andypj.xyz

TS:   s.split(",")
来源：http://cvp.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://aim.xziqi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://svr.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://ram.chenjidiqi.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qgf.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://pbf.jiagoushi.top

Py:   ",".join(items)
来源：http://ktm.jianghu66.top

PHP:  implode(",", $items);
来源：http://nuy.jianghu66.top

JS:   items.join(",")
来源：http://lzg.redwolf501.top

TS:   items.join(",")
来源：http://klb.yongpay.top

Java: String.join(",", items)
来源：http://ftg.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://hnk.aibaodan.cn

Ruby: items.join(",")
来源：http://zku.hesvh.cn

C#:   string.Join(",", items)
来源：http://xrz.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://kbi.guannengcc.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wbb.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wnq.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://ake.zhaomingkeji.xyz

TS:   s.replace(/\s+/g, "")
来源：http://gch.gzhubu.top

Java: s.replaceAll("\\s+", "")
来源：http://qlh.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dti.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://gyn.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://voh.fanxiaobao.xyz

[E10] 左侧补零 / 定长填充
来源：http://bih.xziqi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kab.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pxf.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://jmp.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://xhp.bjfxy.top

Java: String.format("%03d", 7)
来源：http://wiq.pycfn.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://cjy.ywan-chungtsiang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eey.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kqx.fanxiaobao.xyz

[E11] 反转字符串
来源：http://rwj.wangdashe.top

Py:   s[::-1]
来源：http://zcv.zycfv.cn

PHP:  strrev($s);
来源：http://bmm.ybcxt.top

JS:   [...s].reverse().join("")
来源：http://bes.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://hfn.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uty.yj20258888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://prj.0kj1m.cn

Ruby: s.reverse
来源：http://kyx.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xri.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://xtf.zhixingplan.top

Py:   s.count("a")
来源：http://zvk.yj202588.top

PHP:  substr_count($s, "a");
来源：http://utu.yj20258.top

JS:   s.split("a").length - 1
来源：http://upe.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://tzx.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nep.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://nws.chenjidiqi.icu

Ruby: s.count("a")
来源：http://rag.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://zth.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://jyf.yj20258.top

Py:   for ch in s: print(ch)
来源：http://ovh.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aeo.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://akm.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ils.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ndf.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vyh.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sju.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iqf.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://ngc.hysaishi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://flw.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://egx.ydzc1.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://swc.daria6918.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ivi.yuxming.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vci.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fek.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fpg.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tai.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://klg.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://och.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wag.316326.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://etc.shangyingyoupin.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vmq.zdqjudy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hwm.jianghu66.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jny.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bcg.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bsj.zhengqikj.top

[E16] 数字千分位
来源：http://zoi.xylfe.cn

Py:   f"{1234567:,}"
来源：http://rwm.jqgfzy.top

PHP:  number_format(1234567);
来源：http://xlu.sysykeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xgz.zhaomingkeji.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://lzb.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hpi.fanxiaobao.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hbp.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gwj.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://eqp.snrcjt.cn

[E17] 首字母大写
来源：http://ffn.quarkkingdee.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://exz.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kou.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bsk.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hcu.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jbg.jianghu66.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ylq.fzhhl.top

Ruby: s.capitalize
来源：http://wkl.jinyuanbaomall.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nga.zdbjq.cn

[E18] 模板占位符替换
来源：http://hfb.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sww.fehbvm.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pvh.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zfs.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fci.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wlq.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bgh.pengpengdd.cyou

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ndu.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ozi.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://ilf.52xcode.cn

Py:   s.splitlines()
来源：http://xts.iojbl.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zva.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://rir.feifeiyinyue.top

TS:   s.split(/\r?\n/)
来源：http://qpe.hnxiangtu.top

Java: s.lines().toList()
来源：http://gbd.snrcjt.cn

Go:   strings.Split(s, "\n")
来源：http://lxm.guannengcc.top

Ruby: s.lines
来源：http://atu.jinqigufen.top

C#:   s.Split('\n')
来源：http://trz.redwolf501.top

[E20] 判断字符串是否为空
来源：http://oyh.sjlbkw.cn

Py:   if not s:
来源：http://hhi.shanyushiyangtech.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xzb.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vwr.sweek.top

TS:   if (s === "") {}
来源：http://tni.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://yzv.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://bpx.jlsjyb.cn

Ruby: if s.empty?
来源：http://nyx.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wwt.yfazqb.com

[E21] 超长截断加省略号
来源：http://chx.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yqn.dashuyun.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zcc.xuanzx.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cgy.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hah.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qqv.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://wem.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hyf.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fwf.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://xfu.uphjek.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jdu.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ruu.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://stj.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vpy.jinqigfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jgy.hammf.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dlz.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://ugr.pengpengdd.cyou

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fnd.cqqwz.cn

================================================================================
来源：http://gfl.daria6918.cn

F. 文件与目录
来源：http://bjo.birdmap.top

================================================================================
来源：http://pon.nanxinkj.top

[F01] 读取整个文件
来源：http://eeb.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oxn.zhongyouzk.top

PHP:  file_get_contents("a.txt");
来源：http://kle.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ael.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ztk.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://grd.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://arb.52xcode.cn

Ruby: File.read("a.txt")
来源：http://dfz.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://htu.havefunace.top

[F02] 逐行读取文件
来源：http://uzv.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nhm.tianlin.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qjj.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://plw.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mqz.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://amh.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sio.gaohongyu789.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bwx.cucudq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ifb.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://vqy.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ptw.ydzc1.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mhs.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://flp.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ojl.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wzx.hongshengwenyu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zzv.xuanzx.com

Ruby: File.write("a.txt", "hi")
来源：http://psp.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hsq.ppjwa.cn

[F04] 追加写入文件
来源：http://mhh.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yfy.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hax.cashguo.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ach.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wbe.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qot.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ipz.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lip.shangyingyoupin.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://thp.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://pas.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ccl.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://aef.xziqi.cn

JS:   fs.existsSync("a.txt")
来源：http://vvo.yueranfly.top

TS:   fs.existsSync("a.txt")
来源：http://hau.hnqzz.top

Java: Files.exists(Path.of("a.txt"))
来源：http://swt.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://grx.fktsv.cn

Ruby: File.exist?("a.txt")
来源：http://umh.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://qkz.zhoulong.xyz

[F06] 删除文件
来源：http://unc.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://lrl.cheryme.top

PHP:  unlink("a.txt");
来源：http://qqs.52xcode.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zgs.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://mmo.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jmk.wangdashe.top

Go:   os.Remove("a.txt")
来源：http://nsx.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://sbw.redwolf501.top

C#:   File.Delete("a.txt");
来源：http://fcc.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://xui.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cgc.hcnkem.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gny.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mtr.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lzu.andypj.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gne.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qsd.xuanzx.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tha.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gdu.sjlbkw.cn

[F08] 遍历目录
来源：http://fju.yonumen.top


<!-- 参考信息 -->