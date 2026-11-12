代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://spd.xziqi.cn

Ruby: arr.include?(x)
来源：http://tmx.zhongyouzk.top

C#:   list.Contains(x)
来源：http://fub.hysaishi.cn

[D22] 复制数组（避免共享引用）
来源：http://fdb.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hfl.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://agk.yj202588.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cuy.hywenlv.cn

TS:   [...arr];
来源：http://zpi.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://any.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://xsy.gotoacloud.top

Ruby: arr.dup;  arr.clone
来源：http://hfn.andypj.xyz

C#:   new List<int>(list);
来源：http://jrb.dianchejie.cn

[D23] reduce 累积计算
来源：http://csq.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tik.bbcook.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uqq.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tap.jqgufenzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uza.epnwcf.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://mej.dianchejie.cn

Go:   // 手写循环
来源：http://mzt.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ren.gotoacloud.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yhs.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://vud.kuanghao11.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hbv.aizwys.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rsy.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://psf.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qza.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qjc.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eas.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kri.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yva.zhoulong.xyz

[D25] Set 集合去重与交并差
来源：http://hxj.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://njv.316326.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jaq.yj20258.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://exf.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cdp.jinqigufen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rdb.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gpy.yanxiufei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cix.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jru.hnqzz.top

[D26] 数组转字符串
来源：http://okv.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://ext.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://cwe.gaohongyu789.top

JS:   arr.join(", ")
来源：http://zwx.wangdashe.top

TS:   arr.join(", ")
来源：http://yno.fanxiaobao.xyz

Java: String.join(", ", list)
来源：http://bzv.uphjek.com

Go:   strings.Join(strs, ", ")
来源：http://jne.snrcjt.cn

Ruby: arr.join(", ")
来源：http://lpi.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://mfi.ydjk.org.cn

================================================================================
来源：http://ojb.guowangkeji.top

E. 字符串处理
来源：http://vkm.dianchejie.cn

================================================================================
来源：http://alf.haohaochexian.top

[E01] 拼接字符串
来源：http://mlv.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vxk.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ukv.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tgb.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xeh.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ohq.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rym.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://abk.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lzw.cqqwz.cn

[E02] 重复字符串
来源：http://rxm.nanxinkj.top

Py:   "ab" * 3
来源：http://cgb.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://zox.gzhubu.top

JS:   "ab".repeat(3)
来源：http://eyl.yj20258.top

TS:   "ab".repeat(3)
来源：http://huc.snrcjt.cn

Java: "ab".repeat(3)
来源：http://ytq.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://cqm.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://xfe.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jlo.andypj.xyz

[E03] 截取子串
来源：http://fjf.guannengcc.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tea.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aek.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rqp.hesvh.cn

TS:   s.slice(1, 4)
来源：http://msz.hysaishi.cn

Java: s.substring(1, 4)
来源：http://oaa.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xaf.zycfv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fji.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://kcn.yfazqb.com

[E04] 查找子串位置
来源：http://mgx.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://new.vqdsnc.cn

PHP:  strpos($s, "x");
来源：http://yav.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jgl.birdmap.top

TS:   s.indexOf("x")
来源：http://bof.haohaochexian.top

Java: s.indexOf("x")
来源：http://zis.aizwys.cn

Go:   strings.Index(s, "x")
来源：http://tld.ctjpmb.com

Ruby: s.index("x")
来源：http://jmi.cucudq.cn

C#:   s.IndexOf("x")
来源：http://swf.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://avo.yvedp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://otl.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tar.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dts.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://uvk.vehdjk.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pdn.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://srn.xziqi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ejz.shangyingyoupin.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rdu.chenzaomai.com

[E06] 替换子串
来源：http://mvx.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rrt.bbcook.cn

PHP:  str_replace("a", "b", $s);
来源：http://yje.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qwi.chenlongwang.top

TS:   s.replaceAll("a", "b")
来源：http://ufq.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://usk.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://srl.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kqq.jqgufenzy.top

C#:   s.Replace("a", "b")
来源：http://bgx.wangdashe.top

[E07] 按分隔符拆分
来源：http://nqm.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jwr.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uxv.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://tuc.chenjidiqi.icu

TS:   s.split(",")
来源：http://ffo.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://vwa.52xcode.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uwv.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://fyy.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wpr.cdnleiting.top

[E08] 数组按分隔符合并
来源：http://ici.jlsjyb.cn

Py:   ",".join(items)
来源：http://ytc.snrcjt.cn

PHP:  implode(",", $items);
来源：http://kcl.jinqigfzy.top

JS:   items.join(",")
来源：http://dhs.xziqi.cn

TS:   items.join(",")
来源：http://eue.tian-w.cn

Java: String.join(",", items)
来源：http://fvd.bbcook.cn

Go:   strings.Join(items, ",")
来源：http://yob.hcnkem.com

Ruby: items.join(",")
来源：http://jxj.yangfankeji.com

C#:   string.Join(",", items)
来源：http://oei.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://cem.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ehl.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://prs.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://gpp.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://wip.tianlin.xyz

Java: s.replaceAll("\\s+", "")
来源：http://yxj.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oqn.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://ucs.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pbt.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://roq.tarul.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hnh.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cgv.gzhubu.top

JS:   "7".padStart(3, "0")
来源：http://zpv.yj202588.top

TS:   "7".padStart(3, "0")
来源：http://ttz.shuidangran.top

Java: String.format("%03d", 7)
来源：http://wud.jianghu66.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pxo.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vem.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://psa.xuetiantiany.cn

[E11] 反转字符串
来源：http://vuo.nwbrower.top

Py:   s[::-1]
来源：http://bpj.uphjek.com

PHP:  strrev($s);
来源：http://acw.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://pew.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://tbf.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xdg.tianlin.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ugz.zhijiandao.cn

Ruby: s.reverse
来源：http://ovt.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fer.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://jvf.yj20258888.top

Py:   s.count("a")
来源：http://fba.hnxiangtu.top

PHP:  substr_count($s, "a");
来源：http://uxu.fzhhl.top

JS:   s.split("a").length - 1
来源：http://ldw.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://dpz.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://etz.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://grw.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://unf.smart0.xyz

C#:   s.Count(c => c == 'a')
来源：http://mxe.shzxlz.cn

[E13] 逐字符遍历
来源：http://fdn.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://qqh.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qnq.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yuz.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://onc.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jcj.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zln.daria6918.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pvd.jqgfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://htr.cqqwz.cn

[E14] URL 编码与 Base64
来源：http://frv.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qmm.0kj1m.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yft.zhixingplan.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://png.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://emy.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rtz.havefunace.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ppp.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://byc.zhiwuduotai.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ojc.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://nya.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vhk.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zqx.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ppg.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://coz.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ice.yuxming.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qds.redwolf501.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rfb.quarkkingdee.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wsl.wangdashe.top

[E16] 数字千分位
来源：http://meg.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://nkl.daxiang520.top

PHP:  number_format(1234567);
来源：http://zwk.gogol.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bpi.iojbl.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kua.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://duw.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://noa.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mix.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://xwe.yonumen.top

[E17] 首字母大写
来源：http://wkf.ybcxt.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://epy.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xel.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://umk.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hhz.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pkz.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pal.daria6918.cn

Ruby: s.capitalize
来源：http://ojd.jinqigfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wsn.meibo888.top

[E18] 模板占位符替换
来源：http://itk.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zmy.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://muf.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nyi.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xab.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uiu.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oro.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jvk.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://llb.yonumen.top

[E19] 多行文本按行拆分
来源：http://yos.vqdsnc.cn

Py:   s.splitlines()
来源：http://egn.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://acx.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://bra.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://pxu.andypj.xyz

Java: s.lines().toList()
来源：http://kdj.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://gpb.redwolf501.top

Ruby: s.lines
来源：http://imn.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://kgm.hnqzz.top

[E20] 判断字符串是否为空
来源：http://yuk.fehbvm.com

Py:   if not s:
来源：http://zsf.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zbs.fktsv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zgo.jqgufenzy.top

TS:   if (s === "") {}
来源：http://cjp.tarul.cn

Java: if (s.isEmpty()) {}
来源：http://hag.quarkkingdee.top

Go:   if s == "" {}
来源：http://nhf.jqgfzy.top

Ruby: if s.empty?
来源：http://hoq.cqqwz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sqb.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://krn.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sis.shangyingyoupin.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gju.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xrq.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iul.wangdashe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yqk.iojbl.cn

Go:   // 按 rune 判断长度后截断
来源：http://uuv.jinqigfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://axt.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aoz.yj202588.top

[E22] 字节长度与字符长度
来源：http://exm.xziqi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cgj.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nxw.feifeiyinyue.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yph.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jzz.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jmk.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jcw.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://ugq.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uxg.shanyushiyangkeji.top

================================================================================
来源：http://iiq.nanxuanxn.top

F. 文件与目录
来源：http://ayl.feifeiyinyue.top

================================================================================
来源：http://hkj.xuetiantiany.cn

[F01] 读取整个文件
来源：http://xnd.sxryk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nbe.chenjidiqi.icu

PHP:  file_get_contents("a.txt");
来源：http://zqx.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eec.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sqo.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zzi.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aeq.zhaomingkeji.xyz

Ruby: File.read("a.txt")
来源：http://ovb.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://fbm.chenzaomai.com

[F02] 逐行读取文件
来源：http://hxo.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gfr.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qge.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bik.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pdz.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nkf.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zcc.smart0.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gqf.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wkl.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://dke.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hde.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rkb.fengsongda.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://goz.zycfv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dvo.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ovj.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yrn.zhongyouzk.top

Ruby: File.write("a.txt", "hi")
来源：http://cur.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mkw.guannengcc.top

[F04] 追加写入文件
来源：http://vgt.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wce.smart0.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ulw.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yfn.gogol.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nhk.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hdo.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hrs.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wnw.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pbw.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://yqi.yangfankeji.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mrh.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://qzi.ywan-chungtsiang.top

JS:   fs.existsSync("a.txt")
来源：http://tzu.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://xhn.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://iiy.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fow.gaohongyu789.top

Ruby: File.exist?("a.txt")
来源：http://vhy.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://teu.haohaochexian.top

[F06] 删除文件
来源：http://boc.meibo888.top

Py:   os.remove("a.txt")
来源：http://foh.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://cul.0kj1m.cn


<!-- 参考信息 -->