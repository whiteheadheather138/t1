代发 wailian999

Java: new ArrayList<>(list);
来源：http://unt.yonumen.top

Go:   copied := append([]int(nil), arr...)
来源：http://rjd.hywenlv.cn

Ruby: arr.dup;  arr.clone
来源：http://mpj.hammf.cn

C#:   new List<int>(list);
来源：http://fuz.shanyushiyangtech.top

[D23] reduce 累积计算
来源：http://hwl.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nmg.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://knq.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fth.jinghuilouyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://riv.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ffs.yj202588.top

Go:   // 手写循环
来源：http://ycb.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vtf.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qhz.redwolf501.top

[D24] 字典 / Map 基本操作
来源：http://gma.yuxming.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://goi.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jac.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aly.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dzz.c1oappe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xdd.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mos.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qds.yueranfly.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://agv.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://vmu.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qio.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cco.cashguo.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kai.xuetiantiany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bib.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://csb.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://svu.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pqv.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fdv.aizwys.cn

[D26] 数组转字符串
来源：http://hoh.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://inz.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://pnx.c1oappe.top

JS:   arr.join(", ")
来源：http://cgz.sysykeji.top

TS:   arr.join(", ")
来源：http://xwc.sufxvd.cn

Java: String.join(", ", list)
来源：http://eyj.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://amu.fanxiaobao.xyz

Ruby: arr.join(", ")
来源：http://kky.yuxming.cn

C#:   string.Join(", ", list)
来源：http://erh.fanxiaobao.xyz

================================================================================
来源：http://ssz.kuanghao11.cn

E. 字符串处理
来源：http://ata.ywan-chungtsiang.top

================================================================================
来源：http://set.nanxuanxn.top

[E01] 拼接字符串
来源：http://xoe.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rwz.zhiwuduotai.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aif.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ahk.cqqwz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aut.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://klk.yfazqb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aqz.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://czm.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gvj.yongpay.top

[E02] 重复字符串
来源：http://dxd.yueranfly.top

Py:   "ab" * 3
来源：http://nhe.vqdsnc.cn

PHP:  str_repeat("ab", 3);
来源：http://vdq.pycfn.com

JS:   "ab".repeat(3)
来源：http://jap.bjfxy.top

TS:   "ab".repeat(3)
来源：http://dqi.sufxvd.cn

Java: "ab".repeat(3)
来源：http://okt.jlsjyb.cn

Go:   strings.Repeat("ab", 3)
来源：http://uhq.ehwqpu.com

Ruby: "ab" * 3
来源：http://kmd.yonumen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cvq.yj20258.top

[E03] 截取子串
来源：http://swd.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ohd.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://frv.yj20258888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pkh.tarul.cn

TS:   s.slice(1, 4)
来源：http://rpa.xuanzx.com

Java: s.substring(1, 4)
来源：http://dop.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ljs.shanyushiyangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://oqe.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://gky.cheryme.top

[E04] 查找子串位置
来源：http://yak.jinqigufen.top

Py:   s.find("x");  s.index("x")
来源：http://hej.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://umn.cheryme.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pvt.xinyue.icu

TS:   s.indexOf("x")
来源：http://riu.hywenlv.cn

Java: s.indexOf("x")
来源：http://pqx.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://sfj.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://rjv.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://dwi.ywan-chungtsiang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ghl.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wgk.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qui.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://npo.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rzj.hammf.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xvv.tian-w.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wvk.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qrs.hywenlv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jmq.zhoulong.xyz

[E06] 替换子串
来源：http://pcl.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ehb.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://esb.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qfp.shanyushiyangtech.top

TS:   s.replaceAll("a", "b")
来源：http://biz.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xob.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pee.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vyz.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://ewm.hesvh.cn

[E07] 按分隔符拆分
来源：http://dxo.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hrj.sxryk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fst.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qww.cqqwz.cn

TS:   s.split(",")
来源：http://ool.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://gkb.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wag.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://kjg.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wtj.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://vup.jqgfzy.top

Py:   ",".join(items)
来源：http://ktz.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://htg.guannengcc.top

JS:   items.join(",")
来源：http://tqs.hysaishi.cn

TS:   items.join(",")
来源：http://qiq.nwbrower.top

Java: String.join(",", items)
来源：http://dqh.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://whl.xuanzx.com

Ruby: items.join(",")
来源：http://ley.tanke756.top

C#:   string.Join(",", items)
来源：http://vvt.shzxlz.cn

[E09] 去除所有空白字符
来源：http://csr.bjfxy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://acs.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rpu.jqgfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://cto.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://pzq.9152youxi.cn

Java: s.replaceAll("\\s+", "")
来源：http://nvd.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://eok.ppjwa.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lqh.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rst.guowangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://gpi.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wxm.0kj1m.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jht.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://reu.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://oix.chenjidiqi.icu

Java: String.format("%03d", 7)
来源：http://idg.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://ymi.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://okn.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jme.shzxlz.cn

[E11] 反转字符串
来源：http://ztt.daxiang520.top

Py:   s[::-1]
来源：http://oux.nanxinkj.top

PHP:  strrev($s);
来源：http://eet.tarul.cn

JS:   [...s].reverse().join("")
来源：http://gip.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://bzb.yfazqb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://rzf.haohaochexian.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xhp.fktsv.cn

Ruby: s.reverse
来源：http://khg.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://qni.wangdashe.top

[E12] 统计某字符出现次数
来源：http://nbz.jqgfzy.top

Py:   s.count("a")
来源：http://uzz.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://tty.hammf.cn

JS:   s.split("a").length - 1
来源：http://rpx.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://erc.zdbjq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://moo.hesvh.cn

Go:   strings.Count(s, "a")
来源：http://xxw.tianlin.xyz

Ruby: s.count("a")
来源：http://ins.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://mdg.svipenyu.cn

[E13] 逐字符遍历
来源：http://gtq.vqdsnc.cn

Py:   for ch in s: print(ch)
来源：http://iqg.zhixingplan.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://feo.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tzv.daxiang520.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://det.jinqigufen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fzu.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nkn.xuanzx.com

Ruby: s.each_char { |ch| puts ch }
来源：http://bwt.snrcjt.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ifv.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://lbd.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ckp.jianghu66.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hrg.shanyushiyangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://esq.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bet.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vcn.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://egg.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sle.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bbj.cdnleiting.top

[E15] HTML 转义 / 反转义
来源：http://xwc.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tij.ivvv.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vpg.aibaodan.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iun.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ldr.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sef.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lil.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pnj.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oti.jiagoushi.top

[E16] 数字千分位
来源：http://lnb.tian-w.cn

Py:   f"{1234567:,}"
来源：http://ohl.fengsongda.top

PHP:  number_format(1234567);
来源：http://mwz.hysaishi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qnu.hesvh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zth.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mni.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://naw.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kai.hammf.cn

C#:   1234567.ToString("N0")
来源：http://knr.snrcjt.cn

[E17] 首字母大写
来源：http://ron.yfazqb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xdn.ybcxt.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bim.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cow.ydjk.org.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ljh.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://icz.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://juc.jlsjyb.cn

Ruby: s.capitalize
来源：http://ubc.jinqigufen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iuc.yuanzhike.top

[E18] 模板占位符替换
来源：http://epp.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kgg.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://unr.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yjm.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://yxb.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ino.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sjm.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xny.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nxi.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://rog.jlsjyb.cn

Py:   s.splitlines()
来源：http://cgr.nanxuanxn.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zdf.tianlin.xyz

JS:   s.split(/\r?\n/)
来源：http://lgh.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://ugg.guowangkeji.top

Java: s.lines().toList()
来源：http://grb.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://bqk.hcnkem.com

Ruby: s.lines
来源：http://foc.ivvv.top

C#:   s.Split('\n')
来源：http://vru.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://idc.hywenlv.cn

Py:   if not s:
来源：http://ned.mhx1999.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xvj.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tfh.smart0.xyz

TS:   if (s === "") {}
来源：http://hyb.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://yle.aibaodan.cn

Go:   if s == "" {}
来源：http://bnv.zhongyouzk.top

Ruby: if s.empty?
来源：http://rqr.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rau.aizwys.cn

[E21] 超长截断加省略号
来源：http://cte.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eof.xingfuxueyuan.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rhi.sweek.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tzm.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fad.sxryk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ohd.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://tnb.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wqy.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://okm.wangdashe.top

[E22] 字节长度与字符长度
来源：http://lhw.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dbe.jqgufenzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yky.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sjq.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pxs.tian-w.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yvj.zhaomingkeji.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ofz.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://fwu.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yja.shzxlz.cn

================================================================================
来源：http://yjg.zycfv.cn

F. 文件与目录
来源：http://lcr.shangyingyoupin.top

================================================================================
来源：http://trz.0kj1m.cn

[F01] 读取整个文件
来源：http://imc.yongpay.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xpf.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://plz.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://neh.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nfj.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tjo.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cpr.xziqi.cn

Ruby: File.read("a.txt")
来源：http://jrf.sweek.top

C#:   File.ReadAllText("a.txt");
来源：http://zcw.cdnleiting.top

[F02] 逐行读取文件
来源：http://rjj.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gwj.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://akx.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wjy.yj20258888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dcb.nanxinkj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lkt.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bbr.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mda.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mta.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://hgx.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yyu.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nph.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gyo.quarkkingdee.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vih.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ijq.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gee.shzxlz.cn

Ruby: File.write("a.txt", "hi")
来源：http://tms.yuxming.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pef.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://eym.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jnm.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ezb.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ndj.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sux.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iog.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hxy.jinqigfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ojg.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://avg.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://jpo.zhijiandao.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aad.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://kzs.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://dgc.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://hty.ehwqpu.com

Java: Files.exists(Path.of("a.txt"))
来源：http://xyf.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qlp.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://ogm.zdqjudy.top

C#:   File.Exists("a.txt")
来源：http://bye.svipenyu.cn

[F06] 删除文件
来源：http://muz.ivvv.top

Py:   os.remove("a.txt")
来源：http://jkf.xziqi.cn

PHP:  unlink("a.txt");
来源：http://edb.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://vdy.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://shk.guowangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wnr.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://txx.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://mfy.fengsongda.top

C#:   File.Delete("a.txt");
来源：http://nml.bjfxy.top

[F07] 创建目录（含多级）
来源：http://zmi.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gln.tianlin.xyz


<!-- 参考信息 -->