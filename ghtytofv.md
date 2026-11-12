代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gyw.yonumen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://erl.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://abt.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://gso.zdbjq.cn

Ruby: arr.tally
来源：http://bmc.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ugo.epnwcf.com

[D21] 判断是否包含某元素
来源：http://tzw.chenzaomai.com

Py:   x in arr
来源：http://szh.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://ixs.yvedp.cn

JS:   arr.includes(x)
来源：http://dgq.guowangkeji.top

TS:   arr.includes(x)
来源：http://ffi.gzhubu.top

Java: list.contains(x)
来源：http://qbp.xingfuxueyuan.xyz

Go:   slices.Contains(arr, x)
来源：http://sjt.cucudq.cn

Ruby: arr.include?(x)
来源：http://zso.yueranfly.top

C#:   list.Contains(x)
来源：http://cwh.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://rjv.jianghu66.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://psp.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qiw.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://now.zhixingplan.top

TS:   [...arr];
来源：http://gwq.jinqigfzy.top

Java: new ArrayList<>(list);
来源：http://nur.sysykeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://ojv.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://osf.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://hib.jiagoushi.top

[D23] reduce 累积计算
来源：http://zds.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://idh.yj20258.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eie.316326.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zmp.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mhv.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nqm.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://qew.nanxinkj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ujr.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tws.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://qkm.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ijy.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aps.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zvk.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vik.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qyf.yuxming.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://brx.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tbw.yueranfly.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ham.pycfn.com

[D25] Set 集合去重与交并差
来源：http://mjn.jlsjyb.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qpm.cqqwz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ktc.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hzu.hysaishi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://svt.yfazqb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zoj.sweek.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tcc.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fnd.shanyushiyangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://moz.vqdsnc.cn

[D26] 数组转字符串
来源：http://axb.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://jzx.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://tba.ppjwa.cn

JS:   arr.join(", ")
来源：http://zkd.bjfxy.top

TS:   arr.join(", ")
来源：http://ixp.iojbl.cn

Java: String.join(", ", list)
来源：http://fwq.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://tva.sxryk.cn

Ruby: arr.join(", ")
来源：http://qfr.smart0.xyz

C#:   string.Join(", ", list)
来源：http://mir.hammf.cn

================================================================================
来源：http://wxp.ybcxt.top

E. 字符串处理
来源：http://ucd.yj20258888.top

================================================================================
来源：http://amx.cucudq.cn

[E01] 拼接字符串
来源：http://yea.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://awg.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xtp.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bil.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://soo.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oml.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fzd.guannengcc.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ggs.quarkkingdee.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xji.yuanzhike.top

[E02] 重复字符串
来源：http://riu.sufxvd.cn

Py:   "ab" * 3
来源：http://cuv.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://uuu.yj20258.top

JS:   "ab".repeat(3)
来源：http://pwt.jinqigfzy.top

TS:   "ab".repeat(3)
来源：http://hgl.jyoumei.cn

Java: "ab".repeat(3)
来源：http://jaf.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://jwz.yfazqb.com

Ruby: "ab" * 3
来源：http://mlr.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pfx.bbcook.cn

[E03] 截取子串
来源：http://jtu.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ukv.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iup.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mds.jinqigufen.top

TS:   s.slice(1, 4)
来源：http://jxr.ybcxt.top

Java: s.substring(1, 4)
来源：http://ows.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kwa.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nsj.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://mhr.snrcjt.cn

[E04] 查找子串位置
来源：http://dhe.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://lic.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://eyx.cucudq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yxp.shzxlz.cn

TS:   s.indexOf("x")
来源：http://cwy.zhijiandao.cn

Java: s.indexOf("x")
来源：http://cin.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://for.zhongyouzk.top

Ruby: s.index("x")
来源：http://wfk.pycfn.com

C#:   s.IndexOf("x")
来源：http://tpk.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://erp.zycfv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jfs.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hoo.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fod.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://txj.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lxb.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xge.hcnkem.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zub.xuetiantiany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://twh.yfazqb.com

[E06] 替换子串
来源：http://sfb.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ayg.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://vni.shanyushiyangtech.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://odh.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://yyd.gzhubu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://akn.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bzl.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cyk.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://ehq.smart0.xyz

[E07] 按分隔符拆分
来源：http://vgc.hysaishi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mah.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yzj.gotoacloud.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rpc.cdnleiting.top

TS:   s.split(",")
来源：http://yer.dianchejie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hjt.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sze.hcnkem.com

Ruby: s.split(",");  s.split
来源：http://cxw.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ads.0kj1m.cn

[E08] 数组按分隔符合并
来源：http://wbj.jianghu66.top

Py:   ",".join(items)
来源：http://jlb.hfpthk.cn

PHP:  implode(",", $items);
来源：http://olf.zhijiandao.cn

JS:   items.join(",")
来源：http://bnj.shuidangran.top

TS:   items.join(",")
来源：http://was.hnxiangtu.top

Java: String.join(",", items)
来源：http://qaz.wangshuangyany.cn

Go:   strings.Join(items, ",")
来源：http://jmu.yongpay.top

Ruby: items.join(",")
来源：http://fry.cucudq.cn

C#:   string.Join(",", items)
来源：http://pdt.gogol.net.cn

[E09] 去除所有空白字符
来源：http://jqo.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ftn.sjlbkw.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qck.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://ppj.yvedp.cn

TS:   s.replace(/\s+/g, "")
来源：http://tzu.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://krh.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lfc.sufxvd.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fpt.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://svj.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://smj.bbcook.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bha.fktsv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iqc.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://fbu.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://sjt.zycfv.cn

Java: String.format("%03d", 7)
来源：http://xqe.pycfn.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ifa.xuetiantiany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mrj.yj20258.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ufr.zhengqikj.top

[E11] 反转字符串
来源：http://irf.feifeiyinyue.top

Py:   s[::-1]
来源：http://cja.zhixingplan.top

PHP:  strrev($s);
来源：http://kja.ivvv.top

JS:   [...s].reverse().join("")
来源：http://mqc.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://qdr.cashguo.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ezp.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://aae.aibaodan.cn

Ruby: s.reverse
来源：http://jzg.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vfs.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://hfl.tianlin.xyz

Py:   s.count("a")
来源：http://wzn.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://wrw.yj20258.top

JS:   s.split("a").length - 1
来源：http://fez.tarul.cn

TS:   s.split("a").length - 1
来源：http://xji.hfpthk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bjo.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://clc.hnqzz.top

Ruby: s.count("a")
来源：http://jje.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://hhm.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://pnx.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://twu.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jfa.cheryme.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uaa.yj20258.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oou.zhixingplan.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qpz.fehbvm.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bnr.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xcs.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rpm.redwolf501.top

[E14] URL 编码与 Base64
来源：http://qml.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yqq.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rvy.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lxz.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://khr.zhijiandao.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nga.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nuc.hammf.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cib.zdbjq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://imc.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://day.ehwqpu.com

Py:   html.escape(s);  html.unescape(s)
来源：http://mdh.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sgq.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://awr.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://htf.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iut.zhiwuduotai.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uhm.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ebm.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fgw.cashguo.top

[E16] 数字千分位
来源：http://ndd.ppjwa.cn

Py:   f"{1234567:,}"
来源：http://hyk.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://ynm.yj20258888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gwu.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mhd.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fqn.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aeh.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://prr.yangfankeji.com

C#:   1234567.ToString("N0")
来源：http://prw.gotoacloud.top

[E17] 首字母大写
来源：http://vil.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bzb.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zou.yvedp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hnj.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oyi.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ofo.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qbn.aibaodan.cn

Ruby: s.capitalize
来源：http://ruz.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ztl.vqdsnc.cn

[E18] 模板占位符替换
来源：http://hoz.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dsl.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mqr.jianghu66.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gwv.yvedp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ncr.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tlo.jqgfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mhr.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://swm.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eat.havefunace.top

[E19] 多行文本按行拆分
来源：http://zfg.xinyue.icu

Py:   s.splitlines()
来源：http://ugl.daxiang520.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zch.zhijiandao.cn

JS:   s.split(/\r?\n/)
来源：http://bux.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://stz.ppjwa.cn

Java: s.lines().toList()
来源：http://izx.jqgfzy.top

Go:   strings.Split(s, "\n")
来源：http://moa.bjfxy.top

Ruby: s.lines
来源：http://nvv.yongpay.top

C#:   s.Split('\n')
来源：http://ath.hammf.cn

[E20] 判断字符串是否为空
来源：http://meh.hysaishi.cn

Py:   if not s:
来源：http://btl.wangdashe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nuo.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://evn.hfpthk.cn

TS:   if (s === "") {}
来源：http://wfd.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://gac.c1oappe.top

Go:   if s == "" {}
来源：http://zqp.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://kly.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://znj.52xcode.cn

[E21] 超长截断加省略号
来源：http://xle.hnxiangtu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tkb.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lcp.haohaochexian.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qbe.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blx.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rbb.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://abn.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wgz.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dks.yueranfly.top

[E22] 字节长度与字符长度
来源：http://iwz.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jrj.guannengcc.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dzw.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hou.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xqp.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yaa.redwolf501.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gtd.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://mdt.hysaishi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gkm.tianlin.xyz

================================================================================
来源：http://cmj.jianghu66.top

F. 文件与目录
来源：http://lqm.zhixingplan.top

================================================================================
来源：http://zqy.tarul.cn

[F01] 读取整个文件
来源：http://rfo.gotoacloud.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kwj.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://hkx.yvedp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jhl.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bap.gaohongyu789.top

Java: Files.readString(Path.of("a.txt"))
来源：http://seh.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zht.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://nlp.fengsongda.top

C#:   File.ReadAllText("a.txt");
来源：http://whn.haohaochexian.top

[F02] 逐行读取文件
来源：http://slw.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qaa.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://atu.fanxiaobao.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tbb.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zla.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qsf.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ejl.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hqt.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://que.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://nzf.hongshengwenyu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uvi.mhx1999.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dia.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fyc.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://csw.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://btr.daria6918.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tiu.zdqjudy.top

Ruby: File.write("a.txt", "hi")
来源：http://crj.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vct.zhengqikj.top

[F04] 追加写入文件
来源：http://cqe.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rrj.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wwv.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qxq.xuetiantiany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pru.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vrj.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dle.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uai.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://brf.cashguo.top


<!-- 参考信息 -->