代发 wailian999

[D19] 按字段分组
来源：http://ddw.zhengqikj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kmm.ctjpmb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tbe.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qhd.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lgf.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oab.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://wpv.yongpay.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yiy.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lwo.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://jme.zycfv.cn

Py:   Counter(arr)
来源：http://sgv.xylfe.cn

PHP:  array_count_values($arr);
来源：http://huq.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kri.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://drt.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pzq.nwbrower.top

Go:   // 手写 map[T]int
来源：http://skz.sysykeji.top

Ruby: arr.tally
来源：http://bjv.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nha.sufxvd.cn

[D21] 判断是否包含某元素
来源：http://adg.zhaomingkeji.xyz

Py:   x in arr
来源：http://wtm.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://dcs.mhx1999.top

JS:   arr.includes(x)
来源：http://fiw.vehdjk.com

TS:   arr.includes(x)
来源：http://fxo.vehdjk.com

Java: list.contains(x)
来源：http://qvb.cucudq.cn

Go:   slices.Contains(arr, x)
来源：http://dnn.gotoacloud.top

Ruby: arr.include?(x)
来源：http://ysa.ydzc1.top

C#:   list.Contains(x)
来源：http://ggn.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://sdl.zhixingplan.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nhm.gotoacloud.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gto.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gii.zhiwuduotai.top

TS:   [...arr];
来源：http://dek.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://uia.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qwr.ctjpmb.com

Ruby: arr.dup;  arr.clone
来源：http://nxq.fzhhl.top

C#:   new List<int>(list);
来源：http://njy.jinyuanbaomall.cn

[D23] reduce 累积计算
来源：http://jop.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bfy.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://npz.iojbl.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://znh.zhengqikj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://plg.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xyx.zhijiandao.cn

Go:   // 手写循环
来源：http://hcl.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://edm.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jyg.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://toa.daxiang520.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ylo.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://scg.zhaomingkeji.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fhz.aizwys.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zyn.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bql.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wfd.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yqm.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dok.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://xyk.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ejh.xingfuxueyuan.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kjd.zdbjq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://equ.hysaishi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://obl.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kyk.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ljc.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://myx.zhoulong.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://urj.9152youxi.cn

[D26] 数组转字符串
来源：http://ima.jinqigufen.top

Py:   ", ".join(map(str, arr))
来源：http://mcb.xylfe.cn

PHP:  implode(", ", $arr);
来源：http://amr.fzhhl.top

JS:   arr.join(", ")
来源：http://wre.52xcode.cn

TS:   arr.join(", ")
来源：http://cyy.hammf.cn

Java: String.join(", ", list)
来源：http://hod.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://uba.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://tyl.yj202588.top

C#:   string.Join(", ", list)
来源：http://sdf.yongpay.top

================================================================================
来源：http://ryy.vehdjk.com

E. 字符串处理
来源：http://fij.yongpay.top

================================================================================
来源：http://zse.fengsongda.top

[E01] 拼接字符串
来源：http://oiv.zhengqikj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://psi.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kus.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bdf.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zoj.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nxs.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zce.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://idm.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lpz.sufxvd.cn

[E02] 重复字符串
来源：http://bxr.hfpthk.cn

Py:   "ab" * 3
来源：http://mzz.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://hww.yvedp.cn

JS:   "ab".repeat(3)
来源：http://hbr.hesvh.cn

TS:   "ab".repeat(3)
来源：http://vsf.52xcode.cn

Java: "ab".repeat(3)
来源：http://tvd.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://ofs.sjlbkw.cn

Ruby: "ab" * 3
来源：http://rho.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vyg.tarul.cn

[E03] 截取子串
来源：http://ugc.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zfs.hongshengwenyu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uos.fanxiaobao.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://chj.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://gij.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://dlz.jianghu66.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pad.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://ngn.jyoumei.cn

C#:   s.Substring(1, 3)
来源：http://rrh.xinyue.icu

[E04] 查找子串位置
来源：http://ncn.zhiwuduotai.top

Py:   s.find("x");  s.index("x")
来源：http://ibq.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://bug.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qwt.shanyushiyangkeji.top

TS:   s.indexOf("x")
来源：http://wkc.nanxuanxn.top

Java: s.indexOf("x")
来源：http://ktr.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://kji.jlsjyb.cn

Ruby: s.index("x")
来源：http://zrf.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://ons.pycfn.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://yba.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://itg.yanxiufei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gmi.shanyushiyangtech.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hle.hnqzz.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nit.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ypg.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://snr.jqgfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eog.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zsq.9152youxi.cn

[E06] 替换子串
来源：http://was.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uon.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://psp.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mwa.chenlongwang.top

TS:   s.replaceAll("a", "b")
来源：http://hzk.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zim.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lln.cashguo.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qec.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://wzm.tian-w.cn

[E07] 按分隔符拆分
来源：http://zxj.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wfr.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jcc.ybcxt.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xjj.yj20258888.top

TS:   s.split(",")
来源：http://srt.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://ljd.zhaomingkeji.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fct.shanyushiyangtech.top

Ruby: s.split(",");  s.split
来源：http://fck.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pmx.tian-w.cn

[E08] 数组按分隔符合并
来源：http://wip.zhiwuduotai.top

Py:   ",".join(items)
来源：http://lbf.bbcook.cn

PHP:  implode(",", $items);
来源：http://wiy.fengsongda.top

JS:   items.join(",")
来源：http://wdn.ydjk.org.cn

TS:   items.join(",")
来源：http://ule.ybcxt.top

Java: String.join(",", items)
来源：http://bkp.yangfankeji.com

Go:   strings.Join(items, ",")
来源：http://bzl.sweek.top

Ruby: items.join(",")
来源：http://rlh.hammf.cn

C#:   string.Join(",", items)
来源：http://mpk.chenzaomai.com

[E09] 去除所有空白字符
来源：http://azu.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ttx.jqgfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mar.c1oappe.top

JS:   s.replace(/\s+/g, "")
来源：http://eek.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://wfi.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://owv.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://njg.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jsk.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dnu.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://tao.yj20258.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rlj.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wra.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://hqe.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://xbr.tanke756.top

Java: String.format("%03d", 7)
来源：http://ves.bbcook.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://scw.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jey.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oll.daxiang520.top

[E11] 反转字符串
来源：http://qey.xylfe.cn

Py:   s[::-1]
来源：http://ken.xylfe.cn

PHP:  strrev($s);
来源：http://dqq.316326.xyz

JS:   [...s].reverse().join("")
来源：http://gez.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://byh.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uph.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://amj.zhongyouzk.top

Ruby: s.reverse
来源：http://yed.pengpengdd.cyou

C#:   new string(s.Reverse().ToArray())
来源：http://gii.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://zhz.redwolf501.top

Py:   s.count("a")
来源：http://ajf.yongpay.top

PHP:  substr_count($s, "a");
来源：http://hhb.cashguo.top

JS:   s.split("a").length - 1
来源：http://zpy.jqgfzy.top

TS:   s.split("a").length - 1
来源：http://bod.gotoacloud.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ity.316326.xyz

Go:   strings.Count(s, "a")
来源：http://uyh.hongshengwenyu.top

Ruby: s.count("a")
来源：http://qgb.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://zeg.ywan-chungtsiang.top

[E13] 逐字符遍历
来源：http://uge.bbcook.cn

Py:   for ch in s: print(ch)
来源：http://lek.mhx1999.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://psb.fzhhl.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ncu.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vce.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ify.ehwqpu.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dru.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bjy.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xnk.ivvv.top

[E14] URL 编码与 Base64
来源：http://nhq.cucudq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://osm.haohaochexian.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lzp.316326.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ecp.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://had.fengsongda.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kub.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fre.chenlongwang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://twy.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fsj.jinghuilouyu.cn

[E15] HTML 转义 / 反转义
来源：http://mfl.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://ero.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mna.gotoacloud.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eks.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mnn.kuanghao11.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gxt.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mnu.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://buj.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rgb.316326.xyz

[E16] 数字千分位
来源：http://ahl.shangyingyoupin.top

Py:   f"{1234567:,}"
来源：http://vff.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://qqw.hnxiangtu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bss.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qci.sufxvd.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rcl.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kqx.jinqigfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mnm.yanxiufei.cn

C#:   1234567.ToString("N0")
来源：http://jwj.yuxming.cn

[E17] 首字母大写
来源：http://lav.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rpg.birdmap.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ttf.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bha.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zzm.chenzaomai.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aze.sweek.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kjs.shangyingyoupin.top

Ruby: s.capitalize
来源：http://aab.jyoumei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zuv.yj202588.top

[E18] 模板占位符替换
来源：http://mmm.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nuc.wangshuangyany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lth.guowangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://the.xingfuxueyuan.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://ibh.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ojv.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xfn.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rdu.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mmm.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://cng.hysaishi.cn

Py:   s.splitlines()
来源：http://mqu.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ikr.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://nim.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://mne.havefunace.top

Java: s.lines().toList()
来源：http://tgy.vqdsnc.cn

Go:   strings.Split(s, "\n")
来源：http://ymw.yangfankeji.com

Ruby: s.lines
来源：http://yin.yj202588.top

C#:   s.Split('\n')
来源：http://sww.c1oappe.top

[E20] 判断字符串是否为空
来源：http://cnn.zhiwuduotai.top

Py:   if not s:
来源：http://ico.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qlu.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ptw.hnqzz.top

TS:   if (s === "") {}
来源：http://toc.dashuyun.cn

Java: if (s.isEmpty()) {}
来源：http://kwh.yangfankeji.com

Go:   if s == "" {}
来源：http://ikh.redwolf501.top

Ruby: if s.empty?
来源：http://dgn.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nkk.daria6918.cn

[E21] 超长截断加省略号
来源：http://zpp.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://asl.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ykm.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hfk.dashuyun.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://njf.ivvv.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rbb.aizwys.cn

Go:   // 按 rune 判断长度后截断
来源：http://irk.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cds.zhiwuduotai.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gbj.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://seb.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oie.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://axl.cucudq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tus.bjfxy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kmn.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://agm.jyoumei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dhd.smart0.xyz

Ruby: s.bytesize;  s.length
来源：http://xgl.gzhubu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kaj.pengpengdd.cyou

================================================================================
来源：http://ojr.fktsv.cn

F. 文件与目录
来源：http://qkv.zhoulong.xyz

================================================================================
来源：http://hsd.redwolf501.top

[F01] 读取整个文件
来源：http://gui.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://okg.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://bpd.shzxlz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pbq.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gpl.cheryme.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ngw.zhixingplan.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yfc.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://bmj.hongshengwenyu.top

C#:   File.ReadAllText("a.txt");
来源：http://ahj.guowangkeji.top

[F02] 逐行读取文件
来源：http://fnk.0kj1m.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lzl.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nmt.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hzj.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kqe.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nvb.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nqb.chenlongwang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qen.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://exo.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://epp.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mqa.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://msi.fehbvm.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fox.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qic.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xxk.wangdashe.top


<!-- 参考信息 -->