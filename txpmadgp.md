代发 wailian999

Ruby: arr.tally
来源：http://wrw.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vjp.shuidangran.top

[D21] 判断是否包含某元素
来源：http://mtg.daria6918.cn

Py:   x in arr
来源：http://nsq.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://fyy.epnwcf.com

JS:   arr.includes(x)
来源：http://bwb.redwolf501.top

TS:   arr.includes(x)
来源：http://fvz.hongshengwenyu.top

Java: list.contains(x)
来源：http://ibt.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://rks.yangfankeji.com

Ruby: arr.include?(x)
来源：http://ypm.yvedp.cn

C#:   list.Contains(x)
来源：http://tuq.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://dbi.zdbjq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jrd.dashuyun.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wkg.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://thm.xinyue.icu

TS:   [...arr];
来源：http://snp.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://ezu.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://eyo.redwolf501.top

Ruby: arr.dup;  arr.clone
来源：http://zzb.haohaochexian.top

C#:   new List<int>(list);
来源：http://frw.daxiang520.top

[D23] reduce 累积计算
来源：http://yot.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://snk.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uki.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mlj.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://myb.yvedp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bbg.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://vbe.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://amr.aizwys.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://doo.svipenyu.cn

[D24] 字典 / Map 基本操作
来源：http://tww.bbcook.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xzl.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vys.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jrl.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://how.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dfv.xingfuxueyuan.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oig.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xlk.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://guz.pycfn.com

[D25] Set 集合去重与交并差
来源：http://eet.ybcxt.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rew.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gkv.hcnkem.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hff.9152youxi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jbk.havefunace.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://knn.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uhb.cashguo.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yxd.c1oappe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://spi.guannengcc.top

[D26] 数组转字符串
来源：http://mhp.aizwys.cn

Py:   ", ".join(map(str, arr))
来源：http://tiv.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://grw.jlsjyb.cn

JS:   arr.join(", ")
来源：http://mft.zdbjq.cn

TS:   arr.join(", ")
来源：http://mox.havefunace.top

Java: String.join(", ", list)
来源：http://wea.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://jkr.dashuyun.cn

Ruby: arr.join(", ")
来源：http://xvh.jlsjyb.cn

C#:   string.Join(", ", list)
来源：http://qvu.yfazqb.com

================================================================================
来源：http://bjb.meibo888.top

E. 字符串处理
来源：http://yrv.jinqigufen.top

================================================================================
来源：http://xxr.cqqwz.cn

[E01] 拼接字符串
来源：http://qwc.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ocm.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rqd.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dxn.cucudq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ppv.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qqx.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vuz.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qym.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fjb.svipenyu.cn

[E02] 重复字符串
来源：http://skj.fehbvm.com

Py:   "ab" * 3
来源：http://rfh.yonumen.top

PHP:  str_repeat("ab", 3);
来源：http://slo.aizwys.cn

JS:   "ab".repeat(3)
来源：http://laa.yongpay.top

TS:   "ab".repeat(3)
来源：http://tiz.yj20258888.top

Java: "ab".repeat(3)
来源：http://zms.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://kan.xylfe.cn

Ruby: "ab" * 3
来源：http://aez.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ezo.zhongyouzk.top

[E03] 截取子串
来源：http://gik.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dsm.cucudq.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://paa.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vfk.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://hvj.cqqwz.cn

Java: s.substring(1, 4)
来源：http://eyb.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rcf.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://rdc.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://wru.shanyushiyangtech.top

[E04] 查找子串位置
来源：http://zhv.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://lqe.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://tpe.9152youxi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bzk.yuanzhike.top

TS:   s.indexOf("x")
来源：http://liv.sweek.top

Java: s.indexOf("x")
来源：http://tqq.pengpengdd.cyou

Go:   strings.Index(s, "x")
来源：http://hbh.svipenyu.cn

Ruby: s.index("x")
来源：http://gci.cucudq.cn

C#:   s.IndexOf("x")
来源：http://mfr.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kaq.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oit.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rwv.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wvc.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jzl.guowangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rsk.ydjk.org.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ctv.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vcm.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eqr.sweek.top

[E06] 替换子串
来源：http://ckt.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kuh.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://gfp.kuanghao11.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kvx.chenjidiqi.icu

TS:   s.replaceAll("a", "b")
来源：http://vxf.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rzn.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ptr.wangshuangyany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qav.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://ixx.havefunace.top

[E07] 按分隔符拆分
来源：http://dqf.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gsn.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kre.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tid.havefunace.top

TS:   s.split(",")
来源：http://err.feifeiyinyue.top

Java: s.split(",");  s.split("\\s+")
来源：http://pwe.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fvb.pycfn.com

Ruby: s.split(",");  s.split
来源：http://pyx.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eur.tarul.cn

[E08] 数组按分隔符合并
来源：http://jdd.epnwcf.com

Py:   ",".join(items)
来源：http://sxz.hysaishi.cn

PHP:  implode(",", $items);
来源：http://lqi.hcnkem.com

JS:   items.join(",")
来源：http://xgg.jinqigufen.top

TS:   items.join(",")
来源：http://gih.uphjek.com

Java: String.join(",", items)
来源：http://jcd.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://can.sjlbkw.cn

Ruby: items.join(",")
来源：http://itv.zycfv.cn

C#:   string.Join(",", items)
来源：http://bwe.shuidangran.top

[E09] 去除所有空白字符
来源：http://czr.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://isl.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tyc.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://xfd.gotoacloud.top

TS:   s.replace(/\s+/g, "")
来源：http://usr.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://cgf.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://pes.zdbjq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xxn.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jcc.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://pvg.fzhhl.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fgl.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://chf.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://smf.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://cvw.bbcook.cn

Java: String.format("%03d", 7)
来源：http://rve.ctjpmb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ahz.dianchejie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jnb.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oxf.hnqzz.top

[E11] 反转字符串
来源：http://ccr.hysaishi.cn

Py:   s[::-1]
来源：http://ixi.tanke756.top

PHP:  strrev($s);
来源：http://mxh.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://tei.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://lfr.ydjk.org.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ygw.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ibh.jinqigfzy.top

Ruby: s.reverse
来源：http://yfw.yonumen.top

C#:   new string(s.Reverse().ToArray())
来源：http://ush.xziqi.cn

[E12] 统计某字符出现次数
来源：http://cch.hesvh.cn

Py:   s.count("a")
来源：http://mze.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://sql.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://shz.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://jex.hammf.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bnv.yonumen.top

Go:   strings.Count(s, "a")
来源：http://yvl.9152youxi.cn

Ruby: s.count("a")
来源：http://nmv.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://oti.yonumen.top

[E13] 逐字符遍历
来源：http://gij.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://bcd.tianlin.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yye.ydjk.org.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ggl.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yge.chenzaomai.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iev.xingfuxueyuan.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zab.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uin.gzhubu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ucz.birdmap.top

[E14] URL 编码与 Base64
来源：http://goz.tianlin.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://laj.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://osu.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hjd.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://otp.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zjm.aibaodan.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ush.fzhhl.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ggf.iojbl.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hgq.hywenlv.cn

[E15] HTML 转义 / 反转义
来源：http://cme.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rcq.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zea.ehwqpu.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jnr.cucudq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wuf.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fal.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kmr.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uif.tanke756.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pab.ppjwa.cn

[E16] 数字千分位
来源：http://nbq.chenlongwang.top

Py:   f"{1234567:,}"
来源：http://spl.meibo888.top

PHP:  number_format(1234567);
来源：http://rdw.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xhm.guowangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xdk.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://olb.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dgj.chenjidiqi.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xkp.zycfv.cn

C#:   1234567.ToString("N0")
来源：http://srw.yj20258888.top

[E17] 首字母大写
来源：http://nwn.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qys.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mkp.meibo888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dhp.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lns.ehwqpu.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ngv.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uqc.yj20258888.top

Ruby: s.capitalize
来源：http://tqi.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tkz.yongpay.top

[E18] 模板占位符替换
来源：http://kii.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lrt.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bwg.hcnkem.com

JS:   tpl.replaceAll("{name}", name)
来源：http://jhu.yj202588.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wyi.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rda.jinyuanbaomall.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://klu.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rwc.mhx1999.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ryb.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://qta.sufxvd.cn

Py:   s.splitlines()
来源：http://kkt.zdqjudy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mrd.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://uti.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://hsf.xuanzx.com

Java: s.lines().toList()
来源：http://vzh.snrcjt.cn

Go:   strings.Split(s, "\n")
来源：http://zff.dashuyun.cn

Ruby: s.lines
来源：http://hft.ehwqpu.com

C#:   s.Split('\n')
来源：http://hgl.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://hog.cdnleiting.top

Py:   if not s:
来源：http://fjg.gzhubu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nhe.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://myg.vqdsnc.cn

TS:   if (s === "") {}
来源：http://yfd.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://yvm.uphjek.com

Go:   if s == "" {}
来源：http://gqu.smart0.xyz

Ruby: if s.empty?
来源：http://kcn.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tht.pycfn.com

[E21] 超长截断加省略号
来源：http://ysc.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nza.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tme.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bpw.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wqt.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ovn.yanxiufei.cn

Go:   // 按 rune 判断长度后截断
来源：http://crj.zdbjq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nir.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qos.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://ngw.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nip.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://frv.guannengcc.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dkl.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://idn.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mqh.zdbjq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yoh.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://joi.ctjpmb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gaa.zhongyouzk.top

================================================================================
来源：http://glf.zdqjudy.top

F. 文件与目录
来源：http://mmu.havefunace.top

================================================================================
来源：http://tyz.sxryk.cn

[F01] 读取整个文件
来源：http://psv.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hxw.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://qzj.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jes.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wdz.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://njx.52xcode.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://esn.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://afn.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://etv.zhongyouzk.top

[F02] 逐行读取文件
来源：http://ncv.9152youxi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zbq.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wwn.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yer.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zwk.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://npc.ydjk.org.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hsy.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oxo.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kwq.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://lst.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zhd.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://iwt.uphjek.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qzv.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cmf.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vau.gogol.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ukd.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://lqm.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dfi.xuetiantiany.cn

[F04] 追加写入文件
来源：http://lbd.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uov.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gws.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jea.bbcook.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fxb.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yhw.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kmc.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ucg.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://onh.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://nwe.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vwo.tarul.cn

PHP:  file_exists("a.txt");
来源：http://vnc.aizwys.cn

JS:   fs.existsSync("a.txt")
来源：http://hwr.52xcode.cn


<!-- 参考信息 -->