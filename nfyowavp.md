代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ddr.meibo888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yoc.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rad.meibo888.top

TS:   [...arr];
来源：http://txb.fehbvm.com

Java: new ArrayList<>(list);
来源：http://ebz.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://bpu.xylfe.cn

Ruby: arr.dup;  arr.clone
来源：http://nat.daria6918.cn

C#:   new List<int>(list);
来源：http://sqb.haohaochexian.top

[D23] reduce 累积计算
来源：http://vmd.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ikz.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://otd.andypj.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vkw.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wcn.shanyushiyangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nlu.kuanghao11.cn

Go:   // 手写循环
来源：http://gig.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nra.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zkg.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://erw.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wrw.tian-w.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cxb.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://inl.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://syb.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zwl.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uzv.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tcf.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zaa.zhoulong.xyz

[D25] Set 集合去重与交并差
来源：http://aol.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sku.zhengqikj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oet.mhx1999.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xbz.bjfxy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sxt.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://res.shanyushiyangtech.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ocs.jiagoushi.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vas.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ahj.vqdsnc.cn

[D26] 数组转字符串
来源：http://tzo.snrcjt.cn

Py:   ", ".join(map(str, arr))
来源：http://kjn.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://nkt.sweek.top

JS:   arr.join(", ")
来源：http://lha.feifeiyinyue.top

TS:   arr.join(", ")
来源：http://hws.tianlin.xyz

Java: String.join(", ", list)
来源：http://ndv.tian-w.cn

Go:   strings.Join(strs, ", ")
来源：http://lxn.yj202588.top

Ruby: arr.join(", ")
来源：http://tdb.yonumen.top

C#:   string.Join(", ", list)
来源：http://pjo.smart0.xyz

================================================================================
来源：http://dgm.yuxming.cn

E. 字符串处理
来源：http://jux.zdbjq.cn

================================================================================
来源：http://huw.guowangkeji.top

[E01] 拼接字符串
来源：http://aha.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jlr.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hbe.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sgc.fktsv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nvl.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://smr.jyoumei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://erl.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qyv.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://txo.guannengcc.top

[E02] 重复字符串
来源：http://fpl.c1oappe.top

Py:   "ab" * 3
来源：http://ulv.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://gmr.shanyushiyangtech.top

JS:   "ab".repeat(3)
来源：http://ebx.ydzc1.top

TS:   "ab".repeat(3)
来源：http://bac.ctjpmb.com

Java: "ab".repeat(3)
来源：http://mcs.52xcode.cn

Go:   strings.Repeat("ab", 3)
来源：http://yvx.fehbvm.com

Ruby: "ab" * 3
来源：http://zed.hesvh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eua.gaohongyu789.top

[E03] 截取子串
来源：http://uih.svipenyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://omb.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kmt.tianlin.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fdy.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://eer.yangfankeji.com

Java: s.substring(1, 4)
来源：http://zky.vqdsnc.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wiy.bbcook.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mdv.shzxlz.cn

C#:   s.Substring(1, 3)
来源：http://giu.nanxinkj.top

[E04] 查找子串位置
来源：http://vmm.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://wic.fengsongda.top

PHP:  strpos($s, "x");
来源：http://vav.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bbb.wangdashe.top

TS:   s.indexOf("x")
来源：http://hdv.quarkkingdee.top

Java: s.indexOf("x")
来源：http://dmc.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://jvt.zhengqikj.top

Ruby: s.index("x")
来源：http://vzd.fktsv.cn

C#:   s.IndexOf("x")
来源：http://hjc.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yyv.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ipq.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://noy.hongshengwenyu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qgo.guowangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ema.gogol.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qos.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hlc.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fzn.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://snj.shzxlz.cn

[E06] 替换子串
来源：http://aqv.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ofv.hongshengwenyu.top

PHP:  str_replace("a", "b", $s);
来源：http://pnm.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ovk.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://vtv.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rrx.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tmr.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jlh.tanke756.top

C#:   s.Replace("a", "b")
来源：http://hdo.jyoumei.cn

[E07] 按分隔符拆分
来源：http://fqe.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ikv.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://olx.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wmd.zdqjudy.top

TS:   s.split(",")
来源：http://efl.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://ubv.chenjidiqi.icu

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wja.yueranfly.top

Ruby: s.split(",");  s.split
来源：http://pvm.cheryme.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dfe.yongpay.top

[E08] 数组按分隔符合并
来源：http://mij.tianlin.xyz

Py:   ",".join(items)
来源：http://ign.gotoacloud.top

PHP:  implode(",", $items);
来源：http://nuy.sweek.top

JS:   items.join(",")
来源：http://xyr.zhiwuduotai.top

TS:   items.join(",")
来源：http://wmr.hcnkem.com

Java: String.join(",", items)
来源：http://wgo.c1oappe.top

Go:   strings.Join(items, ",")
来源：http://rub.hywenlv.cn

Ruby: items.join(",")
来源：http://rav.tianlin.xyz

C#:   string.Join(",", items)
来源：http://ahd.yongpay.top

[E09] 去除所有空白字符
来源：http://gof.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://plj.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dyr.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://bya.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://pwd.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://lyz.shuidangran.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://sdu.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://xlh.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mbs.wangshuangyany.cn

[E10] 左侧补零 / 定长填充
来源：http://ojw.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tfh.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cwo.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://xyn.zdbjq.cn

TS:   "7".padStart(3, "0")
来源：http://hip.hnxiangtu.top

Java: String.format("%03d", 7)
来源：http://jfh.gzhubu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nuy.xziqi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ika.pengpengdd.cyou

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kdl.yueranfly.top

[E11] 反转字符串
来源：http://xnm.xylfe.cn

Py:   s[::-1]
来源：http://cni.zhiwuduotai.top

PHP:  strrev($s);
来源：http://vun.yfazqb.com

JS:   [...s].reverse().join("")
来源：http://bbl.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://jxg.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zmu.ppjwa.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ihj.yangfankeji.com

Ruby: s.reverse
来源：http://skq.guannengcc.top

C#:   new string(s.Reverse().ToArray())
来源：http://ekz.smart0.xyz

[E12] 统计某字符出现次数
来源：http://rrz.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://cbn.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://ldj.sysykeji.top

JS:   s.split("a").length - 1
来源：http://qsb.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://wxo.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wdq.9152youxi.cn

Go:   strings.Count(s, "a")
来源：http://djf.yfazqb.com

Ruby: s.count("a")
来源：http://kqf.yanxiufei.cn

C#:   s.Count(c => c == 'a')
来源：http://ysk.yongpay.top

[E13] 逐字符遍历
来源：http://dqz.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://twt.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ust.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rtq.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://aih.xingfuxueyuan.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bzm.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qhi.fzhhl.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xpl.gzhubu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kug.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://snv.sjlbkw.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oop.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xdh.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://itb.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://siz.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iwe.smart0.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zzi.ivvv.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bqx.sufxvd.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mnk.yfazqb.com

[E15] HTML 转义 / 反转义
来源：http://yed.fktsv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zkb.cheryme.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rhk.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rgw.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fjq.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://drl.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vbn.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kzv.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oew.shanyushiyangkeji.top

[E16] 数字千分位
来源：http://lvf.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://oij.jqgfzy.top

PHP:  number_format(1234567);
来源：http://qma.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://emn.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://fyh.andypj.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zrq.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://akl.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nzs.quarkkingdee.top

C#:   1234567.ToString("N0")
来源：http://rkm.ybcxt.top

[E17] 首字母大写
来源：http://xdi.jqgfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dml.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://juc.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rdh.zhaomingkeji.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cya.ywan-chungtsiang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wud.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://piv.hammf.cn

Ruby: s.capitalize
来源：http://gsg.yfazqb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ekd.zdqjudy.top

[E18] 模板占位符替换
来源：http://tjb.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://irv.vehdjk.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ozc.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://zzt.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hpl.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jde.yongpay.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gup.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rte.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ejh.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://okt.hammf.cn

Py:   s.splitlines()
来源：http://ety.sxryk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hjq.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://xri.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://cow.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://sny.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://mdb.bbcook.cn

Ruby: s.lines
来源：http://sfd.zycfv.cn

C#:   s.Split('\n')
来源：http://hvf.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://qwi.yj20258888.top

Py:   if not s:
来源：http://owp.hnqzz.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cyl.tanke756.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://erc.guowangkeji.top

TS:   if (s === "") {}
来源：http://vng.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://jcg.ydzc1.top

Go:   if s == "" {}
来源：http://zer.aibaodan.cn

Ruby: if s.empty?
来源：http://ems.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cqr.shzxlz.cn

[E21] 超长截断加省略号
来源：http://alr.yj202588.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vwh.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kgl.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zhd.0kj1m.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ksl.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sai.ehwqpu.com

Go:   // 按 rune 判断长度后截断
来源：http://ulu.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sfm.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kle.hnxiangtu.top

[E22] 字节长度与字符长度
来源：http://plo.sxryk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xtp.meibo888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dfi.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ozz.ywan-chungtsiang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tqi.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uet.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kxs.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://obq.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uhm.havefunace.top

================================================================================
来源：http://doe.jlsjyb.cn

F. 文件与目录
来源：http://kiv.zhaomingkeji.xyz

================================================================================
来源：http://dyk.yueranfly.top

[F01] 读取整个文件
来源：http://zxi.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mqh.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://laa.jinghuilouyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qci.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tau.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nbo.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oki.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://lmt.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://kjq.shuidangran.top

[F02] 逐行读取文件
来源：http://jkr.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qzk.cdnleiting.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gkc.zhijiandao.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vgv.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aya.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mxg.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dqd.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eql.fehbvm.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fwt.sweek.top

[F03] 写入文件（覆盖）
来源：http://xeg.cashguo.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://drw.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jqr.dashuyun.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://akj.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kjb.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vpu.jinghuilouyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://viw.yongpay.top

Ruby: File.write("a.txt", "hi")
来源：http://lwq.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ucd.smart0.xyz

[F04] 追加写入文件
来源：http://zpo.pengpengdd.cyou

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xot.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qkc.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xqb.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rzb.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ufa.yj202588.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lyp.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vcg.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wna.quarkkingdee.top

[F05] 判断文件或目录是否存在
来源：http://dak.meibo888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pmc.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://gfi.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://oqv.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://kga.tianlin.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://dky.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tvq.shanyushiyangkeji.top

Ruby: File.exist?("a.txt")
来源：http://jaq.dashuyun.cn

C#:   File.Exists("a.txt")
来源：http://otd.svipenyu.cn

[F06] 删除文件
来源：http://ive.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://amy.ivvv.top

PHP:  unlink("a.txt");
来源：http://fvc.yj20258.top

JS:   fs.unlinkSync("a.txt")
来源：http://pbl.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://ums.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xrb.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://yev.fzhhl.top


<!-- 参考信息 -->