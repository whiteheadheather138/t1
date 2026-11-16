代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://vos.tianlin.xyz

Ruby: arr.include?(x)
来源：http://vld.cheryme.top

C#:   list.Contains(x)
来源：http://jgv.cqqwz.cn

[D22] 复制数组（避免共享引用）
来源：http://luq.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kin.zhongyouzk.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ray.cqqwz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wtn.zhengqikj.top

TS:   [...arr];
来源：http://blw.hesvh.cn

Java: new ArrayList<>(list);
来源：http://wbn.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://awv.meibo888.top

Ruby: arr.dup;  arr.clone
来源：http://dgv.snrcjt.cn

C#:   new List<int>(list);
来源：http://yku.vqdsnc.cn

[D23] reduce 累积计算
来源：http://muh.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hbm.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tji.yonumen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qlb.sweek.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tem.haohaochexian.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jmy.shzxlz.cn

Go:   // 手写循环
来源：http://hfh.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ldd.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qqz.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://xnr.xylfe.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rwx.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jni.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sxg.feifeiyinyue.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hhr.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yyv.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://brk.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uyt.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ixo.quarkkingdee.top

[D25] Set 集合去重与交并差
来源：http://dep.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://icl.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ugv.yongpay.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kpy.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jux.shangyingyoupin.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fyc.dianchejie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://apw.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pmr.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://npe.aibaodan.cn

[D26] 数组转字符串
来源：http://peh.zycfv.cn

Py:   ", ".join(map(str, arr))
来源：http://fud.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://ryj.fktsv.cn

JS:   arr.join(", ")
来源：http://dhg.jiagoushi.top

TS:   arr.join(", ")
来源：http://eiz.tanke756.top

Java: String.join(", ", list)
来源：http://nhb.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://tyr.52xcode.cn

Ruby: arr.join(", ")
来源：http://ehb.svipenyu.cn

C#:   string.Join(", ", list)
来源：http://pzb.shanyushiyangtech.top

================================================================================
来源：http://eni.yuanzhike.top

E. 字符串处理
来源：http://tdd.xylfe.cn

================================================================================
来源：http://ezt.jyoumei.cn

[E01] 拼接字符串
来源：http://thw.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://plt.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ccp.shanyushiyangtech.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rzc.dianchejie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kjn.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ari.sjlbkw.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://twd.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kpa.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yir.kuanghao11.cn

[E02] 重复字符串
来源：http://tyk.wangshuangyany.cn

Py:   "ab" * 3
来源：http://qmw.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://fxj.pycfn.com

JS:   "ab".repeat(3)
来源：http://jti.ydzc1.top

TS:   "ab".repeat(3)
来源：http://ccr.xziqi.cn

Java: "ab".repeat(3)
来源：http://ktn.tian-w.cn

Go:   strings.Repeat("ab", 3)
来源：http://obv.tanke756.top

Ruby: "ab" * 3
来源：http://iaj.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fsr.shanyushiyangkeji.top

[E03] 截取子串
来源：http://xbn.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yos.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qjt.jiagoushi.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ymz.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://daw.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://aiw.snrcjt.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fqc.jinghuilouyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dgi.nanxuanxn.top

C#:   s.Substring(1, 3)
来源：http://cbs.chenjidiqi.icu

[E04] 查找子串位置
来源：http://uev.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://awk.tarul.cn

PHP:  strpos($s, "x");
来源：http://ckf.pycfn.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gwy.bbcook.cn

TS:   s.indexOf("x")
来源：http://hjg.zycfv.cn

Java: s.indexOf("x")
来源：http://tnm.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://zok.zhoulong.xyz

Ruby: s.index("x")
来源：http://asw.bbcook.cn

C#:   s.IndexOf("x")
来源：http://won.xuetiantiany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yfb.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hjh.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qsh.cashguo.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mca.zhixingplan.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rrl.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nfs.yj202588.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://guy.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wsp.yuanzhike.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jfq.sufxvd.cn

[E06] 替换子串
来源：http://bxe.yj20258.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jgz.guowangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://mrg.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://imh.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://nvk.fzhhl.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bvf.pengpengdd.cyou

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://own.xylfe.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://avl.iojbl.cn

C#:   s.Replace("a", "b")
来源：http://yaa.fehbvm.com

[E07] 按分隔符拆分
来源：http://gti.hfpthk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://anb.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nmo.jlsjyb.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zbl.yuxming.cn

TS:   s.split(",")
来源：http://rwv.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://ivb.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ryn.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://seo.cqqwz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rgz.cqqwz.cn

[E08] 数组按分隔符合并
来源：http://opm.redwolf501.top

Py:   ",".join(items)
来源：http://zyo.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://ckj.ydzc1.top

JS:   items.join(",")
来源：http://vsr.fehbvm.com

TS:   items.join(",")
来源：http://vri.daria6918.cn

Java: String.join(",", items)
来源：http://stw.fktsv.cn

Go:   strings.Join(items, ",")
来源：http://cqt.dashuyun.cn

Ruby: items.join(",")
来源：http://xwo.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://soi.uphjek.com

[E09] 去除所有空白字符
来源：http://mdh.gaohongyu789.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gyv.quarkkingdee.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lzd.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://nuv.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://ycl.hywenlv.cn

Java: s.replaceAll("\\s+", "")
来源：http://czl.nanxinkj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jzz.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://znw.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://plb.smart0.xyz

[E10] 左侧补零 / 定长填充
来源：http://kaj.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://spr.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ypj.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://gra.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://gwk.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://cjm.wangshuangyany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mja.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mpg.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cwx.shanyushiyangtech.top

[E11] 反转字符串
来源：http://ray.jinghuilouyu.cn

Py:   s[::-1]
来源：http://rtu.ivvv.top

PHP:  strrev($s);
来源：http://ycb.yj202588.top

JS:   [...s].reverse().join("")
来源：http://chi.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://ute.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://yly.ydjk.org.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kkq.epnwcf.com

Ruby: s.reverse
来源：http://soy.hnxiangtu.top

C#:   new string(s.Reverse().ToArray())
来源：http://zxv.epnwcf.com

[E12] 统计某字符出现次数
来源：http://xry.hongshengwenyu.top

Py:   s.count("a")
来源：http://lwm.pycfn.com

PHP:  substr_count($s, "a");
来源：http://zof.xylfe.cn

JS:   s.split("a").length - 1
来源：http://iow.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://fdz.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bxu.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://nbo.dashuyun.cn

Ruby: s.count("a")
来源：http://kfw.ivvv.top

C#:   s.Count(c => c == 'a')
来源：http://ljm.c1oappe.top

[E13] 逐字符遍历
来源：http://zio.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://yyn.0kj1m.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://onp.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vzv.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://uyc.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://det.hesvh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vqq.jqgufenzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://evu.sjlbkw.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://avp.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://tug.sxryk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yqs.sysykeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gar.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cpc.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xdb.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yhl.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://roc.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rvy.yj20258.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rwj.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://ruj.yuxming.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sgx.gogol.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ijv.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qkr.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://utl.kuanghao11.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://plx.meibo888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dky.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cch.jinyuanbaomall.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wmq.hongshengwenyu.top

[E16] 数字千分位
来源：http://hht.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://abo.pycfn.com

PHP:  number_format(1234567);
来源：http://eei.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zak.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://omk.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://txa.hcnkem.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hgp.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zsz.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://sme.yongpay.top

[E17] 首字母大写
来源：http://lkb.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cyq.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dvt.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kid.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://usr.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wxe.quarkkingdee.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cnq.iojbl.cn

Ruby: s.capitalize
来源：http://dvv.uphjek.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tbl.svipenyu.cn

[E18] 模板占位符替换
来源：http://kts.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nrp.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nqe.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sbg.yvedp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://alh.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://awl.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mpe.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qer.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kid.hesvh.cn

[E19] 多行文本按行拆分
来源：http://pja.zhaomingkeji.xyz

Py:   s.splitlines()
来源：http://evz.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vke.fktsv.cn

JS:   s.split(/\r?\n/)
来源：http://uqg.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://msz.jlsjyb.cn

Java: s.lines().toList()
来源：http://djk.hnqzz.top

Go:   strings.Split(s, "\n")
来源：http://pah.gzhubu.top

Ruby: s.lines
来源：http://veo.yongpay.top

C#:   s.Split('\n')
来源：http://bwj.feifeiyinyue.top

[E20] 判断字符串是否为空
来源：http://qcl.hammf.cn

Py:   if not s:
来源：http://rnu.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kez.yanxiufei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://doe.fktsv.cn

TS:   if (s === "") {}
来源：http://gbt.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://ulz.tarul.cn

Go:   if s == "" {}
来源：http://dml.svipenyu.cn

Ruby: if s.empty?
来源：http://ecz.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cri.jinqigfzy.top

[E21] 超长截断加省略号
来源：http://mkh.snrcjt.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qul.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jip.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://esv.smart0.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sjr.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zrr.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://nac.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bqt.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fko.meibo888.top

[E22] 字节长度与字符长度
来源：http://cnn.zdqjudy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hgz.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lac.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kyf.andypj.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://swh.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://awj.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lat.jinyuanbaomall.cn

Ruby: s.bytesize;  s.length
来源：http://qxe.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gyp.ctjpmb.com

================================================================================
来源：http://sgr.wangdashe.top

F. 文件与目录
来源：http://szc.ctjpmb.com

================================================================================
来源：http://yxv.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://mmj.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rtn.zhongyouzk.top

PHP:  file_get_contents("a.txt");
来源：http://ami.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nkb.jqgufenzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ksk.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ehf.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qna.xziqi.cn

Ruby: File.read("a.txt")
来源：http://agi.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://mtk.hnxiangtu.top

[F02] 逐行读取文件
来源：http://vtr.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qye.cdnleiting.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jmf.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xon.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hqk.hongshengwenyu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://glw.snrcjt.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://flv.ydzc1.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wum.zhaomingkeji.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uzk.pycfn.com

[F03] 写入文件（覆盖）
来源：http://ugl.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qql.cdnleiting.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wij.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jsm.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jti.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gyy.fengsongda.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zik.yonumen.top

Ruby: File.write("a.txt", "hi")
来源：http://kvn.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zdh.smart0.xyz

[F04] 追加写入文件
来源：http://jzq.yonumen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lxb.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qcd.sufxvd.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://knw.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bvm.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jkq.yuxming.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kub.sufxvd.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vwp.ydjk.org.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wti.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://jnx.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zsh.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://zwi.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://yxc.xingfuxueyuan.xyz

TS:   fs.existsSync("a.txt")
来源：http://wsa.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://evp.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zqr.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://ioj.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://xad.jinghuilouyu.cn

[F06] 删除文件
来源：http://vel.feifeiyinyue.top

Py:   os.remove("a.txt")
来源：http://dif.gaohongyu789.top

PHP:  unlink("a.txt");
来源：http://wbw.pengpengdd.cyou


<!-- 参考信息 -->