代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bpd.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dlf.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ohx.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://vqc.yj20258888.top

Ruby: arr.tally
来源：http://tqo.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qyw.yueranfly.top

[D21] 判断是否包含某元素
来源：http://qlj.chenjidiqi.icu

Py:   x in arr
来源：http://luv.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://zla.yuanzhike.top

JS:   arr.includes(x)
来源：http://ewp.nwbrower.top

TS:   arr.includes(x)
来源：http://ywd.haohaochexian.top

Java: list.contains(x)
来源：http://zfd.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://mvs.hywenlv.cn

Ruby: arr.include?(x)
来源：http://qot.fehbvm.com

C#:   list.Contains(x)
来源：http://klk.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://ekj.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://erm.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://irm.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hyy.dianchejie.cn

TS:   [...arr];
来源：http://vxj.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://wuq.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qbt.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://xqx.svipenyu.cn

C#:   new List<int>(list);
来源：http://swa.316326.xyz

[D23] reduce 累积计算
来源：http://zhu.shuidangran.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://abr.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xmh.hfpthk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://reg.hesvh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jxl.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ofa.hcnkem.com

Go:   // 手写循环
来源：http://jmd.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ncu.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vwn.birdmap.top

[D24] 字典 / Map 基本操作
来源：http://oxh.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gep.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ljc.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ejh.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zwz.ivvv.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fpb.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://muo.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qqa.haohaochexian.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sal.ehwqpu.com

[D25] Set 集合去重与交并差
来源：http://qhj.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hqj.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xap.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cdq.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fla.yj20258.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://euf.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://opa.guannengcc.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xut.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qrw.zhixingplan.top

[D26] 数组转字符串
来源：http://mxi.yongpay.top

Py:   ", ".join(map(str, arr))
来源：http://ven.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://ibo.ehwqpu.com

JS:   arr.join(", ")
来源：http://feg.nanxinkj.top

TS:   arr.join(", ")
来源：http://sfx.cqqwz.cn

Java: String.join(", ", list)
来源：http://ikz.ydjk.org.cn

Go:   strings.Join(strs, ", ")
来源：http://cqv.xuanzx.com

Ruby: arr.join(", ")
来源：http://mra.zhiwuduotai.top

C#:   string.Join(", ", list)
来源：http://bvh.cdnleiting.top

================================================================================
来源：http://msh.xinyue.icu

E. 字符串处理
来源：http://xty.meibo888.top

================================================================================
来源：http://wqk.yvedp.cn

[E01] 拼接字符串
来源：http://rrg.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://opk.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yol.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://typ.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dst.fehbvm.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wkr.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zae.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://azn.yj20258.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bde.sweek.top

[E02] 重复字符串
来源：http://ciq.jinqigufen.top

Py:   "ab" * 3
来源：http://for.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://kbi.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://ztm.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://opd.wangdashe.top

Java: "ab".repeat(3)
来源：http://xjo.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://dib.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://xsr.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://igo.ppjwa.cn

[E03] 截取子串
来源：http://ztz.tarul.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nkl.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ole.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bip.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://lda.xziqi.cn

Java: s.substring(1, 4)
来源：http://mtb.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jny.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://lhe.redwolf501.top

C#:   s.Substring(1, 3)
来源：http://nrn.tarul.cn

[E04] 查找子串位置
来源：http://cmp.smart0.xyz

Py:   s.find("x");  s.index("x")
来源：http://qkc.yj202588.top

PHP:  strpos($s, "x");
来源：http://isz.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xfa.xinyue.icu

TS:   s.indexOf("x")
来源：http://vjz.meibo888.top

Java: s.indexOf("x")
来源：http://eth.gotoacloud.top

Go:   strings.Index(s, "x")
来源：http://qml.hywenlv.cn

Ruby: s.index("x")
来源：http://zvl.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://ntq.haohaochexian.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pzz.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aeg.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sll.jlsjyb.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ecx.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dpt.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jhk.yangfankeji.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dgd.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cgo.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mcr.cucudq.cn

[E06] 替换子串
来源：http://wet.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oic.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://zra.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wvo.snrcjt.cn

TS:   s.replaceAll("a", "b")
来源：http://fhe.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://elm.ppjwa.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jic.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zgo.redwolf501.top

C#:   s.Replace("a", "b")
来源：http://luy.meibo888.top

[E07] 按分隔符拆分
来源：http://lov.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kxk.jinyuanbaomall.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jdl.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://etq.jiagoushi.top

TS:   s.split(",")
来源：http://eeh.bbcook.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yhy.zycfv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jnw.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://rqx.guowangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kjk.fzhhl.top

[E08] 数组按分隔符合并
来源：http://zjs.ydzc1.top

Py:   ",".join(items)
来源：http://xaz.hysaishi.cn

PHP:  implode(",", $items);
来源：http://jvv.hfpthk.cn

JS:   items.join(",")
来源：http://qqf.dashuyun.cn

TS:   items.join(",")
来源：http://txb.gogol.net.cn

Java: String.join(",", items)
来源：http://hol.xinyue.icu

Go:   strings.Join(items, ",")
来源：http://bgb.quarkkingdee.top

Ruby: items.join(",")
来源：http://wpq.9152youxi.cn

C#:   string.Join(",", items)
来源：http://hbi.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://bxi.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lpw.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ttf.tianlin.xyz

JS:   s.replace(/\s+/g, "")
来源：http://nys.zycfv.cn

TS:   s.replace(/\s+/g, "")
来源：http://fgi.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://flz.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wrw.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ygm.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uvd.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://dpp.snrcjt.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hue.jianghu66.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vzx.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://kpl.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://myb.sweek.top

Java: String.format("%03d", 7)
来源：http://yqf.yj20258.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ilo.cucudq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ymf.meibo888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xzf.316326.xyz

[E11] 反转字符串
来源：http://yuf.iojbl.cn

Py:   s[::-1]
来源：http://cbf.epnwcf.com

PHP:  strrev($s);
来源：http://tol.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://aej.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://ocs.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lix.epnwcf.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://hqu.hesvh.cn

Ruby: s.reverse
来源：http://fpo.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qkv.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://jph.bjfxy.top

Py:   s.count("a")
来源：http://lan.0kj1m.cn

PHP:  substr_count($s, "a");
来源：http://fiy.fktsv.cn

JS:   s.split("a").length - 1
来源：http://ynn.316326.xyz

TS:   s.split("a").length - 1
来源：http://vae.jqgfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kln.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://wnk.zhixingplan.top

Ruby: s.count("a")
来源：http://gkg.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://khm.jinyuanbaomall.cn

[E13] 逐字符遍历
来源：http://dnr.sufxvd.cn

Py:   for ch in s: print(ch)
来源：http://exl.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://edp.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zzx.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://kaf.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wgx.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jzq.chenjidiqi.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://txi.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kyo.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://fvs.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aon.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vkr.hammf.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://utz.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gdx.bbcook.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://edv.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gos.hcnkem.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rvp.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kzu.yfazqb.com

[E15] HTML 转义 / 反转义
来源：http://gfv.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://oqo.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hfb.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ylb.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://twc.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://teu.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dpt.guowangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qlv.vehdjk.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zyh.0kj1m.cn

[E16] 数字千分位
来源：http://gfg.tanke756.top

Py:   f"{1234567:,}"
来源：http://wmf.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://uot.dashuyun.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zyz.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lxp.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://smr.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qgd.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rxx.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://wuf.chenlongwang.top

[E17] 首字母大写
来源：http://efl.52xcode.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://beq.jinqigufen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dbd.daria6918.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fwz.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://llz.wangshuangyany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iqb.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://alp.zhixingplan.top

Ruby: s.capitalize
来源：http://wvk.zhengqikj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gvw.tarul.cn

[E18] 模板占位符替换
来源：http://axf.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://owf.ydjk.org.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vdg.hnxiangtu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://teu.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vrx.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xof.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dvz.yuxming.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vxm.9152youxi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fgy.hammf.cn

[E19] 多行文本按行拆分
来源：http://niu.mhx1999.top

Py:   s.splitlines()
来源：http://jhf.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pgv.yanxiufei.cn

JS:   s.split(/\r?\n/)
来源：http://kgi.yangfankeji.com

TS:   s.split(/\r?\n/)
来源：http://vwy.andypj.xyz

Java: s.lines().toList()
来源：http://oxw.yfazqb.com

Go:   strings.Split(s, "\n")
来源：http://rrn.mhx1999.top

Ruby: s.lines
来源：http://dsu.zhoulong.xyz

C#:   s.Split('\n')
来源：http://tul.uphjek.com

[E20] 判断字符串是否为空
来源：http://vit.fktsv.cn

Py:   if not s:
来源：http://zdb.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://woq.shangyingyoupin.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gdn.iojbl.cn

TS:   if (s === "") {}
来源：http://wro.jqgfzy.top

Java: if (s.isEmpty()) {}
来源：http://ioh.cqqwz.cn

Go:   if s == "" {}
来源：http://tcm.hysaishi.cn

Ruby: if s.empty?
来源：http://vsj.chenzaomai.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gip.c1oappe.top

[E21] 超长截断加省略号
来源：http://cso.c1oappe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rew.xinyue.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://elp.tianlin.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fmh.kuanghao11.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tzk.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qox.zhengqikj.top

Go:   // 按 rune 判断长度后截断
来源：http://ter.sjlbkw.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hsg.ivvv.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vev.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://sea.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://him.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bmk.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://plp.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cnq.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qwo.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://moz.zdbjq.cn

Ruby: s.bytesize;  s.length
来源：http://ovp.hysaishi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gdv.xingfuxueyuan.xyz

================================================================================
来源：http://nuu.zhongyouzk.top

F. 文件与目录
来源：http://xha.hesvh.cn

================================================================================
来源：http://juf.nanxuanxn.top

[F01] 读取整个文件
来源：http://bcl.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bzu.chenlongwang.top

PHP:  file_get_contents("a.txt");
来源：http://mtx.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sqs.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vjg.cdnleiting.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wnl.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jrv.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://xsy.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://gml.havefunace.top

[F02] 逐行读取文件
来源：http://kjn.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rta.zhengqikj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tkl.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qea.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bfn.jinqigfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qaw.gaohongyu789.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://etz.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://urb.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hfp.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://inm.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://egn.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pwp.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gvx.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qjb.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zwf.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kff.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://lrq.9152youxi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://klc.vqdsnc.cn

[F04] 追加写入文件
来源：http://vsq.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cng.yongpay.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://odf.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ltk.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qqi.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xcb.cqqwz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qlf.guannengcc.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vdt.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wzz.gaohongyu789.top


<!-- 参考信息 -->