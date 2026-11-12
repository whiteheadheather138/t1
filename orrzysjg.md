代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uat.c1oappe.top

[D20] 统计每个元素出现次数
来源：http://mdw.jqgufenzy.top

Py:   Counter(arr)
来源：http://oec.zhijiandao.cn

PHP:  array_count_values($arr);
来源：http://nwo.redwolf501.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hyq.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://unz.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zhr.bjfxy.top

Go:   // 手写 map[T]int
来源：http://yjt.ctjpmb.com

Ruby: arr.tally
来源：http://rcs.jqgufenzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xma.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://mxt.jinyuanbaomall.cn

Py:   x in arr
来源：http://xtk.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://xkh.ydjk.org.cn

JS:   arr.includes(x)
来源：http://zcn.kuanghao11.cn

TS:   arr.includes(x)
来源：http://tdc.zhaomingkeji.xyz

Java: list.contains(x)
来源：http://uhc.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://qal.sweek.top

Ruby: arr.include?(x)
来源：http://djg.zdbjq.cn

C#:   list.Contains(x)
来源：http://ggc.pengpengdd.cyou

[D22] 复制数组（避免共享引用）
来源：http://owo.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oaz.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tub.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yko.hcnkem.com

TS:   [...arr];
来源：http://wot.epnwcf.com

Java: new ArrayList<>(list);
来源：http://zvp.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://jbc.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://tsc.fzhhl.top

C#:   new List<int>(list);
来源：http://cxf.wangdashe.top

[D23] reduce 累积计算
来源：http://ave.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xrf.xuanzx.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tii.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oqu.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jqv.xuetiantiany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tzn.epnwcf.com

Go:   // 手写循环
来源：http://ibj.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://toz.smart0.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://swe.ppjwa.cn

[D24] 字典 / Map 基本操作
来源：http://okc.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wcl.hnxiangtu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kfy.jianghu66.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eym.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dqe.zycfv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lag.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://haw.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pwz.yuxming.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gsi.uphjek.com

[D25] Set 集合去重与交并差
来源：http://gsi.iojbl.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iqt.52xcode.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vnq.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cij.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gaz.pycfn.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qfs.hywenlv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pih.ivvv.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dlc.havefunace.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://evb.cqqwz.cn

[D26] 数组转字符串
来源：http://gfq.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://zrp.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://byh.nanxuanxn.top

JS:   arr.join(", ")
来源：http://xau.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://xwu.ydjk.org.cn

Java: String.join(", ", list)
来源：http://ihi.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://icz.yuxming.cn

Ruby: arr.join(", ")
来源：http://ezw.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://rgr.hnqzz.top

================================================================================
来源：http://xvg.ctjpmb.com

E. 字符串处理
来源：http://vej.yanxiufei.cn

================================================================================
来源：http://fqd.jyoumei.cn

[E01] 拼接字符串
来源：http://lfa.yuanzhike.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dib.ydjk.org.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://shf.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bpv.ybcxt.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://woh.aizwys.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lza.yanxiufei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nmv.smart0.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gte.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nca.hnqzz.top

[E02] 重复字符串
来源：http://psj.jinqigfzy.top

Py:   "ab" * 3
来源：http://grx.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://jki.zhiwuduotai.top

JS:   "ab".repeat(3)
来源：http://jak.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://kpq.jqgfzy.top

Java: "ab".repeat(3)
来源：http://cuo.ybcxt.top

Go:   strings.Repeat("ab", 3)
来源：http://fjk.hongshengwenyu.top

Ruby: "ab" * 3
来源：http://rhj.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://emq.jyoumei.cn

[E03] 截取子串
来源：http://egd.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jbe.iojbl.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ans.yj202588.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xso.birdmap.top

TS:   s.slice(1, 4)
来源：http://afc.uphjek.com

Java: s.substring(1, 4)
来源：http://yvn.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ovm.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://qmp.birdmap.top

C#:   s.Substring(1, 3)
来源：http://yhl.jiagoushi.top

[E04] 查找子串位置
来源：http://qyc.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://csm.uphjek.com

PHP:  strpos($s, "x");
来源：http://qql.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rqu.birdmap.top

TS:   s.indexOf("x")
来源：http://xmx.fktsv.cn

Java: s.indexOf("x")
来源：http://gdn.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://pfz.nanxinkj.top

Ruby: s.index("x")
来源：http://cjp.yueranfly.top

C#:   s.IndexOf("x")
来源：http://bpy.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://mtj.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xpw.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pij.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sos.tarul.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cvm.tanke756.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://acc.nanxinkj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fvj.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://amn.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tew.wangshuangyany.cn

[E06] 替换子串
来源：http://gpu.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xcs.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://ouc.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://llp.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://ldi.hnxiangtu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://urf.dianchejie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wzn.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://env.daxiang520.top

C#:   s.Replace("a", "b")
来源：http://ubr.gotoacloud.top

[E07] 按分隔符拆分
来源：http://mox.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wto.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fkz.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://mew.jqgufenzy.top

TS:   s.split(",")
来源：http://yqy.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://nmp.cdnleiting.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jaf.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://qjw.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xvw.tian-w.cn

[E08] 数组按分隔符合并
来源：http://qhn.hammf.cn

Py:   ",".join(items)
来源：http://tqu.yongpay.top

PHP:  implode(",", $items);
来源：http://fog.sufxvd.cn

JS:   items.join(",")
来源：http://lut.yueranfly.top

TS:   items.join(",")
来源：http://vuq.dashuyun.cn

Java: String.join(",", items)
来源：http://czj.shzxlz.cn

Go:   strings.Join(items, ",")
来源：http://wfd.fzhhl.top

Ruby: items.join(",")
来源：http://jxk.cqqwz.cn

C#:   string.Join(",", items)
来源：http://bie.andypj.xyz

[E09] 去除所有空白字符
来源：http://wml.fzhhl.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://msu.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rdo.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://ahn.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://vwt.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://kaj.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dka.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://vev.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lzg.jianghu66.top

[E10] 左侧补零 / 定长填充
来源：http://raa.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://prx.shzxlz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cxp.jyoumei.cn

JS:   "7".padStart(3, "0")
来源：http://zzh.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://khc.yj20258.top

Java: String.format("%03d", 7)
来源：http://lki.zhongyouzk.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://dby.xuanzx.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bpk.yuanzhike.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zcr.shanyushiyangkeji.top

[E11] 反转字符串
来源：http://xtx.tianlin.xyz

Py:   s[::-1]
来源：http://rgx.wangshuangyany.cn

PHP:  strrev($s);
来源：http://yhc.jinqigfzy.top

JS:   [...s].reverse().join("")
来源：http://mjl.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://uub.yj20258.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kit.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://qqv.xuanzx.com

Ruby: s.reverse
来源：http://jjs.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tou.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://dbs.hammf.cn

Py:   s.count("a")
来源：http://elx.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://cdy.chenlongwang.top

JS:   s.split("a").length - 1
来源：http://vdw.nwbrower.top

TS:   s.split("a").length - 1
来源：http://rev.feifeiyinyue.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://frb.kuanghao11.cn

Go:   strings.Count(s, "a")
来源：http://jsy.cashguo.top

Ruby: s.count("a")
来源：http://fpb.ivvv.top

C#:   s.Count(c => c == 'a')
来源：http://yjy.yueranfly.top

[E13] 逐字符遍历
来源：http://nfj.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://ycw.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bkb.ivvv.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jde.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zht.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jyj.xziqi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qxt.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://lif.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://llu.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://twl.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rei.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rfs.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rzz.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tuk.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oyo.hcnkem.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lkk.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dvr.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qoz.nanxuanxn.top

[E15] HTML 转义 / 反转义
来源：http://ycf.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cvu.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rlm.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kvw.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qal.dashuyun.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yoq.gogol.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://egp.ybcxt.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ffw.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://exh.shangyingyoupin.top

[E16] 数字千分位
来源：http://ywo.guannengcc.top

Py:   f"{1234567:,}"
来源：http://ncc.sxryk.cn

PHP:  number_format(1234567);
来源：http://uhy.hywenlv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ayb.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ylh.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aaq.fengsongda.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qkd.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ijl.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://fqf.fktsv.cn

[E17] 首字母大写
来源：http://spr.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cvk.shanyushiyangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cbb.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://haj.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qxk.meibo888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lwj.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tro.meibo888.top

Ruby: s.capitalize
来源：http://yoz.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://elg.yfazqb.com

[E18] 模板占位符替换
来源：http://wrf.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ueh.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gfp.daxiang520.top

JS:   tpl.replaceAll("{name}", name)
来源：http://crx.gzhubu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://loe.nwbrower.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kcx.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://crx.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xtg.zhixingplan.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xzf.fehbvm.com

[E19] 多行文本按行拆分
来源：http://jbk.zhixingplan.top

Py:   s.splitlines()
来源：http://ypq.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ilx.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://nla.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://nue.tianlin.xyz

Java: s.lines().toList()
来源：http://qiz.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://zgi.jinqigfzy.top

Ruby: s.lines
来源：http://ekm.jianghu66.top

C#:   s.Split('\n')
来源：http://zmn.yvedp.cn

[E20] 判断字符串是否为空
来源：http://ekh.chenjidiqi.icu

Py:   if not s:
来源：http://tvy.chenjidiqi.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://glq.jyoumei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nci.zdbjq.cn

TS:   if (s === "") {}
来源：http://aeq.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://mna.kuanghao11.cn

Go:   if s == "" {}
来源：http://fgy.yj20258888.top

Ruby: if s.empty?
来源：http://tig.hywenlv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jgx.snrcjt.cn

[E21] 超长截断加省略号
来源：http://xkl.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xkm.guannengcc.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rxx.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ddj.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jcp.fktsv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://isl.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://jjq.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jea.fehbvm.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dfb.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://zsh.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ipm.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ege.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://glu.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xcy.sysykeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wqd.hnxiangtu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sys.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://ebr.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bpa.jinghuilouyu.cn

================================================================================
来源：http://nig.meibo888.top

F. 文件与目录
来源：http://ojg.zycfv.cn

================================================================================
来源：http://jxl.jqgufenzy.top

[F01] 读取整个文件
来源：http://sty.jqgufenzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dyv.chenjidiqi.icu

PHP:  file_get_contents("a.txt");
来源：http://hnt.jqgfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tdl.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://quz.mhx1999.top

Java: Files.readString(Path.of("a.txt"))
来源：http://flm.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zln.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://kbe.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://mex.bjfxy.top

[F02] 逐行读取文件
来源：http://cyi.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://omk.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dqj.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hfk.pengpengdd.cyou

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ndy.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://svf.xziqi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ycb.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://htr.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tgs.tianlin.xyz

[F03] 写入文件（覆盖）
来源：http://fjv.xingfuxueyuan.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gnf.hysaishi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ocn.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iac.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kjs.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nnd.dashuyun.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eax.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://msf.snrcjt.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ivw.fehbvm.com

[F04] 追加写入文件
来源：http://yqe.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eis.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yxq.ehwqpu.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qnm.fzhhl.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://owo.epnwcf.com


<!-- 参考信息 -->