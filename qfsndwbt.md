代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://pha.xziqi.cn

Ruby: arr.include?(x)
来源：http://dix.hnqzz.top

C#:   list.Contains(x)
来源：http://ddh.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://cpg.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rjb.zdqjudy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kry.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kjn.cdnleiting.top

TS:   [...arr];
来源：http://vdd.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://hvo.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://fsc.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://tch.yj20258888.top

C#:   new List<int>(list);
来源：http://zpc.zhoulong.xyz

[D23] reduce 累积计算
来源：http://eut.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://enu.yonumen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bkw.sufxvd.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ddp.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tjn.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qwr.dashuyun.cn

Go:   // 手写循环
来源：http://hxc.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gfk.jqgfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ccl.jinyuanbaomall.cn

[D24] 字典 / Map 基本操作
来源：http://nqa.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://awu.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://upt.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mcv.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zki.zycfv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gak.birdmap.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cey.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tot.shuidangran.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qnc.hnxiangtu.top

[D25] Set 集合去重与交并差
来源：http://djs.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fnh.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dkx.tanke756.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cpf.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cfb.jinqigufen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gjq.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iti.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sck.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dct.wangshuangyany.cn

[D26] 数组转字符串
来源：http://luf.kuanghao11.cn

Py:   ", ".join(map(str, arr))
来源：http://fqa.bjfxy.top

PHP:  implode(", ", $arr);
来源：http://bdl.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://lrw.nwbrower.top

TS:   arr.join(", ")
来源：http://aln.cheryme.top

Java: String.join(", ", list)
来源：http://ajc.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://byr.yuxming.cn

Ruby: arr.join(", ")
来源：http://dpa.zhiwuduotai.top

C#:   string.Join(", ", list)
来源：http://aaf.yonumen.top

================================================================================
来源：http://zcq.yanxiufei.cn

E. 字符串处理
来源：http://kcy.guannengcc.top

================================================================================
来源：http://yiq.zhoulong.xyz

[E01] 拼接字符串
来源：http://nej.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dpz.daria6918.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nmo.jqgfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cip.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bzs.hnxiangtu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://peh.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dxd.zhengqikj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pfp.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://szt.fengsongda.top

[E02] 重复字符串
来源：http://laf.chenzaomai.com

Py:   "ab" * 3
来源：http://oil.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://jly.yj20258.top

JS:   "ab".repeat(3)
来源：http://psx.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://rkx.xziqi.cn

Java: "ab".repeat(3)
来源：http://ddp.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://zti.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://zfy.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mdw.sufxvd.cn

[E03] 截取子串
来源：http://vvb.shzxlz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fox.yj20258.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wvo.jinqigufen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dsd.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://zfd.sxryk.cn

Java: s.substring(1, 4)
来源：http://hyj.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ptr.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iiv.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://egm.ydzc1.top

[E04] 查找子串位置
来源：http://ugt.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://btm.zhiwuduotai.top

PHP:  strpos($s, "x");
来源：http://hgw.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pki.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://hxb.gaohongyu789.top

Java: s.indexOf("x")
来源：http://ojg.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://ugb.smart0.xyz

Ruby: s.index("x")
来源：http://ykf.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://ups.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dvk.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tla.wangdashe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tdp.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://brj.svipenyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ird.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cqx.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://faq.jlsjyb.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nsx.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uam.cashguo.top

[E06] 替换子串
来源：http://qhe.daria6918.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dae.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://rzy.kuanghao11.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://shx.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://idh.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bzi.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hyw.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qhu.zhaomingkeji.xyz

C#:   s.Replace("a", "b")
来源：http://gfc.dianchejie.cn

[E07] 按分隔符拆分
来源：http://qkh.chenzaomai.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cvo.jyoumei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mnu.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://koj.pycfn.com

TS:   s.split(",")
来源：http://yaj.0kj1m.cn

Java: s.split(",");  s.split("\\s+")
来源：http://buc.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wkv.havefunace.top

Ruby: s.split(",");  s.split
来源：http://vry.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zrh.pengpengdd.cyou

[E08] 数组按分隔符合并
来源：http://dzs.yangfankeji.com

Py:   ",".join(items)
来源：http://nwn.yonumen.top

PHP:  implode(",", $items);
来源：http://mrv.jyoumei.cn

JS:   items.join(",")
来源：http://qgk.gotoacloud.top

TS:   items.join(",")
来源：http://mah.hnqzz.top

Java: String.join(",", items)
来源：http://anx.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://vhi.hnxiangtu.top

Ruby: items.join(",")
来源：http://kpb.tanke756.top

C#:   string.Join(",", items)
来源：http://fhr.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://mno.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eot.xylfe.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uxm.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://mri.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://yss.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://cwr.aizwys.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ufo.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xoj.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vps.nanxuanxn.top

[E10] 左侧补零 / 定长填充
来源：http://cnj.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hcv.kuanghao11.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pvd.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://ioo.yuxming.cn

TS:   "7".padStart(3, "0")
来源：http://urv.andypj.xyz

Java: String.format("%03d", 7)
来源：http://zdq.cdnleiting.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ynr.fehbvm.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jcp.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uhs.sysykeji.top

[E11] 反转字符串
来源：http://ejd.jqgufenzy.top

Py:   s[::-1]
来源：http://vtk.fehbvm.com

PHP:  strrev($s);
来源：http://ohw.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://shb.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://rbg.pengpengdd.cyou

Java: new StringBuilder(s).reverse().toString()
来源：http://diw.tanke756.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ykm.yvedp.cn

Ruby: s.reverse
来源：http://yeq.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://pms.guannengcc.top

[E12] 统计某字符出现次数
来源：http://nwd.quarkkingdee.top

Py:   s.count("a")
来源：http://aom.cashguo.top

PHP:  substr_count($s, "a");
来源：http://hsm.yj20258888.top

JS:   s.split("a").length - 1
来源：http://aon.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://owj.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kdl.yongpay.top

Go:   strings.Count(s, "a")
来源：http://wgx.hongshengwenyu.top

Ruby: s.count("a")
来源：http://lwz.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://jhd.zdqjudy.top

[E13] 逐字符遍历
来源：http://dyo.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://xnj.yuxming.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cuo.ydjk.org.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ftd.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ool.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yao.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://din.havefunace.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sjm.shuidangran.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ewu.fengsongda.top

[E14] URL 编码与 Base64
来源：http://wlp.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cpc.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kgi.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hkd.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mmv.feifeiyinyue.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jow.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bkm.ppjwa.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ils.shzxlz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dqr.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://pog.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vgl.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://imd.9152youxi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rey.yueranfly.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qkq.gotoacloud.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gpi.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jhp.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wii.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lpy.hesvh.cn

[E16] 数字千分位
来源：http://wwr.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://fwo.tianlin.xyz

PHP:  number_format(1234567);
来源：http://maw.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://aso.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xmm.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lsn.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jrv.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wnf.shzxlz.cn

C#:   1234567.ToString("N0")
来源：http://dti.ydzc1.top

[E17] 首字母大写
来源：http://bwq.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mga.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cjr.guowangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iyo.shzxlz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rqg.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://erb.ybcxt.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gya.fzhhl.top

Ruby: s.capitalize
来源：http://pie.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://var.fzhhl.top

[E18] 模板占位符替换
来源：http://ngs.ybcxt.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cgm.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kxo.ybcxt.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wbv.svipenyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iei.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fdn.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mal.nanxuanxn.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hro.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pzd.gzhubu.top

[E19] 多行文本按行拆分
来源：http://wwb.sjlbkw.cn

Py:   s.splitlines()
来源：http://fmp.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fyu.jinqigufen.top

JS:   s.split(/\r?\n/)
来源：http://nhx.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://stl.fktsv.cn

Java: s.lines().toList()
来源：http://uxy.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://oyb.yj202588.top

Ruby: s.lines
来源：http://ggb.tarul.cn

C#:   s.Split('\n')
来源：http://moe.fzhhl.top

[E20] 判断字符串是否为空
来源：http://qlm.yfazqb.com

Py:   if not s:
来源：http://kvq.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pky.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kjc.redwolf501.top

TS:   if (s === "") {}
来源：http://hth.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://boy.feifeiyinyue.top

Go:   if s == "" {}
来源：http://fck.xuetiantiany.cn

Ruby: if s.empty?
来源：http://soq.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zba.tanke756.top

[E21] 超长截断加省略号
来源：http://ahz.hywenlv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://coy.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ddv.gotoacloud.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hjo.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://str.jlsjyb.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yle.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://bzr.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fxi.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vag.pycfn.com

[E22] 字节长度与字符长度
来源：http://pgr.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bja.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://puw.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://obo.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nwe.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tsi.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mdv.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://zhg.nanxinkj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wqz.ctjpmb.com

================================================================================
来源：http://aub.cucudq.cn

F. 文件与目录
来源：http://dfl.gzhubu.top

================================================================================
来源：http://vvw.zdqjudy.top

[F01] 读取整个文件
来源：http://sjy.jinyuanbaomall.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ddu.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://ris.wangshuangyany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pwn.fengsongda.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pvv.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lho.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vmh.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://inu.epnwcf.com

C#:   File.ReadAllText("a.txt");
来源：http://tak.bjfxy.top

[F02] 逐行读取文件
来源：http://tti.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fqv.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uir.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eun.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tti.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uwl.meibo888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://svn.cucudq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wsa.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uut.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://bnn.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rgo.gaohongyu789.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://aei.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://urx.jlsjyb.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mdc.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eps.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jsh.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://gdq.cheryme.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cfo.yuxming.cn

[F04] 追加写入文件
来源：http://fur.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://krz.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ncc.sxryk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wdo.nanxuanxn.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gob.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://frc.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bst.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gjc.yuxming.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xkj.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://sxa.iojbl.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jpe.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://qqx.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://yqg.andypj.xyz

TS:   fs.existsSync("a.txt")
来源：http://gwb.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kse.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jpc.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://dms.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://req.snrcjt.cn

[F06] 删除文件
来源：http://cxc.nwbrower.top

Py:   os.remove("a.txt")
来源：http://vpu.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://xbd.wangdashe.top


<!-- 参考信息 -->