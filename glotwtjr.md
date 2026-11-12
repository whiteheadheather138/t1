代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://rqd.shanyushiyangtech.top

Ruby: arr.include?(x)
来源：http://cnq.uphjek.com

C#:   list.Contains(x)
来源：http://sii.c1oappe.top

[D22] 复制数组（避免共享引用）
来源：http://ewr.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eoz.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ywz.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://imk.gaohongyu789.top

TS:   [...arr];
来源：http://yho.yvedp.cn

Java: new ArrayList<>(list);
来源：http://evk.xuetiantiany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pmp.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://ury.yonumen.top

C#:   new List<int>(list);
来源：http://lby.iojbl.cn

[D23] reduce 累积计算
来源：http://ejz.epnwcf.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xwd.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://miy.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wgv.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sxh.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rtq.9152youxi.cn

Go:   // 手写循环
来源：http://ujy.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xja.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pdw.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://hca.c1oappe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sxl.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tda.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fdo.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rta.vehdjk.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ovz.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ord.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mge.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bjs.zhaomingkeji.xyz

[D25] Set 集合去重与交并差
来源：http://ueu.shanyushiyangtech.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cxe.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uuc.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cdk.cdnleiting.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bsz.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dpv.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://adn.wangshuangyany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://liy.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://szt.chenzaomai.com

[D26] 数组转字符串
来源：http://xim.zycfv.cn

Py:   ", ".join(map(str, arr))
来源：http://jwa.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://wuw.xziqi.cn

JS:   arr.join(", ")
来源：http://brp.cashguo.top

TS:   arr.join(", ")
来源：http://kry.aizwys.cn

Java: String.join(", ", list)
来源：http://ugz.mhx1999.top

Go:   strings.Join(strs, ", ")
来源：http://dnc.nanxinkj.top

Ruby: arr.join(", ")
来源：http://aaa.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://nao.pengpengdd.cyou

================================================================================
来源：http://frg.fengsongda.top

E. 字符串处理
来源：http://ubt.vehdjk.com

================================================================================
来源：http://igr.hysaishi.cn

[E01] 拼接字符串
来源：http://tqh.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hek.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fpq.yangfankeji.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tuc.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xsy.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fqd.jinyuanbaomall.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tze.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gul.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pqe.aizwys.cn

[E02] 重复字符串
来源：http://dxx.vehdjk.com

Py:   "ab" * 3
来源：http://puk.guannengcc.top

PHP:  str_repeat("ab", 3);
来源：http://tti.ybcxt.top

JS:   "ab".repeat(3)
来源：http://nvs.dianchejie.cn

TS:   "ab".repeat(3)
来源：http://nrd.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://rcb.yfazqb.com

Go:   strings.Repeat("ab", 3)
来源：http://mpa.hammf.cn

Ruby: "ab" * 3
来源：http://idv.hcnkem.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mbj.chenjidiqi.icu

[E03] 截取子串
来源：http://hne.jqgufenzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eqz.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hyr.shangyingyoupin.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jdi.sysykeji.top

TS:   s.slice(1, 4)
来源：http://mft.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://bgd.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rzs.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://bez.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://qiu.shuidangran.top

[E04] 查找子串位置
来源：http://egw.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://jhd.smart0.xyz

PHP:  strpos($s, "x");
来源：http://tyv.jyoumei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fhy.yongpay.top

TS:   s.indexOf("x")
来源：http://rux.nanxinkj.top

Java: s.indexOf("x")
来源：http://ayu.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://kwh.yangfankeji.com

Ruby: s.index("x")
来源：http://ifl.sufxvd.cn

C#:   s.IndexOf("x")
来源：http://ouw.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uwf.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yql.yfazqb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ayl.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qbe.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vqv.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bgt.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://esq.wangdashe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hyj.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sut.ybcxt.top

[E06] 替换子串
来源：http://zuw.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xdf.zhengqikj.top

PHP:  str_replace("a", "b", $s);
来源：http://omd.zhengqikj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://loe.pengpengdd.cyou

TS:   s.replaceAll("a", "b")
来源：http://arx.cqqwz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hpu.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://emf.mhx1999.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hxp.ydjk.org.cn

C#:   s.Replace("a", "b")
来源：http://hjl.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://gaq.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ilo.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pvo.sweek.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dfg.bjfxy.top

TS:   s.split(",")
来源：http://zcu.xingfuxueyuan.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://yge.fktsv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cnv.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://mro.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://khe.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://mam.ppjwa.cn

Py:   ",".join(items)
来源：http://svh.sysykeji.top

PHP:  implode(",", $items);
来源：http://aqm.zdqjudy.top

JS:   items.join(",")
来源：http://qeh.zhengqikj.top

TS:   items.join(",")
来源：http://hav.hfpthk.cn

Java: String.join(",", items)
来源：http://dhj.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://qtg.bjfxy.top

Ruby: items.join(",")
来源：http://tub.shuidangran.top

C#:   string.Join(",", items)
来源：http://ayr.hysaishi.cn

[E09] 去除所有空白字符
来源：http://tif.uphjek.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cxj.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ggs.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://qvr.cucudq.cn

TS:   s.replace(/\s+/g, "")
来源：http://brh.tarul.cn

Java: s.replaceAll("\\s+", "")
来源：http://lzr.wangdashe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bxg.guowangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://hfy.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://euc.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://bqj.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lit.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ran.ywan-chungtsiang.top

JS:   "7".padStart(3, "0")
来源：http://rgd.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://dqk.gaohongyu789.top

Java: String.format("%03d", 7)
来源：http://gcw.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cbp.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://htz.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ste.yj20258888.top

[E11] 反转字符串
来源：http://wqv.hnqzz.top

Py:   s[::-1]
来源：http://del.dianchejie.cn

PHP:  strrev($s);
来源：http://akg.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://tdo.nanxinkj.top

TS:   [...s].reverse().join("")
来源：http://mxb.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pei.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jnm.ctjpmb.com

Ruby: s.reverse
来源：http://ynn.shanyushiyangtech.top

C#:   new string(s.Reverse().ToArray())
来源：http://iwo.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://tbe.bbcook.cn

Py:   s.count("a")
来源：http://iip.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://qgq.shuidangran.top

JS:   s.split("a").length - 1
来源：http://ugg.ydzc1.top

TS:   s.split("a").length - 1
来源：http://hgo.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iuw.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://frx.ybcxt.top

Ruby: s.count("a")
来源：http://cxo.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://gnj.andypj.xyz

[E13] 逐字符遍历
来源：http://dcd.daxiang520.top

Py:   for ch in s: print(ch)
来源：http://xye.dianchejie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jvi.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yru.daxiang520.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mrr.aibaodan.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://idj.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bee.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://acq.tianlin.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kmc.yvedp.cn

[E14] URL 编码与 Base64
来源：http://fmt.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lzp.vehdjk.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://jpf.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gwb.nanxuanxn.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://awy.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dpc.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hxp.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tkb.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gnj.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://uvp.gzhubu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://khd.xinyue.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://whe.ehwqpu.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://afo.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gwb.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hpj.hcnkem.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rkz.ybcxt.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kwu.9152youxi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bih.jqgufenzy.top

[E16] 数字千分位
来源：http://jnu.birdmap.top

Py:   f"{1234567:,}"
来源：http://iyx.ctjpmb.com

PHP:  number_format(1234567);
来源：http://roj.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mbo.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://enb.fanxiaobao.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fzt.chenzaomai.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ejr.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wlo.birdmap.top

C#:   1234567.ToString("N0")
来源：http://lfq.havefunace.top

[E17] 首字母大写
来源：http://itg.ywan-chungtsiang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aat.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ank.haohaochexian.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nou.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ghy.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fvp.yongpay.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gvg.iojbl.cn

Ruby: s.capitalize
来源：http://kdc.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://frw.chenjidiqi.icu

[E18] 模板占位符替换
来源：http://dmu.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wru.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://djt.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hku.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://psj.jianghu66.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bia.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sbb.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zse.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lje.tarul.cn

[E19] 多行文本按行拆分
来源：http://vsx.cdnleiting.top

Py:   s.splitlines()
来源：http://jrd.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iyp.hywenlv.cn

JS:   s.split(/\r?\n/)
来源：http://akc.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://gin.316326.xyz

Java: s.lines().toList()
来源：http://zrh.yongpay.top

Go:   strings.Split(s, "\n")
来源：http://uvw.andypj.xyz

Ruby: s.lines
来源：http://qpc.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://fcm.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://byt.cashguo.top

Py:   if not s:
来源：http://edf.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wqa.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aeb.smart0.xyz

TS:   if (s === "") {}
来源：http://nbp.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://bjm.ctjpmb.com

Go:   if s == "" {}
来源：http://mmx.yuxming.cn

Ruby: if s.empty?
来源：http://jfw.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cqg.9152youxi.cn

[E21] 超长截断加省略号
来源：http://arx.yuxming.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lqw.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lth.snrcjt.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nvg.bjfxy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://twl.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bnm.shanyushiyangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://kkl.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uri.ehwqpu.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vot.xuetiantiany.cn

[E22] 字节长度与字符长度
来源：http://ypq.havefunace.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kfd.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ydm.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kvz.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lms.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://key.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://odi.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://uhd.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gtm.yonumen.top

================================================================================
来源：http://msf.mhx1999.top

F. 文件与目录
来源：http://ptf.ctjpmb.com

================================================================================
来源：http://wbr.chenlongwang.top

[F01] 读取整个文件
来源：http://byd.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hlj.yonumen.top

PHP:  file_get_contents("a.txt");
来源：http://jvx.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jzt.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hfy.hnqzz.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dik.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rgu.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://qxq.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://jze.andypj.xyz

[F02] 逐行读取文件
来源：http://lst.nwbrower.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wpr.sxryk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://duk.hesvh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://red.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mbm.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://knn.sufxvd.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hjm.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ysu.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mfq.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://dhz.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pzn.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bmq.cucudq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gic.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ofc.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kfz.zdbjq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xlo.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://uac.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kpl.jqgfzy.top

[F04] 追加写入文件
来源：http://rcg.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kez.jianghu66.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zpj.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vlc.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://osu.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fui.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yvo.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hdv.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lzj.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://wdr.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://epl.dashuyun.cn

PHP:  file_exists("a.txt");
来源：http://pxd.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://ohx.dashuyun.cn

TS:   fs.existsSync("a.txt")
来源：http://rjc.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://unf.ydjk.org.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pcj.hfpthk.cn

Ruby: File.exist?("a.txt")
来源：http://rbh.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://vzf.ctjpmb.com

[F06] 删除文件
来源：http://mrp.yuanzhike.top

Py:   os.remove("a.txt")
来源：http://zkm.yj20258.top

PHP:  unlink("a.txt");
来源：http://abn.havefunace.top


<!-- 参考信息 -->