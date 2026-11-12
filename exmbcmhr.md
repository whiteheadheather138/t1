代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://ujt.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fgd.0kj1m.cn

Go:   // 手写 map[string][]T
来源：http://mdm.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uhd.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oae.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://wmd.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://ylq.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://bvt.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fvw.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zck.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://epb.xylfe.cn

Go:   // 手写 map[T]int
来源：http://tfx.tian-w.cn

Ruby: arr.tally
来源：http://nlz.chenjidiqi.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gtn.mhx1999.top

[D21] 判断是否包含某元素
来源：http://avs.ybcxt.top

Py:   x in arr
来源：http://yhd.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://mlv.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://akk.hnxiangtu.top

TS:   arr.includes(x)
来源：http://uhe.birdmap.top

Java: list.contains(x)
来源：http://vwe.xuetiantiany.cn

Go:   slices.Contains(arr, x)
来源：http://wex.yj20258.top

Ruby: arr.include?(x)
来源：http://jba.aizwys.cn

C#:   list.Contains(x)
来源：http://niu.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://rbm.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://klz.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cpd.pengpengdd.cyou

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dfq.yueranfly.top

TS:   [...arr];
来源：http://qqc.nanxuanxn.top

Java: new ArrayList<>(list);
来源：http://vmt.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://ayi.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://gmc.gogol.net.cn

C#:   new List<int>(list);
来源：http://xyz.gzhubu.top

[D23] reduce 累积计算
来源：http://rqu.sweek.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hwx.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://udi.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://spe.yvedp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tnd.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wwu.gogol.net.cn

Go:   // 手写循环
来源：http://vlv.epnwcf.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://njf.ctjpmb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sdv.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://dtn.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mnh.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tqb.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cep.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lyu.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://txa.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bvy.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xwq.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xkf.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://zqt.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mky.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iru.hcnkem.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wsy.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bvo.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uxp.ybcxt.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uyu.xuanzx.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qlv.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dne.0kj1m.cn

[D26] 数组转字符串
来源：http://xxy.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://tir.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://xur.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://ucw.jinqigufen.top

TS:   arr.join(", ")
来源：http://ejt.sxryk.cn

Java: String.join(", ", list)
来源：http://bmi.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://qqf.zycfv.cn

Ruby: arr.join(", ")
来源：http://gyq.jianghu66.top

C#:   string.Join(", ", list)
来源：http://qxj.snrcjt.cn

================================================================================
来源：http://bfg.hammf.cn

E. 字符串处理
来源：http://ufu.shangyingyoupin.top

================================================================================
来源：http://hli.yj20258888.top

[E01] 拼接字符串
来源：http://exy.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://esr.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pye.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wkb.xuanzx.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gmb.ivvv.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zcm.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pug.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wqr.bbcook.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gcc.sysykeji.top

[E02] 重复字符串
来源：http://iat.svipenyu.cn

Py:   "ab" * 3
来源：http://onj.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://xna.jqgfzy.top

JS:   "ab".repeat(3)
来源：http://wkz.zhongyouzk.top

TS:   "ab".repeat(3)
来源：http://ltx.sxryk.cn

Java: "ab".repeat(3)
来源：http://nhz.yj20258888.top

Go:   strings.Repeat("ab", 3)
来源：http://xwt.jinqigufen.top

Ruby: "ab" * 3
来源：http://tnz.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mys.jinyuanbaomall.cn

[E03] 截取子串
来源：http://qjd.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xgi.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pke.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jik.hcnkem.com

TS:   s.slice(1, 4)
来源：http://izu.sysykeji.top

Java: s.substring(1, 4)
来源：http://nhs.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vne.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://ltu.xuetiantiany.cn

C#:   s.Substring(1, 3)
来源：http://wck.jyoumei.cn

[E04] 查找子串位置
来源：http://sfy.gotoacloud.top

Py:   s.find("x");  s.index("x")
来源：http://fby.zhixingplan.top

PHP:  strpos($s, "x");
来源：http://szb.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xrh.wangdashe.top

TS:   s.indexOf("x")
来源：http://caa.52xcode.cn

Java: s.indexOf("x")
来源：http://jgk.jlsjyb.cn

Go:   strings.Index(s, "x")
来源：http://hde.yongpay.top

Ruby: s.index("x")
来源：http://bvh.xylfe.cn

C#:   s.IndexOf("x")
来源：http://vvi.pycfn.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://yok.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hue.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vwt.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iow.shuidangran.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vpc.cheryme.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vqx.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dwg.hesvh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vzu.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://luv.xuetiantiany.cn

[E06] 替换子串
来源：http://tvj.bjfxy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kyl.shangyingyoupin.top

PHP:  str_replace("a", "b", $s);
来源：http://rih.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uup.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://zpj.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uwv.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ord.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pof.chenzaomai.com

C#:   s.Replace("a", "b")
来源：http://dhw.zdbjq.cn

[E07] 按分隔符拆分
来源：http://tmr.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qjz.cdnleiting.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pkn.tanke756.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ged.redwolf501.top

TS:   s.split(",")
来源：http://kas.jinghuilouyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oru.jinqigfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://myi.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://ahu.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ltt.yfazqb.com

[E08] 数组按分隔符合并
来源：http://rgh.hesvh.cn

Py:   ",".join(items)
来源：http://xtr.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://rtv.iojbl.cn

JS:   items.join(",")
来源：http://xsp.gotoacloud.top

TS:   items.join(",")
来源：http://ecs.yongpay.top

Java: String.join(",", items)
来源：http://ahp.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://mgb.zhengqikj.top

Ruby: items.join(",")
来源：http://akv.yj202588.top

C#:   string.Join(",", items)
来源：http://rfo.shuidangran.top

[E09] 去除所有空白字符
来源：http://oyh.ivvv.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tue.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hke.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://pow.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://ogk.yuxming.cn

Java: s.replaceAll("\\s+", "")
来源：http://ehi.sweek.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kwf.zhengqikj.top

Ruby: s.gsub(/\s+/, "")
来源：http://wdf.guannengcc.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fll.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://nqe.shanyushiyangtech.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lkw.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vut.zycfv.cn

JS:   "7".padStart(3, "0")
来源：http://ain.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://gwx.yonumen.top

Java: String.format("%03d", 7)
来源：http://onr.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tck.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eny.yvedp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://emt.fktsv.cn

[E11] 反转字符串
来源：http://icy.nwbrower.top

Py:   s[::-1]
来源：http://gxh.shuidangran.top

PHP:  strrev($s);
来源：http://oxe.dashuyun.cn

JS:   [...s].reverse().join("")
来源：http://wkg.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://bwo.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sxy.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://lon.zhaomingkeji.xyz

Ruby: s.reverse
来源：http://utn.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://uhc.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://nqj.hammf.cn

Py:   s.count("a")
来源：http://tkk.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://ycj.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://zhf.yvedp.cn

TS:   s.split("a").length - 1
来源：http://kov.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://itl.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://pgg.cashguo.top

Ruby: s.count("a")
来源：http://vrn.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://qjw.cqqwz.cn

[E13] 逐字符遍历
来源：http://xln.vqdsnc.cn

Py:   for ch in s: print(ch)
来源：http://ihp.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sfj.sweek.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bqk.ywan-chungtsiang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zhr.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wcb.ywan-chungtsiang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rjj.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://exr.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rnb.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://lgp.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mbm.xziqi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jgg.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eyl.yanxiufei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uyu.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kfn.vehdjk.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zoo.chenjidiqi.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gjg.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cqy.kuanghao11.cn

[E15] HTML 转义 / 反转义
来源：http://tcx.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://lnm.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kon.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yty.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ckd.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fmd.guowangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gzv.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ngh.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://onx.jinqigufen.top

[E16] 数字千分位
来源：http://xpu.snrcjt.cn

Py:   f"{1234567:,}"
来源：http://pyi.zhijiandao.cn

PHP:  number_format(1234567);
来源：http://bcm.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://jwo.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://sit.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ome.aizwys.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nno.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vsv.uphjek.com

C#:   1234567.ToString("N0")
来源：http://jwb.gotoacloud.top

[E17] 首字母大写
来源：http://utu.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bxd.hesvh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qty.cqqwz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lvl.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ssf.sysykeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kia.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bkm.chenlongwang.top

Ruby: s.capitalize
来源：http://htm.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hna.snrcjt.cn

[E18] 模板占位符替换
来源：http://hjz.dianchejie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bgj.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pes.tian-w.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://moa.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://qcz.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sfu.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yog.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cld.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qhw.epnwcf.com

[E19] 多行文本按行拆分
来源：http://gfp.yueranfly.top

Py:   s.splitlines()
来源：http://xtq.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mob.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://tuv.zhengqikj.top

TS:   s.split(/\r?\n/)
来源：http://xab.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://jth.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://qqu.xuanzx.com

Ruby: s.lines
来源：http://ana.aizwys.cn

C#:   s.Split('\n')
来源：http://cmh.gotoacloud.top

[E20] 判断字符串是否为空
来源：http://gcx.jyoumei.cn

Py:   if not s:
来源：http://xnp.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cvw.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kgh.fktsv.cn

TS:   if (s === "") {}
来源：http://aoy.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://gln.gaohongyu789.top

Go:   if s == "" {}
来源：http://mhm.cashguo.top

Ruby: if s.empty?
来源：http://upc.zycfv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xsg.jqgfzy.top

[E21] 超长截断加省略号
来源：http://onj.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hkk.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rcu.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://drs.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pyr.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gkn.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://xhq.cqqwz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://elg.svipenyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ejm.fengsongda.top

[E22] 字节长度与字符长度
来源：http://sln.andypj.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tnv.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ncj.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iki.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cae.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wmz.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rhu.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://egw.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fob.yvedp.cn

================================================================================
来源：http://osy.c1oappe.top

F. 文件与目录
来源：http://dky.zhaomingkeji.xyz

================================================================================
来源：http://wmg.yuanzhike.top

[F01] 读取整个文件
来源：http://vul.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rcd.jinqigufen.top

PHP:  file_get_contents("a.txt");
来源：http://dke.zhaomingkeji.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blc.jinyuanbaomall.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kop.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://btn.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pbj.meibo888.top

Ruby: File.read("a.txt")
来源：http://wcw.svipenyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://gqm.jyoumei.cn

[F02] 逐行读取文件
来源：http://bfb.hesvh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rqv.svipenyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ktn.yonumen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hre.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dsh.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zmr.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://izx.sysykeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://moo.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qev.zdbjq.cn

[F03] 写入文件（覆盖）
来源：http://zeg.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gdz.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://txn.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qjd.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://szt.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mnm.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pjd.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://gur.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jkk.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://vmz.feifeiyinyue.top


<!-- 参考信息 -->