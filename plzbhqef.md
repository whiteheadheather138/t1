代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rdh.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://szn.jianghu66.top

C#:   list.Max();  list.Min()
来源：http://wmi.hywenlv.cn

[D18] 扁平化嵌套数组
来源：http://qeq.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wct.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://rqg.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zed.yangfankeji.com

TS:   nested.flat();
来源：http://frm.yongpay.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://meo.uphjek.com

Go:   // 手写双层循环
来源：http://zei.gzhubu.top

Ruby: nested.flatten
来源：http://ukp.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://hol.shuidangran.top

[D19] 按字段分组
来源：http://odd.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hsh.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://izi.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tmt.ctjpmb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://zks.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://euk.jyoumei.cn

Go:   // 手写 map[string][]T
来源：http://egz.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://btj.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pbe.zdbjq.cn

[D20] 统计每个元素出现次数
来源：http://qko.yuanzhike.top

Py:   Counter(arr)
来源：http://wzm.ybcxt.top

PHP:  array_count_values($arr);
来源：http://zsz.cucudq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nye.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qib.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cqv.fzhhl.top

Go:   // 手写 map[T]int
来源：http://ufm.cashguo.top

Ruby: arr.tally
来源：http://xpi.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ply.bjfxy.top

[D21] 判断是否包含某元素
来源：http://jrr.cqqwz.cn

Py:   x in arr
来源：http://czc.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://umv.xuanzx.com

JS:   arr.includes(x)
来源：http://fcv.yj20258.top

TS:   arr.includes(x)
来源：http://hbm.yvedp.cn

Java: list.contains(x)
来源：http://hvw.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://uwj.aibaodan.cn

Ruby: arr.include?(x)
来源：http://xla.zhongyouzk.top

C#:   list.Contains(x)
来源：http://shr.hysaishi.cn

[D22] 复制数组（避免共享引用）
来源：http://mgw.zhixingplan.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rms.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zkg.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nwf.bjfxy.top

TS:   [...arr];
来源：http://ddc.zycfv.cn

Java: new ArrayList<>(list);
来源：http://chl.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://fsp.shangyingyoupin.top

Ruby: arr.dup;  arr.clone
来源：http://cdl.xziqi.cn

C#:   new List<int>(list);
来源：http://jtz.yj20258888.top

[D23] reduce 累积计算
来源：http://tdo.xingfuxueyuan.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rjk.xuanzx.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tvu.ywan-chungtsiang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nhg.xziqi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sfm.xuetiantiany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nco.zhoulong.xyz

Go:   // 手写循环
来源：http://oha.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hox.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ers.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://vca.jqgfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cie.uphjek.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zuf.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bpu.gaohongyu789.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lnu.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qzy.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ezu.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wor.shanyushiyangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ppb.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://fuh.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rhj.fehbvm.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bnf.jinyuanbaomall.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vpg.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jsj.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vsw.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hcw.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fbx.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gxa.xziqi.cn

[D26] 数组转字符串
来源：http://dfd.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://yzm.hcnkem.com

PHP:  implode(", ", $arr);
来源：http://vsa.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://hzj.kuanghao11.cn

TS:   arr.join(", ")
来源：http://rxs.sweek.top

Java: String.join(", ", list)
来源：http://hvb.zhaomingkeji.xyz

Go:   strings.Join(strs, ", ")
来源：http://yhk.meibo888.top

Ruby: arr.join(", ")
来源：http://myq.chenjidiqi.icu

C#:   string.Join(", ", list)
来源：http://ezl.zhijiandao.cn

================================================================================
来源：http://mqq.sxryk.cn

E. 字符串处理
来源：http://lew.hysaishi.cn

================================================================================
来源：http://fuq.cheryme.top

[E01] 拼接字符串
来源：http://aed.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hhw.aizwys.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hus.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wke.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jfy.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ozz.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://elc.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xhv.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qmn.cheryme.top

[E02] 重复字符串
来源：http://hxl.zhongyouzk.top

Py:   "ab" * 3
来源：http://rnh.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://mau.daria6918.cn

JS:   "ab".repeat(3)
来源：http://nep.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://jwe.ctjpmb.com

Java: "ab".repeat(3)
来源：http://qhh.gaohongyu789.top

Go:   strings.Repeat("ab", 3)
来源：http://ght.yuanzhike.top

Ruby: "ab" * 3
来源：http://txi.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nmy.feifeiyinyue.top

[E03] 截取子串
来源：http://dud.jiagoushi.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sdo.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vun.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ona.jinqigufen.top

TS:   s.slice(1, 4)
来源：http://aex.daxiang520.top

Java: s.substring(1, 4)
来源：http://dcj.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pwa.bjfxy.top

Ruby: s[1, 3];  s[1..3]
来源：http://mzd.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://mcq.jinqigufen.top

[E04] 查找子串位置
来源：http://ami.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://rmg.9152youxi.cn

PHP:  strpos($s, "x");
来源：http://nft.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://anl.sweek.top

TS:   s.indexOf("x")
来源：http://wcn.sweek.top

Java: s.indexOf("x")
来源：http://oam.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://cee.andypj.xyz

Ruby: s.index("x")
来源：http://fuc.tanke756.top

C#:   s.IndexOf("x")
来源：http://tyt.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uvr.epnwcf.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ljr.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jnh.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yqi.shanyushiyangtech.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rwa.aibaodan.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zgd.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uco.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ptt.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tpt.gaohongyu789.top

[E06] 替换子串
来源：http://bgr.yuxming.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mhz.nanxuanxn.top

PHP:  str_replace("a", "b", $s);
来源：http://kdb.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jzd.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://rka.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kif.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dup.yueranfly.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mwl.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://rfl.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://qvj.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://brx.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jdi.pycfn.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://opu.sxryk.cn

TS:   s.split(",")
来源：http://fxt.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://vdl.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://suj.jyoumei.cn

Ruby: s.split(",");  s.split
来源：http://fxa.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gah.cheryme.top

[E08] 数组按分隔符合并
来源：http://buq.ybcxt.top

Py:   ",".join(items)
来源：http://ryt.vehdjk.com

PHP:  implode(",", $items);
来源：http://blb.shzxlz.cn

JS:   items.join(",")
来源：http://akw.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://gdd.zhixingplan.top

Java: String.join(",", items)
来源：http://ayn.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://cjm.nanxuanxn.top

Ruby: items.join(",")
来源：http://xxo.fehbvm.com

C#:   string.Join(",", items)
来源：http://vnq.wangshuangyany.cn

[E09] 去除所有空白字符
来源：http://pal.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ead.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://exn.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://ygu.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://jyu.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://umb.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kol.snrcjt.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xmj.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ctl.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://wjq.shangyingyoupin.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qgf.jinyuanbaomall.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cyg.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://hue.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://rif.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://zho.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zvn.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pwj.smart0.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ahi.sxryk.cn

[E11] 反转字符串
来源：http://uoq.jinqigfzy.top

Py:   s[::-1]
来源：http://rnt.aibaodan.cn

PHP:  strrev($s);
来源：http://nfb.hammf.cn

JS:   [...s].reverse().join("")
来源：http://igt.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://jzf.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kzt.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vyy.xinyue.icu

Ruby: s.reverse
来源：http://ycz.zhiwuduotai.top

C#:   new string(s.Reverse().ToArray())
来源：http://doe.wangdashe.top

[E12] 统计某字符出现次数
来源：http://gpl.wangdashe.top

Py:   s.count("a")
来源：http://iqu.ehwqpu.com

PHP:  substr_count($s, "a");
来源：http://nnv.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://hyt.bjfxy.top

TS:   s.split("a").length - 1
来源：http://qlu.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kgz.jianghu66.top

Go:   strings.Count(s, "a")
来源：http://tja.zhiwuduotai.top

Ruby: s.count("a")
来源：http://znd.sweek.top

C#:   s.Count(c => c == 'a')
来源：http://tas.zhoulong.xyz

[E13] 逐字符遍历
来源：http://asu.chenjidiqi.icu

Py:   for ch in s: print(ch)
来源：http://xig.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jcn.yj202588.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://smh.jqgfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hfb.chenlongwang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yhw.hesvh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tyi.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hoz.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ntp.birdmap.top

[E14] URL 编码与 Base64
来源：http://crd.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aax.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://exw.tarul.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xls.jyoumei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zza.ydjk.org.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ubi.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pmn.zdbjq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xtj.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zzh.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://iuv.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hsu.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://auz.guowangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pwy.sxryk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wjk.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ixo.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bsf.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gqi.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://all.daxiang520.top

[E16] 数字千分位
来源：http://ott.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://wti.birdmap.top

PHP:  number_format(1234567);
来源：http://hoe.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bkg.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://pca.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xwv.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mjk.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ptc.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://mxv.nanxinkj.top

[E17] 首字母大写
来源：http://kxb.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qym.yj20258.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://usm.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://otv.bjfxy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lgo.xingfuxueyuan.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gwn.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ijv.zhixingplan.top

Ruby: s.capitalize
来源：http://tla.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://klz.kuanghao11.cn

[E18] 模板占位符替换
来源：http://mlw.pycfn.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nlx.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kjb.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ulw.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://grl.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eba.cheryme.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vtr.yuanzhike.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hdf.hongshengwenyu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cyy.yueranfly.top

[E19] 多行文本按行拆分
来源：http://rzd.guannengcc.top

Py:   s.splitlines()
来源：http://jtl.yvedp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uts.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://doe.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://rli.hnqzz.top

Java: s.lines().toList()
来源：http://ywl.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://eef.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://aag.dianchejie.cn

C#:   s.Split('\n')
来源：http://paf.tanke756.top

[E20] 判断字符串是否为空
来源：http://lnp.zhijiandao.cn

Py:   if not s:
来源：http://hrb.ivvv.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vwp.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kyl.wangdashe.top

TS:   if (s === "") {}
来源：http://nql.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://wgp.vehdjk.com

Go:   if s == "" {}
来源：http://btr.nanxuanxn.top

Ruby: if s.empty?
来源：http://lrs.cucudq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nni.guowangkeji.top

[E21] 超长截断加省略号
来源：http://nfy.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lim.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hcg.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://utu.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://afq.cdnleiting.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rkd.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://fem.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gqn.hfpthk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xbc.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://kma.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mga.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://laa.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uvk.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tox.dianchejie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gdb.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wjx.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://mbo.cheryme.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zyp.xinyue.icu

================================================================================
来源：http://zzb.jyoumei.cn

F. 文件与目录
来源：http://dfv.iojbl.cn

================================================================================
来源：http://uyo.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://zry.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hvg.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://erm.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ljk.cheryme.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lzf.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jwd.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://acf.guannengcc.top

Ruby: File.read("a.txt")
来源：http://omc.yfazqb.com

C#:   File.ReadAllText("a.txt");
来源：http://xyz.zhongyouzk.top

[F02] 逐行读取文件
来源：http://nsr.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kik.hesvh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jzb.yj202588.top


<!-- 参考信息 -->