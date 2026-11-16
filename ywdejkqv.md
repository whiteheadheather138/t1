代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ilx.yfazqb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ycj.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://men.jiagoushi.top

Go:   // 手写 map[T]int
来源：http://hun.fzhhl.top

Ruby: arr.tally
来源：http://qao.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bgt.sysykeji.top

[D21] 判断是否包含某元素
来源：http://xbi.zhengqikj.top

Py:   x in arr
来源：http://koy.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://qdn.zhengqikj.top

JS:   arr.includes(x)
来源：http://prn.havefunace.top

TS:   arr.includes(x)
来源：http://ssi.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://koi.zhoulong.xyz

Go:   slices.Contains(arr, x)
来源：http://dyh.jiagoushi.top

Ruby: arr.include?(x)
来源：http://cqi.xuanzx.com

C#:   list.Contains(x)
来源：http://dtf.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://rri.jlsjyb.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lnh.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://prc.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://swg.sufxvd.cn

TS:   [...arr];
来源：http://ctt.jianghu66.top

Java: new ArrayList<>(list);
来源：http://smk.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tkg.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://irj.shuidangran.top

C#:   new List<int>(list);
来源：http://jhq.jqgfzy.top

[D23] reduce 累积计算
来源：http://wvt.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jef.chenjidiqi.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pxs.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aus.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pez.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ekm.zhiwuduotai.top

Go:   // 手写循环
来源：http://nap.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fyy.vehdjk.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rvp.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://nwr.birdmap.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zqy.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fky.bjfxy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yvp.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://msb.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mbu.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dwr.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eqe.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cyd.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://fme.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bbc.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://llv.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ftp.sxryk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jej.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xzd.yonumen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ugr.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eed.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yzf.xylfe.cn

[D26] 数组转字符串
来源：http://fnm.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://yms.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://ioz.jqgfzy.top

JS:   arr.join(", ")
来源：http://zas.epnwcf.com

TS:   arr.join(", ")
来源：http://nat.hongshengwenyu.top

Java: String.join(", ", list)
来源：http://ltf.jiagoushi.top

Go:   strings.Join(strs, ", ")
来源：http://lin.ybcxt.top

Ruby: arr.join(", ")
来源：http://gus.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://kmv.zhongyouzk.top

================================================================================
来源：http://geq.xingfuxueyuan.xyz

E. 字符串处理
来源：http://iqs.yj20258888.top

================================================================================
来源：http://cde.zycfv.cn

[E01] 拼接字符串
来源：http://etm.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xxy.jlsjyb.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hij.aizwys.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qvv.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iqp.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pyh.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uln.sweek.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cfm.shanyushiyangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qzn.ybcxt.top

[E02] 重复字符串
来源：http://ibg.kuanghao11.cn

Py:   "ab" * 3
来源：http://svb.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://bcu.bbcook.cn

JS:   "ab".repeat(3)
来源：http://pah.wangdashe.top

TS:   "ab".repeat(3)
来源：http://bbp.fktsv.cn

Java: "ab".repeat(3)
来源：http://sfd.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://xoy.xylfe.cn

Ruby: "ab" * 3
来源：http://dcg.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xdn.kuanghao11.cn

[E03] 截取子串
来源：http://bej.cqqwz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kwy.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://obp.nanxuanxn.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xgm.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://jxx.gotoacloud.top

Java: s.substring(1, 4)
来源：http://dud.hfpthk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://who.zhengqikj.top

Ruby: s[1, 3];  s[1..3]
来源：http://buq.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://yvt.yuanzhike.top

[E04] 查找子串位置
来源：http://aiz.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://elg.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://job.52xcode.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://drn.fengsongda.top

TS:   s.indexOf("x")
来源：http://hnb.aibaodan.cn

Java: s.indexOf("x")
来源：http://hrw.bjfxy.top

Go:   strings.Index(s, "x")
来源：http://nnr.birdmap.top

Ruby: s.index("x")
来源：http://pee.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://oeq.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cwe.fengsongda.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ett.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yfa.redwolf501.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cuh.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dsp.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://duz.yonumen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gnk.nanxuanxn.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uvt.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ddj.cashguo.top

[E06] 替换子串
来源：http://bpz.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://suf.jinqigufen.top

PHP:  str_replace("a", "b", $s);
来源：http://lks.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hxj.hfpthk.cn

TS:   s.replaceAll("a", "b")
来源：http://trx.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gve.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ajy.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eqt.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://svl.bjfxy.top

[E07] 按分隔符拆分
来源：http://nep.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bwm.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pub.9152youxi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://omc.yanxiufei.cn

TS:   s.split(",")
来源：http://jxz.cashguo.top

Java: s.split(",");  s.split("\\s+")
来源：http://dnv.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://til.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://dmx.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://che.sysykeji.top

[E08] 数组按分隔符合并
来源：http://yhs.jinqigfzy.top

Py:   ",".join(items)
来源：http://rwb.jinghuilouyu.cn

PHP:  implode(",", $items);
来源：http://slv.guowangkeji.top

JS:   items.join(",")
来源：http://tjj.zdqjudy.top

TS:   items.join(",")
来源：http://amd.birdmap.top

Java: String.join(",", items)
来源：http://ofk.yvedp.cn

Go:   strings.Join(items, ",")
来源：http://pid.hfpthk.cn

Ruby: items.join(",")
来源：http://khq.tanke756.top

C#:   string.Join(",", items)
来源：http://jsr.0kj1m.cn

[E09] 去除所有空白字符
来源：http://kkz.yj20258888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gcd.hcnkem.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gdo.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://ssw.jqgfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://xjl.fzhhl.top

Java: s.replaceAll("\\s+", "")
来源：http://rjp.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xmv.cqqwz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qjg.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qcs.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://shp.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kgf.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xnt.yfazqb.com

JS:   "7".padStart(3, "0")
来源：http://izt.dianchejie.cn

TS:   "7".padStart(3, "0")
来源：http://jko.iojbl.cn

Java: String.format("%03d", 7)
来源：http://gtw.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://utu.xziqi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mpv.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zfe.pengpengdd.cyou

[E11] 反转字符串
来源：http://bzv.quarkkingdee.top

Py:   s[::-1]
来源：http://mtd.tian-w.cn

PHP:  strrev($s);
来源：http://zly.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://idf.yj20258888.top

TS:   [...s].reverse().join("")
来源：http://cuf.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rvf.hfpthk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qri.jinghuilouyu.cn

Ruby: s.reverse
来源：http://ayo.ydjk.org.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ros.yongpay.top

[E12] 统计某字符出现次数
来源：http://crn.hysaishi.cn

Py:   s.count("a")
来源：http://aeh.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://iyj.yangfankeji.com

JS:   s.split("a").length - 1
来源：http://nzs.yonumen.top

TS:   s.split("a").length - 1
来源：http://lae.yueranfly.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://umn.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://oie.sxryk.cn

Ruby: s.count("a")
来源：http://kpl.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://sbu.wangdashe.top

[E13] 逐字符遍历
来源：http://bpw.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://neh.hnxiangtu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bsa.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rwt.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qxt.cucudq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vww.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vqx.zdbjq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://opp.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://utv.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://kvt.zhixingplan.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gen.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://quu.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://siu.epnwcf.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zvw.havefunace.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wbj.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://toj.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://teh.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tib.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://zlv.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ayu.daxiang520.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tzy.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vfl.vehdjk.com

TS:   // 同上，务必做 XSS 过滤
来源：http://gjf.ctjpmb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fnm.yvedp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tck.zhoulong.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jxo.hfpthk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qxu.aizwys.cn

[E16] 数字千分位
来源：http://ata.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://xcs.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://rhz.quarkkingdee.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cig.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ryw.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lmf.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aub.jlsjyb.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tpn.xingfuxueyuan.xyz

C#:   1234567.ToString("N0")
来源：http://xpl.xuanzx.com

[E17] 首字母大写
来源：http://szu.hysaishi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qog.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uoq.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bvx.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bnq.andypj.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://smi.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://efo.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://hjb.jiagoushi.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pce.shanyushiyangkeji.top

[E18] 模板占位符替换
来源：http://gcj.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tvw.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tge.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wmj.pycfn.com

TS:   tpl.replaceAll("{name}", name)
来源：http://oxz.fengsongda.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oeb.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ads.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lkj.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oww.ctjpmb.com

[E19] 多行文本按行拆分
来源：http://yzj.xuanzx.com

Py:   s.splitlines()
来源：http://ysb.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hdh.cqqwz.cn

JS:   s.split(/\r?\n/)
来源：http://hzj.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://phg.sxryk.cn

Java: s.lines().toList()
来源：http://edi.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://tvc.daria6918.cn

Ruby: s.lines
来源：http://whe.zdbjq.cn

C#:   s.Split('\n')
来源：http://vvm.havefunace.top

[E20] 判断字符串是否为空
来源：http://txf.xziqi.cn

Py:   if not s:
来源：http://nnd.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gun.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qtm.tarul.cn

TS:   if (s === "") {}
来源：http://etb.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://ehm.dianchejie.cn

Go:   if s == "" {}
来源：http://qty.fzhhl.top

Ruby: if s.empty?
来源：http://nwz.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fit.gogol.net.cn

[E21] 超长截断加省略号
来源：http://uzi.dianchejie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zki.daria6918.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hwd.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://usv.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zrp.yanxiufei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://spt.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://vhc.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ctl.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rlq.ivvv.top

[E22] 字节长度与字符长度
来源：http://xch.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lyb.nanxinkj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gwm.wangdashe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xia.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gcx.guannengcc.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://noz.nanxinkj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://elc.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://fhp.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gdd.sysykeji.top

================================================================================
来源：http://ipl.meibo888.top

F. 文件与目录
来源：http://uji.yuanzhike.top

================================================================================
来源：http://cxr.c1oappe.top

[F01] 读取整个文件
来源：http://fcg.shangyingyoupin.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zmw.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://dtx.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ufa.yj20258.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://els.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ohb.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://esc.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://gqw.svipenyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://gag.shzxlz.cn

[F02] 逐行读取文件
来源：http://djl.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jgs.xylfe.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ift.jiagoushi.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jyb.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bua.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fgu.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ufs.zhijiandao.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zoq.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qjf.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://kap.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vbv.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://fsz.sufxvd.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iyj.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xbg.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zpr.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ccv.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://cke.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://swj.c1oappe.top

[F04] 追加写入文件
来源：http://axd.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rjb.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cug.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qyd.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kcq.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dou.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pvs.tianlin.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vfs.ydjk.org.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uhc.yueranfly.top


<!-- 参考信息 -->