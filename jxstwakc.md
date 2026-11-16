代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://alc.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wta.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://gou.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ejj.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jto.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://whu.kuanghao11.cn

Py:   Counter(arr)
来源：http://ycd.yj202588.top

PHP:  array_count_values($arr);
来源：http://vua.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tkl.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pbt.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ucg.xziqi.cn

Go:   // 手写 map[T]int
来源：http://xco.birdmap.top

Ruby: arr.tally
来源：http://kwt.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://que.ehwqpu.com

[D21] 判断是否包含某元素
来源：http://lde.hysaishi.cn

Py:   x in arr
来源：http://hvg.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://uvi.pycfn.com

JS:   arr.includes(x)
来源：http://yrg.dianchejie.cn

TS:   arr.includes(x)
来源：http://elh.hcnkem.com

Java: list.contains(x)
来源：http://wiw.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://xcl.ppjwa.cn

Ruby: arr.include?(x)
来源：http://rtn.sufxvd.cn

C#:   list.Contains(x)
来源：http://erg.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://mgq.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xzf.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yij.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vxb.hcnkem.com

TS:   [...arr];
来源：http://dwc.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://yfa.pengpengdd.cyou

Go:   copied := append([]int(nil), arr...)
来源：http://sir.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://qzu.kuanghao11.cn

C#:   new List<int>(list);
来源：http://qfn.yj20258888.top

[D23] reduce 累积计算
来源：http://fxp.hnxiangtu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qnp.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dkd.jinqigufen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wou.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fhr.xuetiantiany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://aqv.fanxiaobao.xyz

Go:   // 手写循环
来源：http://hfl.aizwys.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pep.iojbl.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pbc.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://lmy.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mau.dianchejie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://awe.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pgc.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eiz.pycfn.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://srt.tanke756.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vuv.jinqigfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://urs.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eck.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://hwz.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://shp.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://azr.shuidangran.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wea.zhengqikj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dkh.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hyn.tianlin.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://woz.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vlf.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lvq.xingfuxueyuan.xyz

[D26] 数组转字符串
来源：http://roz.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://mjh.hywenlv.cn

PHP:  implode(", ", $arr);
来源：http://grb.jlsjyb.cn

JS:   arr.join(", ")
来源：http://ydj.hnxiangtu.top

TS:   arr.join(", ")
来源：http://ifk.shangyingyoupin.top

Java: String.join(", ", list)
来源：http://abg.yj20258888.top

Go:   strings.Join(strs, ", ")
来源：http://sel.feifeiyinyue.top

Ruby: arr.join(", ")
来源：http://rud.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://vxi.fehbvm.com

================================================================================
来源：http://wye.yuxming.cn

E. 字符串处理
来源：http://mmv.chenlongwang.top

================================================================================
来源：http://yrm.yanxiufei.cn

[E01] 拼接字符串
来源：http://hpw.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ebb.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nqd.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ecd.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://izm.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tnh.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://odw.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dlr.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cjy.zhengqikj.top

[E02] 重复字符串
来源：http://cfr.316326.xyz

Py:   "ab" * 3
来源：http://qhn.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://mul.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://utf.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://jjd.yj20258888.top

Java: "ab".repeat(3)
来源：http://klz.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://obr.daxiang520.top

Ruby: "ab" * 3
来源：http://kll.jqgufenzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qlp.hnxiangtu.top

[E03] 截取子串
来源：http://cyx.aizwys.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wgm.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jgp.hnqzz.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xlf.zhijiandao.cn

TS:   s.slice(1, 4)
来源：http://lms.yuanzhike.top

Java: s.substring(1, 4)
来源：http://qco.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gov.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dcl.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://eqs.meibo888.top

[E04] 查找子串位置
来源：http://hml.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://qjq.zhiwuduotai.top

PHP:  strpos($s, "x");
来源：http://suo.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pid.bjfxy.top

TS:   s.indexOf("x")
来源：http://zzy.316326.xyz

Java: s.indexOf("x")
来源：http://agl.yj202588.top

Go:   strings.Index(s, "x")
来源：http://jrs.aizwys.cn

Ruby: s.index("x")
来源：http://sdm.yonumen.top

C#:   s.IndexOf("x")
来源：http://jfy.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qfa.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dod.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zso.redwolf501.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jmn.cashguo.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qqy.aizwys.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qgp.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kpj.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gcj.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qek.hongshengwenyu.top

[E06] 替换子串
来源：http://git.zdbjq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lqn.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://ote.chenlongwang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kpn.feifeiyinyue.top

TS:   s.replaceAll("a", "b")
来源：http://sct.jqgufenzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vzw.jiagoushi.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hjw.wangshuangyany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zcy.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://cjk.chenjidiqi.icu

[E07] 按分隔符拆分
来源：http://gqg.xziqi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zyz.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tzz.fengsongda.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ynk.guannengcc.top

TS:   s.split(",")
来源：http://utq.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://gfx.nanxuanxn.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://npl.vehdjk.com

Ruby: s.split(",");  s.split
来源：http://hav.yj20258888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://glg.zycfv.cn

[E08] 数组按分隔符合并
来源：http://jpm.svipenyu.cn

Py:   ",".join(items)
来源：http://afh.bjfxy.top

PHP:  implode(",", $items);
来源：http://kar.iojbl.cn

JS:   items.join(",")
来源：http://tqq.chenjidiqi.icu

TS:   items.join(",")
来源：http://qgg.sweek.top

Java: String.join(",", items)
来源：http://bvl.gzhubu.top

Go:   strings.Join(items, ",")
来源：http://xaa.shanyushiyangtech.top

Ruby: items.join(",")
来源：http://olp.316326.xyz

C#:   string.Join(",", items)
来源：http://jfb.chenjidiqi.icu

[E09] 去除所有空白字符
来源：http://xib.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gin.ctjpmb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lsg.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://kpt.hfpthk.cn

TS:   s.replace(/\s+/g, "")
来源：http://rff.shanyushiyangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://vvm.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tdg.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://cls.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vbk.zhaomingkeji.xyz

[E10] 左侧补零 / 定长填充
来源：http://huv.fktsv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vav.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dht.daxiang520.top

JS:   "7".padStart(3, "0")
来源：http://jyj.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://din.hywenlv.cn

Java: String.format("%03d", 7)
来源：http://qfe.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://oqy.aizwys.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wuy.zhixingplan.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ozy.yonumen.top

[E11] 反转字符串
来源：http://qtg.jqgfzy.top

Py:   s[::-1]
来源：http://iqc.daria6918.cn

PHP:  strrev($s);
来源：http://lym.quarkkingdee.top

JS:   [...s].reverse().join("")
来源：http://yxj.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://qkq.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://hxb.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://gkb.uphjek.com

Ruby: s.reverse
来源：http://lpn.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://bwy.hongshengwenyu.top

[E12] 统计某字符出现次数
来源：http://brh.epnwcf.com

Py:   s.count("a")
来源：http://pes.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://lkf.tian-w.cn

JS:   s.split("a").length - 1
来源：http://uoc.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://ebw.vqdsnc.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ylq.shuidangran.top

Go:   strings.Count(s, "a")
来源：http://hdh.ivvv.top

Ruby: s.count("a")
来源：http://pnn.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://cec.uphjek.com

[E13] 逐字符遍历
来源：http://iye.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://grz.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sij.nwbrower.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bul.ywan-chungtsiang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dyu.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gbf.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jjy.iojbl.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fhw.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vsv.gzhubu.top

[E14] URL 编码与 Base64
来源：http://bfg.dashuyun.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pku.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://raw.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eht.yanxiufei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tjd.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ria.shanyushiyangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://biv.chenlongwang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xhk.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fzv.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://mye.gotoacloud.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xbx.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ree.yonumen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://duy.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jjm.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rtk.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://awj.pengpengdd.cyou

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hpx.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bvn.ywan-chungtsiang.top

[E16] 数字千分位
来源：http://vyg.pycfn.com

Py:   f"{1234567:,}"
来源：http://whn.xziqi.cn

PHP:  number_format(1234567);
来源：http://eew.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://snk.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zxy.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jqx.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://moz.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ila.ybcxt.top

C#:   1234567.ToString("N0")
来源：http://swl.zdqjudy.top

[E17] 首字母大写
来源：http://vla.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hzj.jinqigufen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hip.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zaw.jinqigufen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fwu.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ylz.andypj.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rft.pycfn.com

Ruby: s.capitalize
来源：http://gzh.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fqy.svipenyu.cn

[E18] 模板占位符替换
来源：http://ykb.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://thb.vqdsnc.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cvc.hcnkem.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ysp.dianchejie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iiy.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dfp.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ily.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aij.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wwn.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://aud.jyoumei.cn

Py:   s.splitlines()
来源：http://enj.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cvh.hnqzz.top

JS:   s.split(/\r?\n/)
来源：http://fib.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://gpc.gotoacloud.top

Java: s.lines().toList()
来源：http://qjx.redwolf501.top

Go:   strings.Split(s, "\n")
来源：http://eem.aizwys.cn

Ruby: s.lines
来源：http://kxp.wangdashe.top

C#:   s.Split('\n')
来源：http://hkt.shzxlz.cn

[E20] 判断字符串是否为空
来源：http://kkp.hnxiangtu.top

Py:   if not s:
来源：http://xil.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wrf.tanke756.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eto.bbcook.cn

TS:   if (s === "") {}
来源：http://ekb.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://axy.52xcode.cn

Go:   if s == "" {}
来源：http://byy.quarkkingdee.top

Ruby: if s.empty?
来源：http://iir.hysaishi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vcs.9152youxi.cn

[E21] 超长截断加省略号
来源：http://adx.yuanzhike.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vir.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dvc.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wkt.yj20258888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ezy.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ahf.feifeiyinyue.top

Go:   // 按 rune 判断长度后截断
来源：http://eux.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dqg.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qcb.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://cjy.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bxe.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fbq.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ocy.mhx1999.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xxv.yj20258888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ghr.meibo888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mfd.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://oxv.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rpa.aibaodan.cn

================================================================================
来源：http://jhy.andypj.xyz

F. 文件与目录
来源：http://pgf.sweek.top

================================================================================
来源：http://rai.svipenyu.cn

[F01] 读取整个文件
来源：http://mxv.xziqi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rlx.jinqigufen.top

PHP:  file_get_contents("a.txt");
来源：http://gru.jinqigfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pjk.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nfn.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jxl.yanxiufei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fut.hammf.cn

Ruby: File.read("a.txt")
来源：http://jyy.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://iqe.zhixingplan.top

[F02] 逐行读取文件
来源：http://bea.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://soc.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cdw.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vof.epnwcf.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rtb.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rgc.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yty.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://klu.jianghu66.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ihb.yanxiufei.cn

[F03] 写入文件（覆盖）
来源：http://ary.zhongyouzk.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xkl.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://fqu.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://flp.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ckj.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tag.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qmk.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://dob.hywenlv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uli.hfpthk.cn

[F04] 追加写入文件
来源：http://xxk.ivvv.top


<!-- 参考信息 -->