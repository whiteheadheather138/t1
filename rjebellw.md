代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eyh.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bnf.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://scq.wangshuangyany.cn

TS:   [...arr];
来源：http://uhe.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://vzl.cucudq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cvm.mhx1999.top

Ruby: arr.dup;  arr.clone
来源：http://lbg.aizwys.cn

C#:   new List<int>(list);
来源：http://mii.iojbl.cn

[D23] reduce 累积计算
来源：http://btq.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gwv.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lma.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nhw.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kwg.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xdl.tianlin.xyz

Go:   // 手写循环
来源：http://rch.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://buh.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://swn.sweek.top

[D24] 字典 / Map 基本操作
来源：http://tur.jyoumei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kug.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bmu.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tyh.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fqr.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sul.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pkc.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://poa.gotoacloud.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tyu.ctjpmb.com

[D25] Set 集合去重与交并差
来源：http://kge.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vmz.xingfuxueyuan.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://awk.chenlongwang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qcu.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gjg.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lcg.fanxiaobao.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kkj.shzxlz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://biv.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iep.ehwqpu.com

[D26] 数组转字符串
来源：http://iwe.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://oek.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://kgv.yvedp.cn

JS:   arr.join(", ")
来源：http://emm.hnxiangtu.top

TS:   arr.join(", ")
来源：http://jqh.316326.xyz

Java: String.join(", ", list)
来源：http://hvz.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://tte.ydzc1.top

Ruby: arr.join(", ")
来源：http://xtl.daria6918.cn

C#:   string.Join(", ", list)
来源：http://sgz.zhongyouzk.top

================================================================================
来源：http://vqi.yuanzhike.top

E. 字符串处理
来源：http://lus.yj202588.top

================================================================================
来源：http://kza.xziqi.cn

[E01] 拼接字符串
来源：http://pdk.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rbt.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nhc.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ycr.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iif.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vvn.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nfo.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zwe.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kox.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://ght.uphjek.com

Py:   "ab" * 3
来源：http://eqg.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://ifn.bjfxy.top

JS:   "ab".repeat(3)
来源：http://miq.gotoacloud.top

TS:   "ab".repeat(3)
来源：http://zuv.jianghu66.top

Java: "ab".repeat(3)
来源：http://ycj.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://ikr.sweek.top

Ruby: "ab" * 3
来源：http://wqm.redwolf501.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aaj.hywenlv.cn

[E03] 截取子串
来源：http://dcd.zhaomingkeji.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ite.zhengqikj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ept.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dox.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://kax.jianghu66.top

Java: s.substring(1, 4)
来源：http://gpn.cheryme.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lee.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://xht.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://qxz.hammf.cn

[E04] 查找子串位置
来源：http://qbk.hesvh.cn

Py:   s.find("x");  s.index("x")
来源：http://qtb.hammf.cn

PHP:  strpos($s, "x");
来源：http://day.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nbz.ydjk.org.cn

TS:   s.indexOf("x")
来源：http://gdt.hcnkem.com

Java: s.indexOf("x")
来源：http://ujq.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://wxq.yvedp.cn

Ruby: s.index("x")
来源：http://izj.fengsongda.top

C#:   s.IndexOf("x")
来源：http://nlw.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rps.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ozc.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lqs.ctjpmb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zri.meibo888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tks.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lld.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yct.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ubi.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ofj.snrcjt.cn

[E06] 替换子串
来源：http://dbw.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aky.daria6918.cn

PHP:  str_replace("a", "b", $s);
来源：http://upz.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zmt.xinyue.icu

TS:   s.replaceAll("a", "b")
来源：http://pbk.daxiang520.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fpp.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zci.jinghuilouyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dge.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://fnn.cdnleiting.top

[E07] 按分隔符拆分
来源：http://nek.ppjwa.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://run.guowangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hgy.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zkq.sysykeji.top

TS:   s.split(",")
来源：http://xcr.cucudq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ztf.chenlongwang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kwk.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://rdm.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mxn.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://bac.cheryme.top

Py:   ",".join(items)
来源：http://lau.zhijiandao.cn

PHP:  implode(",", $items);
来源：http://ive.mhx1999.top

JS:   items.join(",")
来源：http://hhj.bjfxy.top

TS:   items.join(",")
来源：http://dvr.wangdashe.top

Java: String.join(",", items)
来源：http://mwt.c1oappe.top

Go:   strings.Join(items, ",")
来源：http://dio.fengsongda.top

Ruby: items.join(",")
来源：http://kaj.hcnkem.com

C#:   string.Join(",", items)
来源：http://cjz.nanxinkj.top

[E09] 去除所有空白字符
来源：http://eyc.jinyuanbaomall.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://man.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://apb.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://got.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://xrq.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://ntw.aibaodan.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cfk.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://mqc.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xwg.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://emu.yuxming.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jht.wangdashe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rcz.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://uey.shuidangran.top

TS:   "7".padStart(3, "0")
来源：http://tbe.yueranfly.top

Java: String.format("%03d", 7)
来源：http://wzm.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zmc.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yib.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dmo.hywenlv.cn

[E11] 反转字符串
来源：http://zqs.9152youxi.cn

Py:   s[::-1]
来源：http://ato.aibaodan.cn

PHP:  strrev($s);
来源：http://byx.pycfn.com

JS:   [...s].reverse().join("")
来源：http://tyx.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://qzo.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bis.epnwcf.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://bwf.jinqigfzy.top

Ruby: s.reverse
来源：http://oro.hnqzz.top

C#:   new string(s.Reverse().ToArray())
来源：http://xmw.guannengcc.top

[E12] 统计某字符出现次数
来源：http://xck.yongpay.top

Py:   s.count("a")
来源：http://wbt.yj20258.top

PHP:  substr_count($s, "a");
来源：http://ruv.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://dmr.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://lxq.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://naa.shzxlz.cn

Go:   strings.Count(s, "a")
来源：http://kge.yj20258.top

Ruby: s.count("a")
来源：http://sqv.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://xtp.shzxlz.cn

[E13] 逐字符遍历
来源：http://rge.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://qcw.fanxiaobao.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bmr.yueranfly.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tqy.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rfo.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lsx.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mkv.jlsjyb.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gij.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ssk.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://len.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jao.wangshuangyany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fnm.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hgr.xuetiantiany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tmd.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tuu.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cai.ywan-chungtsiang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dfo.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aef.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://cck.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sbf.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nhs.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rtr.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hsu.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://had.vehdjk.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://chz.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nnr.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cde.jlsjyb.cn

[E16] 数字千分位
来源：http://lzm.ydjk.org.cn

Py:   f"{1234567:,}"
来源：http://qwa.vehdjk.com

PHP:  number_format(1234567);
来源：http://vxc.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bzl.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://kkd.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jaz.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://afs.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vyk.uphjek.com

C#:   1234567.ToString("N0")
来源：http://rfr.ywan-chungtsiang.top

[E17] 首字母大写
来源：http://ycs.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://klb.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://maz.xylfe.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qmo.smart0.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xwi.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nmh.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wso.hesvh.cn

Ruby: s.capitalize
来源：http://xkj.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lsn.9152youxi.cn

[E18] 模板占位符替换
来源：http://csv.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://frf.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://snu.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://efq.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://joo.wangdashe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nfu.fzhhl.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jza.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hll.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bto.jqgufenzy.top

[E19] 多行文本按行拆分
来源：http://tmv.yueranfly.top

Py:   s.splitlines()
来源：http://ngk.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fuz.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://czr.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://spt.gaohongyu789.top

Java: s.lines().toList()
来源：http://qhk.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://smx.shanyushiyangkeji.top

Ruby: s.lines
来源：http://scb.hammf.cn

C#:   s.Split('\n')
来源：http://glz.cucudq.cn

[E20] 判断字符串是否为空
来源：http://qpo.yueranfly.top

Py:   if not s:
来源：http://ldi.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ddi.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qkp.52xcode.cn

TS:   if (s === "") {}
来源：http://iel.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://iks.sxryk.cn

Go:   if s == "" {}
来源：http://fft.ehwqpu.com

Ruby: if s.empty?
来源：http://ibv.zhoulong.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ypl.nwbrower.top

[E21] 超长截断加省略号
来源：http://hto.hongshengwenyu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nek.zhoulong.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aob.guannengcc.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fkk.wangshuangyany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wkp.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gdl.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://pqf.yongpay.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wjo.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oam.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://epm.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rrw.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://znl.hammf.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://egq.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wjd.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eyj.shangyingyoupin.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sqe.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://zih.xylfe.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zyw.hywenlv.cn

================================================================================
来源：http://rmj.xylfe.cn

F. 文件与目录
来源：http://vjk.kuanghao11.cn

================================================================================
来源：http://fwm.yangfankeji.com

[F01] 读取整个文件
来源：http://qnp.xingfuxueyuan.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jch.ydjk.org.cn

PHP:  file_get_contents("a.txt");
来源：http://ska.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cgk.hesvh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hlx.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bum.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qnh.fanxiaobao.xyz

Ruby: File.read("a.txt")
来源：http://wda.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://zwt.uphjek.com

[F02] 逐行读取文件
来源：http://yap.yj20258888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xhr.sxryk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://une.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ulq.hywenlv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hbs.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://odr.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://whk.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://llk.svipenyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hhc.ydjk.org.cn

[F03] 写入文件（覆盖）
来源：http://jpj.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hmu.bbcook.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://olx.andypj.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://saw.guannengcc.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cxr.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uog.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://luk.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://sqk.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oqj.jinqigfzy.top

[F04] 追加写入文件
来源：http://diy.ehwqpu.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dfn.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bjj.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qlx.ybcxt.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mka.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lbf.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mcu.xingfuxueyuan.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ihk.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://twb.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://jof.daria6918.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mcg.ydjk.org.cn

PHP:  file_exists("a.txt");
来源：http://woz.daxiang520.top

JS:   fs.existsSync("a.txt")
来源：http://pww.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://oto.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://acj.mhx1999.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://osp.xingfuxueyuan.xyz

Ruby: File.exist?("a.txt")
来源：http://lak.redwolf501.top

C#:   File.Exists("a.txt")
来源：http://zuj.svipenyu.cn

[F06] 删除文件
来源：http://zpr.xingfuxueyuan.xyz

Py:   os.remove("a.txt")
来源：http://eae.gzhubu.top

PHP:  unlink("a.txt");
来源：http://for.yuxming.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dbb.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bgm.iojbl.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fyu.daria6918.cn

Go:   os.Remove("a.txt")
来源：http://xtx.pengpengdd.cyou


<!-- 参考信息 -->