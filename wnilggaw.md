代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://fzk.zhixingplan.top

JS:   arr.includes(x)
来源：http://wwn.jinqigufen.top

TS:   arr.includes(x)
来源：http://sbw.xuetiantiany.cn

Java: list.contains(x)
来源：http://pbx.cdnleiting.top

Go:   slices.Contains(arr, x)
来源：http://mts.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://zma.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://krc.cashguo.top

[D22] 复制数组（避免共享引用）
来源：http://qbt.zhengqikj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hme.hysaishi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kkn.sxryk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mnb.wangshuangyany.cn

TS:   [...arr];
来源：http://gfl.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://pbd.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://yvm.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://hcw.iojbl.cn

C#:   new List<int>(list);
来源：http://kkl.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://azo.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oed.fanxiaobao.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fqk.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ncj.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://quy.fehbvm.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://jls.yj20258888.top

Go:   // 手写循环
来源：http://zox.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nfo.tarul.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jau.316326.xyz

[D24] 字典 / Map 基本操作
来源：http://klh.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bzd.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ska.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yfy.c1oappe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://usd.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ejy.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://siw.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://csx.dashuyun.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iuq.sysykeji.top

[D25] Set 集合去重与交并差
来源：http://ikm.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cgq.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fva.yanxiufei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://emp.jinyuanbaomall.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://txq.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ndd.tianlin.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://whk.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gvt.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hoo.yanxiufei.cn

[D26] 数组转字符串
来源：http://imq.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://kdg.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://ikq.yj20258.top

JS:   arr.join(", ")
来源：http://uyg.iojbl.cn

TS:   arr.join(", ")
来源：http://quq.xuanzx.com

Java: String.join(", ", list)
来源：http://veq.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://xtc.kuanghao11.cn

Ruby: arr.join(", ")
来源：http://fvr.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://fea.ctjpmb.com

================================================================================
来源：http://byv.shzxlz.cn

E. 字符串处理
来源：http://qxz.dashuyun.cn

================================================================================
来源：http://olt.yuxming.cn

[E01] 拼接字符串
来源：http://srq.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zdl.sjlbkw.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bvz.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://teo.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sor.zhengqikj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qzs.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uam.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aag.shangyingyoupin.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://esw.cheryme.top

[E02] 重复字符串
来源：http://xak.shanyushiyangkeji.top

Py:   "ab" * 3
来源：http://ewt.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://yey.haohaochexian.top

JS:   "ab".repeat(3)
来源：http://lgl.ywan-chungtsiang.top

TS:   "ab".repeat(3)
来源：http://nzb.chenzaomai.com

Java: "ab".repeat(3)
来源：http://dvx.zhixingplan.top

Go:   strings.Repeat("ab", 3)
来源：http://ucc.fzhhl.top

Ruby: "ab" * 3
来源：http://zan.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dyu.tanke756.top

[E03] 截取子串
来源：http://atg.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://slu.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vdd.zhoulong.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://exl.yueranfly.top

TS:   s.slice(1, 4)
来源：http://lcz.0kj1m.cn

Java: s.substring(1, 4)
来源：http://xzy.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dti.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://fpm.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://jdt.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://eet.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://spz.yuxming.cn

PHP:  strpos($s, "x");
来源：http://gxd.zhixingplan.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://elf.jiagoushi.top

TS:   s.indexOf("x")
来源：http://oqe.zdqjudy.top

Java: s.indexOf("x")
来源：http://ceg.vehdjk.com

Go:   strings.Index(s, "x")
来源：http://czd.jianghu66.top

Ruby: s.index("x")
来源：http://wkx.sysykeji.top

C#:   s.IndexOf("x")
来源：http://xwc.yj202588.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pkd.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://coy.zdqjudy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://llr.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fsq.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fwa.xziqi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hlo.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pcc.fktsv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://akr.hesvh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hrz.xingfuxueyuan.xyz

[E06] 替换子串
来源：http://vja.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mtq.redwolf501.top

PHP:  str_replace("a", "b", $s);
来源：http://ujf.svipenyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://itp.nanxinkj.top

TS:   s.replaceAll("a", "b")
来源：http://pkz.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mqn.guowangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uun.shzxlz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vcm.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://unq.hywenlv.cn

[E07] 按分隔符拆分
来源：http://xwr.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rgm.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gnk.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vha.zhiwuduotai.top

TS:   s.split(",")
来源：http://jgl.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://sro.bjfxy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tcm.tarul.cn

Ruby: s.split(",");  s.split
来源：http://srq.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dpn.uphjek.com

[E08] 数组按分隔符合并
来源：http://zma.fengsongda.top

Py:   ",".join(items)
来源：http://hzt.havefunace.top

PHP:  implode(",", $items);
来源：http://dii.pengpengdd.cyou

JS:   items.join(",")
来源：http://rbc.jqgfzy.top

TS:   items.join(",")
来源：http://lvh.vehdjk.com

Java: String.join(",", items)
来源：http://cwp.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://uqg.epnwcf.com

Ruby: items.join(",")
来源：http://oxv.cashguo.top

C#:   string.Join(",", items)
来源：http://cqu.haohaochexian.top

[E09] 去除所有空白字符
来源：http://rad.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://drl.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bzx.sufxvd.cn

JS:   s.replace(/\s+/g, "")
来源：http://bvb.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://vly.wangdashe.top

Java: s.replaceAll("\\s+", "")
来源：http://fvr.yvedp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oty.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://ebb.snrcjt.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yio.zhixingplan.top

[E10] 左侧补零 / 定长填充
来源：http://qbd.gzhubu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ldc.xuetiantiany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zcn.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://fjg.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://crc.cheryme.top

Java: String.format("%03d", 7)
来源：http://xrp.mhx1999.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cio.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pbo.jinqigufen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wjf.yanxiufei.cn

[E11] 反转字符串
来源：http://xyy.quarkkingdee.top

Py:   s[::-1]
来源：http://yus.52xcode.cn

PHP:  strrev($s);
来源：http://ruk.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://oaz.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://idz.xuanzx.com

Java: new StringBuilder(s).reverse().toString()
来源：http://dlc.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kjv.zhengqikj.top

Ruby: s.reverse
来源：http://zrw.xuetiantiany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gwh.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://jsi.hcnkem.com

Py:   s.count("a")
来源：http://ohh.sweek.top

PHP:  substr_count($s, "a");
来源：http://kgb.zdqjudy.top

JS:   s.split("a").length - 1
来源：http://fkn.chenjidiqi.icu

TS:   s.split("a").length - 1
来源：http://lmo.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zwa.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://uvc.aizwys.cn

Ruby: s.count("a")
来源：http://xew.bbcook.cn

C#:   s.Count(c => c == 'a')
来源：http://llr.zhoulong.xyz

[E13] 逐字符遍历
来源：http://aqr.316326.xyz

Py:   for ch in s: print(ch)
来源：http://qci.chenjidiqi.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kex.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://sxc.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ebv.9152youxi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oya.sufxvd.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tbe.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://ujz.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vam.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://syd.yueranfly.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://byh.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://slf.daxiang520.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pgv.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://thd.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ioa.hcnkem.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ikb.nwbrower.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qky.quarkkingdee.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wyo.9152youxi.cn

[E15] HTML 转义 / 反转义
来源：http://jac.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xct.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yny.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tzp.jinghuilouyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pbb.xingfuxueyuan.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://izb.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xem.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ycz.vqdsnc.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://plf.sjlbkw.cn

[E16] 数字千分位
来源：http://oja.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://nzu.fktsv.cn

PHP:  number_format(1234567);
来源：http://axn.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://gdv.xingfuxueyuan.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://nel.jyoumei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jiw.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dzr.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uja.jinyuanbaomall.cn

C#:   1234567.ToString("N0")
来源：http://dge.tian-w.cn

[E17] 首字母大写
来源：http://gvj.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fqz.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jdv.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://luk.fzhhl.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xfc.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uqw.andypj.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ega.bbcook.cn

Ruby: s.capitalize
来源：http://gfg.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ald.jqgfzy.top

[E18] 模板占位符替换
来源：http://fak.yfazqb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jxd.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zzi.fengsongda.top

JS:   tpl.replaceAll("{name}", name)
来源：http://stc.yuanzhike.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mng.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ihz.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vst.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gvj.yj20258.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nlf.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://zqn.xingfuxueyuan.xyz

Py:   s.splitlines()
来源：http://lbw.fktsv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://paa.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://omi.tian-w.cn

TS:   s.split(/\r?\n/)
来源：http://vpv.redwolf501.top

Java: s.lines().toList()
来源：http://ceg.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://llz.hywenlv.cn

Ruby: s.lines
来源：http://ysk.shanyushiyangkeji.top

C#:   s.Split('\n')
来源：http://zio.pycfn.com

[E20] 判断字符串是否为空
来源：http://col.jinghuilouyu.cn

Py:   if not s:
来源：http://jph.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lra.zdqjudy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fin.dashuyun.cn

TS:   if (s === "") {}
来源：http://atd.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://kxf.shzxlz.cn

Go:   if s == "" {}
来源：http://qpb.hywenlv.cn

Ruby: if s.empty?
来源：http://toj.yuanzhike.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ctv.xylfe.cn

[E21] 超长截断加省略号
来源：http://fcj.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gag.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nla.uphjek.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://onx.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dyj.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nnm.cucudq.cn

Go:   // 按 rune 判断长度后截断
来源：http://gmg.snrcjt.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gla.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://opq.xuetiantiany.cn

[E22] 字节长度与字符长度
来源：http://stp.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xfh.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xrb.bjfxy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ejn.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rde.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nrj.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vqv.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://vdw.52xcode.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tpj.aibaodan.cn

================================================================================
来源：http://zlp.shuidangran.top

F. 文件与目录
来源：http://uso.sjlbkw.cn

================================================================================
来源：http://eaz.hnxiangtu.top

[F01] 读取整个文件
来源：http://qjx.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cbx.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://rpg.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sdo.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oih.yj20258888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://luc.hnxiangtu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vvg.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://kxi.sxryk.cn

C#:   File.ReadAllText("a.txt");
来源：http://gla.havefunace.top

[F02] 逐行读取文件
来源：http://hfc.shanyushiyangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://afb.fehbvm.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wyd.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hxv.nanxinkj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vwy.jianghu66.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://odj.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cge.pengpengdd.cyou

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ors.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kof.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://jja.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hwj.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yoa.dashuyun.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ofe.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xzv.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mtt.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gog.yvedp.cn

Ruby: File.write("a.txt", "hi")
来源：http://obu.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zkw.hywenlv.cn

[F04] 追加写入文件
来源：http://kqg.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zux.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xve.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sqd.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ckd.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iox.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gje.shuidangran.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://koj.cheryme.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wsk.jianghu66.top

[F05] 判断文件或目录是否存在
来源：http://pvo.havefunace.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vth.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://sbg.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://ake.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://mad.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://wqf.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ctk.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://tfn.yanxiufei.cn


<!-- 参考信息 -->